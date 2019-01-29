---
cover: 
description: A successful postmortem process is based on a culture of honesty, learning, and accountability. Culture change requires management buy-in, but you can lead culture change no matter your role. This guide describes common challenges faced in building a culture of continuous learning through postmortems and strategies for overcoming these challenges. 
---
![Blameless](../assets/img/covers/blameless.png)

#The Blameless Postmortem
As IT professionals, we understand that failure is inevitable in complex systems. **How we respond to failure when it occurs matters.** In *The Field Guide to Understanding Human Error*, Sidney Dekker describes two views on human error: 1) the old view, which asserts that people’s mistakes cause failure, and 2) the new view, which treats human error as a symptom of a systemic problem. The old view ascribes to “the bad apple theory,” which believes that removing bad actors will prevent failure. This view attaches an individual's character to their actions, assuming negligence or bad intent leads to the error. 

An organization that follows this old view of human error may respond to an incident by finding the careless individual who caused the incident so they can be reprimanded. **This impulse to blame and punish has the unintended effect of disincentivizing the knowledge sharing required to prevent future failure.** Engineers will hesitate to speak up when incidents occur for fear of being blamed. This silence increases overall mean time to acknowledge, mean time to resolve, and exacerbates the impact of incidents. 

For the postmortem process to result in learning and system improvements, the new view of human error must be followed. In complex systems of software development, a variety of conditions interact to lead to failure. **The goal of the postmortem is to understand what systemic factors led to the incident and identify actions that can prevent this kind of failure from recurring.** A blameless postmortem stays focused on _how_ a mistake was made instead of _who_ made it. This is a crucial mindset leveraged by many leading organizations, such as Etsy (a pioneer for [blameless postmortems](https://codeascraft.com/2012/05/22/blameless-postmortems/)), for ensuring postmortems have the right tone, empowering engineers to give truly objective accounts of what happened by eliminating the fear of punishment.


# Why Blamelessness Is Hard
It is easy to agree that we want a culture of continuous improvement, but it is difficult to practice the blamelessness required for learning. The unexpected nature of failure naturally leads humans to react in ways that interfere with our understanding of it. When processing information, the human mind unconsciously takes shortcuts. By applying general rules-of-thumb, the mind optimizes for timeliness over accuracy. When this produces an incorrect conclusion, it is a cognitive bias.

[J. Paul Reed](https://techbeacon.com/blameless-postmortems-dont-work-heres-what-does) argues the blameless postmortem is a myth because the tendency to blame is hardwired through millions of years of evolutionary neurobiology. Ignoring this tendency or trying to eliminate it entirely is impossible. It is more productive to be “blame aware.” **By being aware of our biases, we will be able to identify when they occur and work to move past them.** We touch upon some of the biases below, but for more details, read [Lindsay Holmwood's](http://fractio.nl/2015/10/30/blame-language-sharing/) article on the cognitive biases we must be aware of when performing postmortems. 

**[Fundamental attribution error](https://en.wikipedia.org/wiki/Fundamental_attribution_error)** is the tendency to believe that what people do reflects their character rather than their circumstances. This describes the old view of human error, assigning responsibility for a failure to bad actors who are careless and incompetent. Ironically, we tend to explain our own actions by our context, not our personality. Combat this tendency to blame by intentionally focusing the analysis on situational causes rather than discrete actions individuals took.  

Another pervasive cognitive bias is **confirmation bias**, which is the tendency to favor information that reinforces existing beliefs. When presented with ambiguous information, we tend to interpret it in a way that supports our existing assumptions. When combined with the old view of human error, this bias is dangerous for postmortems because it seeks to blame the bad apple. When approaching the analysis with the assumption that an individual is at fault, you will find a way to support that belief despite evidence to the contrary. 

To combat confirmation bias, Holmwood suggests appointing someone to play devil’s advocate to take contrarian viewpoints during investigations. Be cautious of introducing negativity or combativeness with a devil’s advocate. You can also counter confirmation bias by inviting someone from another team to ask any and all questions that come to their mind. This will help surface lines of inquiry the team has learned to take for granted. 

**Hindsight bias** is a type of memory distortion where we recall events to form a judgment. Knowing the outcome, it is easy to see the event as being predictable despite there having been little or no objective basis for predicting it. Often, we recall events in a way to make ourselves look better. An example is when a person analyzing the causes of an incident believes they knew it would happen like that. Enacting this bias can lead to defensiveness and division within a team. Holmwood suggests avoiding the hindsight bias by explaining events in terms of foresight instead. Start your timeline analysis at a point before the incident and work your way forward instead of backward from resolution. 

Another common bias to be aware of is **[negativity bias](https://en.wikipedia.org/wiki/Negativity_bias)**. This is the notion that things of a more negative nature have a greater effect on one’s mental state than those of neutral or even positive nature. Research on social judgments has shown negative information disproportionately impacts a person’s impression of others. This relates to the “bad apple theory,” the belief that there are negative actors in your organization to blame for failures. Studies have also shown people are more likely to attribute negative outcomes to the intentions of another person than neutral and positive outcomes. This also explains our tendency to blame individuals’ characters to explain a major incident. 

In reality, things go right more often than they go wrong, but we tend to focus on and magnify the importance of negative events. Focusing on, exaggerating, and internalizing incidents as negative events can be demoralizing and lead to burnout. Reframing incidents as learning opportunities and remembering to describe what was handled well in your response can help balance perspective. 

## Cognitive Biases

| Bias | Definition | Countermeasure |
|---|---|---|
| Fundamental attribution error | What people do reflects their character rather than their circumstances. |   |Intentionally focus the analysis on situational causes rather than discrete actions individuals took. |
| Confirmation bias | Favoring information that reinforces existing positions. | Appoint someone to play devil’s advocate to take contrarian viewpoints during investigations. |
| Hindsight bias | Seeing the incident as inevitable despite there having been little or no objective basis for predicting it because we know the outcome. | Explain events in terms of foresight instead. Start your timeline analysis at a point before the incident, and work your way forward instead of backward from resolution. |
| Negativity bias | Things of a more negative nature have a greater effect on one’s mental state than neutral or even positive things. | Reframe incidents as learning opportunities, and remember to describe what was handled well in incident response. |

We all have these cognitive biases that can lead to distorted views of events and damage team relationships if gone unchecked. It is important to be aware of these tendencies so we can acknowledge bias when it occurs. By making postmortems a collaborative process, teams can work as a group to identify blame and then constantly dig deeper in the analysis.  


# How to Avoid Blame
Acknowledging blame and working past it is easier said than done. What behaviors can we adopt to move towards a blameless culture? Holmwood eloquently writes about the importance of the words we use to minimize blame and maximize learning. He urges us to ask “what” questions(e.g., “What did you think was happening?” and “What did you do next?” Asking “what” questions grounds the analysis in the big-picture contributing factors to the incident.  

In his article “[The Infinite Hows](https://www.oreilly.com/ideas/the-infinite-hows),” John Allspaw encourages us to ask “how” questions because they get people to describe (at least some of) the conditions that allowed an event to take place. Holmwood also notes that “how” questions can help clarify technical details, distancing people from the actions they took. Avoid asking “why” questions because it forces people to justify their actions, attributing blame.

[Crucial Accountability](https://www.vitalsmarts.com/crucial-accountability-training/)  offers a helpful framework for approaching difficult conversations about unmet expectations that can be applied to postmortems when emotions run high. When analyzing failure, we may fall into victim, villain, and helpless stories that propel emotions and attempt to justify our worst behaviors. You can move beyond blame by telling the rest of the story. Consider your and others’ roles in the problem. Ask yourself why a reasonable, rational, and decent person may have taken the action that seems to have caused the incident. This thinking will help turn attention to the multiple systemic factors that led to the incident. 

Even when you have made a best effort to remain blameless, it is possible someone may still become defensive during a postmortem meeting if they feel they are being blamed. When this happens, work to restore mutual purpose and mutual respect so a productive discussion can continue. Restore mutual purpose by reiterating that the goal of the postmortem is to understand what systemic factors lead to the incident and collaboratively identify actions that can reduce failure moving forward. Often, people act out defensively when they feel their character is being attacked. Restore mutual respect by contrasting. Say what you did not intend (“I did not mean to imply you’re bad at your job.”) contrasted with what you do intend (“I meant to inquire to the situational factors that would lead any responder to take that action.”) Refocus your inquiry away from individual motivation, which implies blame. Abstracting to an inspecific responder also encourages other responders to contribute more suggestions as to what could have contributed to the system failure. 

!!! info "Key Takeaways"
    * Ask “what” and “how” questions rather than “who” or “why.”
    * Consider multiple and diverse perspectives.
    * Ask yourself why a reasonable, rational, and decent person may have taken a particular action.
    * When inquiring about a human action, abstract to an inspecific responder. Anyone could have made the same mistake. 
    * Restore mutual purpose and mutual respect by contrasting what you did not intend with what you do intend.

