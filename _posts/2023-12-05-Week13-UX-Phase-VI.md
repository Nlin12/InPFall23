---
layout: post
title: Week 13-UX Design Research-Phase VI
subtitle: 
tags: []
---

### Introduction

During the last phase, I developed prototypes based on previous research findings and initial ideas. In this last phase of the UX design process, I will be focusing on making more iterations and adjustments to my prototypes and creating a cohesive narrative of my project and findings.

### Feedbacks & Iteration

After I developed the prototypes that showed 2 ways of how the system would look like, I went and got some feedback from a couple of people. Some recently moved to NYC, and some either have visited or intend to visit NYC. Considering the small sample size and the fact that the process is not conducted in an actual road-crossing setting, I did not go with structured, quantitative measurements. Instead, I just collected their general qualitative opinion to help me evaluate the direction I'm going and find potential problems. I focused on two aspects: 1. Will the system attract the attention of pedestrians; 2. Will the pedestrian follow the directions provided by the system, since they correspond to the 2 aspects that my design is intended to improve upon the current system. 

Although they all agreed that it would be more salient and attractive than traffic signals/stop signs, some did raise the question of whether virtual representations will be compelling enough for people to feel the social influence and be affected by it. It is also questioned whether it's clear enough for pedestrians to understand what it's displaying.

Around the same time when I was thinking about how to improve, I randomly stumbled upon a video on YouTube on [Shikakeology (仕掛学)](https://youtu.be/QovoN036vz0). It immediately caught my attention, as it focuses on very similar objectives as my project: influencing people's behavior through design. I immediately did some research on this topic. It seems that this is a topic that still has limited recognition and discussion, especially outside Japan, and most of the studies around Shikakeology are related to Professor Naohiro Matsumura. It shares some similarity to the Nudge Theory, however focuses on more indirect approaches and emphasize more on the psychological aspect. Nevertheless, I found some very interesting and relevant cases of applying Shikekalogy, which utilizes people's intrinsic curiosity, as well as the attracting power of seeing others doing something to guide people's behavior through a game-like engaging experience.

![Shikake]({{ '/assets/img/W13/Shikake1.jpg' | relative_url }})

*[The news video](https://youtu.be/QovoN036vz0)*

2 cases of implementation of Shikakeology came out as my favorite. The first is a trash can with a basketball net placed above it. Compared to traditional trash cans, it significantly increases the amount of trash people put in them. Another version of the trash can uses a speaker to simulate the sound of trash dropping for multiple seconds before landing, and is called "the World's Deepest Trash Can". According to Professor Matsumura, some people will collect more trash just to hear the sound again. This design uses people's curiosity to create simple and low-cost "gimmicks" that attract people;

![Shikake]({{ '/assets/img/W13/Shikake2.png' | relative_url }})

*[Source](https://www.rikelab.jp/post/3119.html)*

The second implementation is painting a subway station stair with a poll question: "Where do you prefer to go after work?", and using sensors to record people walking up on either side of the stair as a vote. This is aimed to encourage people to use the stairs more during the rush hours where to escalators will become congested. According to the professor, seeing others engaging with the Shikake also serves as a further motivation for others to participate themselves. Compared to the well-known Nudge Theory, I feel like what Shikakeology is doing focuses more on psychological influences, is more indirect, and often involves a duality of purpose. 

![Shikake]({{ '/assets/img/W13/Shikake3.png' | relative_url }})

*[Source](https://www.rikelab.jp/post/3119.html)*

![Shikake]({{ '/assets/img/W13/Shikake4.jpg' | relative_url }})

*[A similar implementation in Manchester](https://www.linkedin.com/posts/kayceeli_i-believe-this-is-also-called-shikakeology-activity-7088642034143547392-RJco)*

Based on what I have learned about Shikakeology, I modified my prototype and added similar mechanisms.

![Prototype]({{ '/assets/img/W13/Prototype1.png' | relative_url }})

### Final Prototype

Although previously I proposed two forms of the system: one using a ground-mounted display, the other being an upright bulletin-board form, I've decided to only focus on the ground version for the final prototype. Despite some feedback showing more interest in the idea of an AR representation of pedestrians, I feel that such a device will adversely affect the environmental visibility at the road crossings for both drivers and pedestrians. What's more, the two format has most of the features overlapping, and I didn't feel like using AR is bringing significant benefits in terms of creating an engaging presentation. On the contrary, through the prototyping process, I found that the ground display options offer more flexibility to display relevant content and are less cluttered.

![Prototype]({{ '/assets/img/W13/Prototype2.png' | relative_url }})

### Building the Narrative

At this point, the project is entering its final state, I began to look back at the whole process, complete the narrative, and review the works I have done.

In terms of the hypothesis and success metrics, I left the hypothesis from last week unchanged, but changed the success metrics to be more specific and measurable.

**Hypothesis:** If an interactive and engaging pedestrian information system that can attract pedestrians' attention and provide situation-aware guidance and warning on road-crossing behavior is installed, then newcomers and tourists of NYC can be safer and more efficient on the road.

**Success Metrics:** Attractiveness of the system installed at road crossings; The willingness to engage with the system; The conformity of pedestrians to the guidance provided by the system.

I used last week's structure of Human Issue--Tool--Solution--Impact structure to construct and present my narrative. This graph roughly shows my thinking and research process, and how different parts are connected and contributed to each other.

![Storytelling]({{ '/assets/img/W13/Storytelling1.png' | relative_url }})

What I think stood out during my process over the weeks: Firstly, it's important to keep the topic manageable and relevant. At first, I started off targeting the entire pedestrian and driver population and was thinking about building an entirely new set of rules for the traffic. However, I quickly found out that this led to a huge web of conflict of interest, and stakeholders that are virtually unreachable. Therefore I narrowed down the POV to a smaller crowd, and more importantly, a crowd that I and many others around me belong to. This made it way easier to emphasize, engage, and seek feedback; Secondly, although not directly related, I found that the topics and findings I explored during previous projects (like the 50 Shades, Time Capsule) can be of valuable inspiration. This encourages me to look back into the takeaways from previous experiences for guidance.

What I think can be improved: I think I could definitely do more research on my target crowd if time and resource permits. I do find observation and inquiry can be a powerful workflow to gather previously unnoticed findings and then make confirmation and seek explanations. This helps me quickly understand how things currently work and find problems. What's more, I'd also like to conduct some preliminary user tests on my prototype. However, I can imagine this can be challenging, since the test would have to be carried out in a real-world setting. 

### References

Matsumura, N., Fruchter, R. & Leifer, L. Shikakeology: designing triggers for behavior change.                    *AI & Soc* **30**, 419–429 (2015). https://doi.org/10.1007/s00146-014-0556-5

Maho Kozai, Tomoko Yagishi. Making Shikake to promote the separating and sorting of garbage in Otemae High School. (2019). https://www.shikakeology.org/pdf/TBC2019005.pdf

Masatoshi Takeuchi, Naohiro Matsumura. "Osaka Loop Line General Election”--A shikake to ease congestion on the escalator in the station. (2020).  https://shikakeology.org/pdf/TBC2020022.pdf
