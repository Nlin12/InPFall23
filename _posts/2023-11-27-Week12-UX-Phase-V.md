---
layout: post
title: Week 12-UX Design Research-Phase V
subtitle: 
tags: []
---

### Introduction

After conducting research on the users using fly-on-the-wall observation and contextual inquiry, and running a preliminary analysis on the findings, I developed some initial ideas for the prototype of my project. For Phase V, I will design a higher fidelity prototype, and develop narratives for the design.

### Prototype ideas

In the previous phase, I developed 3 ideas to improve the experience of newcomers and visitors navigating the road crossings in NYC. They are:

##### 1. The car-sensing signal

This idea focuses on the "danger prevention" side, since I noticed the view of the road is often blocked by parking cars or other obstacles. Devices that can sense whether a vehicle is approaching are not uncommon, and they can provide valuable information for pedestrians that warns them of imminent danger.

![Storyboard]({{ '/assets/img/W12/Storyboard1.jpeg' | relative_url }})

##### 2. The interactive billboard

Many pedestrians, locals and tourists alike, are not paying enough attention when they are crossing the street. They either are attached to their smartphones or are paying attention to their surroundings, especially in places like Times Square. Therefore, I proposed this way of grabbing their attention back and providing warnings on road safety.

![Storyboard]({{ '/assets/img/W12/Storyboard2.jpeg' | relative_url }})

##### 3. The wisdom of the crowd

During my research, I observed that crowd behavior has a great influence on individual decision-making. Especially for people not familiar with the city, they will rely on others as a reference. However, such "model" will not always be available (or there might be bad ones), making them susceptible to unexpected hidden dangers, or carrying a false sense of danger on the streets. I proposed constructing "digital pedestrians" based on past recorded crowd behaviors, and presenting them through augmented reality, which can act as a virtual sensei for newcomers.

![Storyboard]({{ '/assets/img/W12/Storyboard3.jpeg' | relative_url }})

As mentioned last week, since these 3 ideas each focus on a different aspect of the problem, I want my final solution to be a combination of them, especially since they all somewhat involve the usage of electronic displays and environment-sensing technologies.

### Revisit the Results & Connecting the Dots

With some general directions in mind, I dug deeper into my research findings and analyzed some early-stage feedback I got from both participants and in class, hoping to find inspiration on integrating these different aspects and goals into a complete experience.

Although my POV is around people unfamiliar with navigating the streets of NYC, one behavior that is shared across the board is the tendency to follow the crowd. For locals, acting in numbers makes everyone in the group more salient to drivers on the road and thus safer; Furthermore, for newcomers, this is also a major social factor and the source of learning through mimicing. Therefore using this power of crowds, it might be possible to actively influence pedestrian behavior.

Another observation that is shared by locals and newcomers is the lack of enough attention and awareness on the road, though for slightly different reasons. While locals are focusing mainly on their phones, I find some tourists are instead attracted by their surroundings, especially by the dazzling billboards of Times Square. Rethinking it, I realized that this is because the billboards are functioning exactly as they should: they are being attractive to people, while the roads under their feet are not.

That's when I got an idea: instead of blaming phones or cityscapes for being "too attractive", why not try to the roads that we commute on "attractive" too? I think if we can make people pay attention to the road without forcing them to do so, that would be the most ideal and sustainable solution.

Separately, some feedback I received previously also noted that compared to a regulatory or limiting implementation, a more artistic and engaging approach would be easier for people to accept, and can also avoid some of the possible legal problems. Therefore, I think this would be a promising direction of design.

What's more, adding interactivity and community engagement are also mentioned, which make sense because they are places where the current system lacks: Traffic signs and signals only show instruction but don't provide situational feedback, and how to properly navigate the streets, just like many other things in NYC, are unspoken wisdom that are not explicitly documented and can't be easily obtained.

### Prototyping

**Hypothesis:** If an interactive and engaging pedestrian information system that can attract pedestrians' attention and provide situation-aware guidance and warning on road-crossing behavior is installed, then newcomers and tourists of NYC can be safer and more efficient on the road.

**Success Metrics:** Safety-wise, traffic accidents involving pedestrians among newcomers and tourists should decrease; Behavior-wise, the behavior pattern of those groups will be more similar to local residents.

With the idea of fusing the informative and interactive nature of a "senpai" system, and the attractiveness of billboards in mind, I started to prototype the looks and features of the system. It is pretty obvious that a digital display would be the most reasonable medium, and I mainly have 2 ideas for the placement: one is embedded on the ground, and shaped like an "enhanced" zebra line; the other one is a vertical sign (kind of like the digital Passenger Information Display System (PIDS)s installed in the subway). Each implementation has its strengths and weaknesses, and there's also the possibility of combining them together.

The "virtual reference pedestrian" part is pretty straightforward: I used footprints, and virtual humans in an AR environment respectively to create the feeling of a crowd that can be used to guide pedestrians in their behavior. The pattern of these virtual pedestrians should be constructed from learning the actual behavioral patterns of pedestrians at this place, thus it can be a more flexible system compared to traditional traffic signals, and have the environment awareness to make the information provided more accurate and relevant.

![Prototype]({{ '/assets/img/W12/Prototype1.png' | relative_url }})

![Prototype]({{ '/assets/img/W12/Prototype2.png' | relative_url }})

But it's a bit trickier when it comes to creating an engaging and attractive experience for the pedestrian, particularly for newcomers and tourists. This is when my previous thoughts and experiments with culture-building and the use of humor in city spaces gave me inspiration. In my 50 Shades project, I tried making subway signs more fun, engaging, and informative by infusing humor and subway cultures into them. I think the same can be done to these pedestrian information systems. Instead of being serious and uniform, playful and location-specific designs could be more effective in drawing consistent attention.

I prototyped some possible implementations of this idea. For example, adding a "Do you know" section that provides interesting facts about the places around. This is especially suitable for visitors at tourist attractions. Even relevant ads can be used to our advantage, such as using humor to provide tips while promoting brands at the same time.

Finally, to reinforce the idea of "learning from the locals", and to invite input from the communities, I imagined a mechanism for "tips sharing", where locals can share what they feel useful to know on the streets and in the neighborhood, and have their tips displayed accordingly depending on the situation.

![Prototype]({{ '/assets/img/W12/Prototype3.png' | relative_url }})

![Prototype]({{ '/assets/img/W12/Prototype4.png' | relative_url }})

Finally, I created some rough mockups to show how they would generally look like on the streets.

![Mock]({{ '/assets/img/W12/Mock1.png' | relative_url }})

![Mock]({{ '/assets/img/W12/Mock2.png' | relative_url }})

### Conclusion

I'm surprised that just by revisiting the research results and feedback with new perspectives or objectives, I was able to draw so many more insights from them. This shows that in addition to ensuring abundant research, making sure you're taking full advantage of your research data is also important. What's more, personal knowledge and past experiences, although they may seem irrelevant at first, can become of great use in unexpected places.

Next week, I'm going to focus on iterating and putting together a more systematic and polished narrative.
