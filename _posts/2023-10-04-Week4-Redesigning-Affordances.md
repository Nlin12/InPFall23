---
layout: post
title: Week 4-Redesigning Affordances
subtitle: 
tags: []
---

### TLDR

I proposed using RFID and E-ink based tags to represent in-game items and create a physical game inventory management system.

### Motivation

Playing video games is one of my hobbies. Of the games, Pokémon probably gets the most of my time. Needless to say that Pokémon is very centered around the idea of "possession". The player will catch and possess Pokémon--a lot of them, as well as other items that can be acquired and used in battle--also a lot of them. To make things worse, Pokémon games are not known for their outstanding code quality and game UI/UX, which means the inventory management experience is unintuitive at best. When you're post game and have accumulated a great amount of Pokémon and items, trying to find or modify anything is just painful. For me, the main problems are: 1. items are arranged in a specific and unchangable order, and there's no other way to navigate though them other than scrolling one by one; 2. Pokémon boxes are slow to rearrange, and once you close them it's very easy to forget what Pokémon you've put in there.

![]({{ '/assets/img/W4/01.JPG' | relative_url }})

![]({{ '/assets/img/W4/02.JPG' | relative_url }})

However, these problems are not exclusive to Pokémon games. Almost all modern games deal with in-game player items, therefore have a inventory management system. The form of these inventory systems are more or less the same, and have stayed this way for a long time. Most of them use grids, lists or carousels to display items, requiring the user to navigate using digital input devices on the game screen, and presents available actions once an item is in focus. This of course "works", but the problems mentioned before, namely the difficulty of navigating, searching and arranging items, and the lack of the sense of presense and the sense of possession of the items.

![](https://game-design-snacks.fandom.com/wiki/File:WoWScrnShot_020712_161153-1-.jpg)

*Image by [Razerlazer](https://game-design-snacks.fandom.com/wiki/User:Razerlazer) on Fandom. [Source](https://game-design-snacks.fandom.com/wiki/Poor_Inventory_Management)*

Therefore, I decide to take this opportunity to explore if I can find ways to enhance the cumbersome inventory management experience of video games by reimaging the process in the physical world.

### Inspirations & Literature Research

So the goal is to represent in-game items and player's interactions with them in the physical world. The first example of such blend is Nintendo's Amiibo. Basically they are NFC(RFID)-equipped figures of various in-game characters, which aside from decoration, can also be read by the NFC reader inside Nitendo consoles. This usually unlocks that specific character (or special items of that character), or is used to set the current controlling character in multiplayer party games.

![]({{ '/assets/img/W4/04.png' | relative_url }})

*[Source: Nintendo Official Website](https://www.nintendo.com/amiibo/line-up/)*

Amiibos have been around fot a few generations of console, but it never saw any widespread interest and adoption. I think this is because of 2 reasons. Firstly, Nintendo did not came up with a truly novel and irreplaceable use of Amiibos. No game feels significantly worse or unplayable without Amiibo, some will argue it's even clunkier with Amiibo in some situations (like each player have

05 to take turn tapping their Amiibo on the controller before controlling). Secondly, Amiibo are game-specific items. Some Amiibo get multiple compatible games (like the generic Mario, Kirby, Isabelle), but most of them can only be used in one single game (sometimes that game is not even that popular to begin with). Couple these limitations with a price tag of $15.99, it no surprise that Amiibo is now more of a die-hards' collectibles than a revolutionary game interaction system.

![]({{ '/assets/img/W4/05.png' | relative_url }})

*[Source: Nintendo Official Website](https://www.nintendo.com/amiibo/)*

Therefore, I think the Amiibo is a good place to start, especially it's use of RFID as a bridge between real world objects and in-game items, but we need a more general solution. To achieve this, ideally we need the RFID-object to be able to change on demand and represent different in-game items in different setting.

This reminds me of the E-ink shelf labels used that began appering in supermarkets in recent years. They not only replace printed paper and can update the content it displays, but also they have RFID built in. This enables digital inventory management and contactless setup for retailers. Better yet, thanks to E-ink display's mechanism, it doesn't need to be refreshed or backlit when displaying static image, virtually drawing no power once set up. The battery in those shelf tags are advertised to be lasting 10 years. So versatile, programmable and low power, this should be a great fit for being physical tokens of virtual items.

![]({{ '/assets/img/W4/06.png' | relative_url }})

*[Source: PRICER Official Website](https://www.pricer.com/products/devices/electronic-shelf-labels)*

Now that I have a direction, I did some research on current applications of physical or pseudo-physical implementations of fictional inventories, as well as using RFID technology for human-game interaction.

There's a good number of attemps of breaking from traditional menu or list interfaces by implementing physical properties to the items by game developers and researchers alike. I find the motivation falls into 2 categories: the first type is mainly seen in games for XR environments, and is aimed towards taking advantage of the virtual environment to make interaction more intuitive like Mußmann et al. (2021); the second type is more focused on emphasising item's properties: it's size, weight, placement, collisions, like this demo of a survival game inventory shared by game developer on Reddit (Disassembly_3D, 2021). This is a way to make players become more aware of the items they carry, or to limit their capacity to carry items for a more realistic experience.

Similarly, research are pretty thorough in terms of using RFID to create "Augmented Games". Although many seem to lean towards adding feedback or digital connections to for physical games. For example, using RFID tagged props to provide variations and rich feedback for children's chasing and catching games (Kinked et al., 2004), or using RFID tags as locators for a real-life Pac-man game (Rashid et al., 2006). Some other implementations are creating a digital twin or a companion of the physical game with RFID equipped objects, like augmenting a tabletop war game (Hinske & Langheinrich, 2007), or making a phone companion for playing cards that can display real-time date and give advices based on the current game (Flörkemeier & Mattern, 2006). One research did uses more generic props (geometric shapes with RFID) as input for children's educational games, to enable automated decision and suggestion for excercises based on previous input (Miglino et al., 2014).

Overall, I think that using RFID props to bring together the advantages of physical and digital interfaces is a widely accepted and explored direction to enhance the user experience. Therefore I decided to move forward with my idea.

### Ideation & Sketching

The design of the actual tag is pretty straightforward. Basically it's a programmable E-ink display with RFID, that can display the current item it's representing and can be read by the system as such item in the game.

The more complex part is how they can be integrated into the bigger system and how they can be interacted with. I decided to approach from thinking about "What's the affordances of a item", and see where the current implementation is lacking in terms of making these affordances correctly perceivable.

An in-game item should afford being:

* Acquired
* Possessed/Carried with player
* Used (but still reusable)
* Used and depleted
* Equipped
* Given away
* Lost/Disposed

I think the current digital system mainly falls short in two aspects:

* The affordances of acquiring and losing is weak. Physical objects is tangible, and takes up physical spaces whether or not you're paying attention. But in-game items often are merely an icon and a number, when you close your inventory it basically disappears. It's easy to lose track or forget about what you get and what you lose (like those little popups in adventure games telling you what you've picked up but I never really paid attention, or somehow I have more than 20 Charmander in Pokémon from different trainers through wonder trade and I have zero memory).
* The processes of possessing and using them are not enjoyable and intuitive. Like mentioned before, some games do not allow customization at all and force you to painfully scroll though a long list, while some try too hard and feel like doing chores. I think this is due to real-life items are starightforward to manipulate and allows for full user customization of the organization (think how people always seem to know where's everything in their messy room, because the placement of items is a direct result of the user actions, it gives a clearer memory). What's more, bringing up a inventory menu pauses the gameplay and breaks the immersion. In real life, you can reach for your pocket or search for something in you bag without losing the context of your current surroundings.

With these in mind, I started sketching how to use tags to better represent these in-game actions.

![]({{ '/assets/img/W4/07.jpeg' | relative_url }})

Through sketching I actually discovered a couple more use cases and interactions with these tags. Like physical trading of game items (again, Pokémon), and position-aware interactions between the items (inspired by Minecraft's crafting mechanism), which would require a antenna mat that can read the relative positions of multiple RFID tags.

So the final design includes 4 components:

* Tags. They can even very in size, maybe like a paper-sized one for displaying those long texts in puzzle-solving games and you can even make markups on it (I never wanted to read those on game screens).
* A base station. This handles the generating and recycling process of item tags. When an item is depleted the player pops the tag into the station, and when a new item is acquired the station updates the information and spits out the tag.
* A controller. This is for using and equipping items. A conventional controller can be added with slots and contact points to register the items. A tap means a single use, while sliding in a slot means equipping for prolonged usage (like weapons).
* An antenna mat. Not required, but like mentioned before this will allow for position-aware interactions with the items, or the implementation of limiting carriable items for realistic gameplay.

I think the best parts of this design are being able to stay aware of you inventory without needing to interrupt the gameplay, and the complete freedom of item placements. For example, the player can place most frequently used items around the hands in a ergonomic way, and for items that are deemed not needed for the moment, they can be piled to the side to clean up the clutter.

### Prototyping

The prototyping process is rather simple. Since the system requires programming to work, the prototype only serves to demonstrate how the interactions happen physically. I used cardboard to cut out the tags and created the controller (which kind of resembles the Nintendo Switch or the Wii U Gamepad), and used a cardboard box for the base station. I did not bother with the antenna mat since it will just be a plain piece of cardboard anyway.

![]({{ '/assets/img/W4/08.jpeg' | relative_url }})

![]({{ '/assets/img/W4/09.jpeg' | relative_url }})

![]({{ '/assets/img/W4/10.jpeg' | relative_url }})

![]({{ '/assets/img/W4/11.jpeg' | relative_url }})

*The whole setup*

![]({{ '/assets/img/W4/12.jpeg' | relative_url }})

*Slots and tap zone on the controller*

![]({{ '/assets/img/W4/13.jpeg' | relative_url }})

*The base station*

![]({{ '/assets/img/W4/14.jpeg' | relative_url }})

*Placement-aware interactions*

![]({{ '/assets/img/W4/15.jpeg' | relative_url }})

*Fully customizable placements of items*

### Conclusion & Reflects

I think approaching design from thinking about affordances is a good way to find out problems and rooms for improvement. It's a process of comparing the user's cognitive model of "what it should do" with its current perceivable affordances of "what it actually does" and find the discrepancies.

This week's readings about who we are designing for and what the users actually need is a good reminder to not jump from ideas to developing and conclusions. Literature research is necessary to know what have been explored and what lessons are learnt. I think this is also a form of "coming to the table", of getting to know about the current progress of the field you're getting in, instead of parachuting ideas with subjective perceptions.

### References

Disassembly_3D (2021, June). New physical inventory system! A refreshing new way of managing your stuff  instead of traditional flat 2d grid system. With custom physics so that  items can stack and remain stable and not explode in a mess. Reddit. https://www.reddit.com/r/IndieGaming/comments/o86ktl/new_physical_inventory_system_a_refreshing_new/

Flörkemeier, C., & Mattern, F. (2006, May). Smart playing cards–enhancing the gaming experience with RFID. In *Proc. 3rd Int. Workshop on Pervasive Gaming Applications–PerGames* (Vol. 2006, pp. 27-36).

Hinske, S., & Langheinrich, M. (2007). An RFID-based infrastructure  for automatically determining the position and orientation of game  objects in tabletop games. *Concepts and Technologies for Pervasive Games-A Reader for Pervasive Gaming Research*, *1*, 311-336.

Konkel, M., Leung, V., Ullmer, B., & Hu, C. (2004). Tagaboo: a  collaborative children’s game based upon wearable RFID technology. *Personal and Ubiquitous Computing*, *8*, 382-384.

Miglino, O., Di Ferdinando, A., Di Fuccio, R., Rega, A., & Ricci, C. (2014). Bridging digital and physical educational games using RFID/NFC  technologies. *Journal of e-Learning and Knowledge Society*, *10*(3).

Mußmann, M., Truman, S., & von Mammen, S. (2021, August). Game-Ready Inventory Systems for Virtual Reality. In *2021 IEEE Conference on Games (CoG)* (pp. 1-8). IEEE.

Rashid, O., Bamford, W., Coulton, P., Edwards, R., & Scheible, J.  (2006). PAC-LAN: mixed-reality gaming with RFID-enabled mobile phones. *Computers in Entertainment (CIE)*, *4*(4), 4-es.
