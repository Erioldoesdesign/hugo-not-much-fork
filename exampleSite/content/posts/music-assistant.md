---
title: "Music listening behaviour in Smart Homes. Improving the smart speaker music management experience"
date: 2026-10-20
slug: "music-assistant"
description: "Portfolio page for Music Assistant"
keywords: ["UI", "UX", "User Research", "IoT"]
draft: false
tags: ["UI", "UX", "User Research", "IoT"]
summary: Improving controls for a music player that is connect to local smart home devices and speakers where we prioritise management of audio across a home's smart ecosystem.
---

## Project Overview: Not *just* another tool for listening to music. Empowering users with smart home speakers to automate music behaviours

<br>

[Music Assistant](https://www.music-assistant.io/) is one of [Home Assistant's](https://www.home-assistant.io/) key maintained projects. Fundementally it allows users to listen to music via their existing streaming services as well as local files, internat radio and other sources. The very unique aspects are the ability to manage and control smart audio players from the Music Assistant interface as well as set up automations in your smart home that play audio.

Music Assistant's interface, like many of Home Assistant's interfaces and tools, were primarily created by developers and OSS contributors that have some knowledge of UX and Ui best practices that can apply to their own use cases and other power users use cases but the UX and UI was not focused towards enabling less familiar, technical and interested to operate the features with comfort.

This project describes some of the iterative UX and UI improvements to Music Assistant over my time working at The Open Home Foundation and less of a 'contained' project. I'll be diving into a few significant releases over 2025 to 2026.

<br>

![Early ideas on how to improve the page that shows what audio is playing right now. This also shows a snippet of the detailed user feedback that I keep stored in the design files for quick reference](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/musicassistant-1.png "Early ideas on how to improve the page that shows what audio is playing right now. This also shows a snippet of the detailed user feedback that I keep stored in the design files for quick reference")

*Above: Early ideas on how to improve the page that shows what audio is playing right now. This also shows a snippet of the detailed user feedback that I keep stored in the design files for quick reference*

<br>

## Goals and Constraints 

<br>

Music Assistant, like many tools and technology that starts out as a ['scratch your own itch' OSS](https://code-maven.com/osdc/osdc-collab-dev/scratch-your-own-itch.html) project. It was created to be used by the creators and thos emost like the creators. But, like with all software, as soon as someone other than you uses it you have a variant user type. No 2 users will use a tool in exactly the same way, under the same motivaions and for the same purpose (or this is statistically very unlikely!). So Music Assistant struggles to understand who it serves and how prominently it serves who. 

Music Assistant is leaning into a 'Smart Home Enthusiast' user. One that has time, abilitya nd interested in 'tinkering' around with settings, features, set-up and updating. As such many of the feature improvements focus on these power users while still hoping that non-power users find their own way. My personal goal as a usability and human centered designer was to improve new user accessibility and usability with every design iteration.

![Example of a stakeholder meeting outputs where I gathered all perspectives and constraints](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/musicassistant-drawer-1.png "Example of a stakeholder meeting outputs where I gathered all perspectives and constraints")

*Above: Example of a stakeholder meeting outputs where I gathered all perspectives and constraints*

<br>

### User goals

<br>

- Enjoy listening to music from across streaming services, local files and audio types.
- For multiple people in a smart home to be able to listen to different audio across different smart devices/speakers.
- For the admin of the Music Assistant system to have a level of access and control to destructive actions like how loud audio can be played, in certain locations under certain circumstances e.g. late at night.
- To Understand better what the playable audio situation is in their own smart home and have the ability and process avaialble to automate what they want.

<br>

### Organisation goals

<br>

- Release quickly, understandable and community approved features and improvements.
- Uderstandable UX and UI that make critical actions more simple, understandable and enjoyable to use.
- For users to discover and use as many features, settings and configurable options as they have access to and know about.
- More users adopt Music Assistant as a preferred music listening tools while a user in in their smart home.
- To appeal to music and audio geeks by offering features and settings that prioritise audio quality and protocol playing mode as a clear option.

<br>

## Methods and Process

<br>

The typical process for Music Assistant was:

1. A Design, development or a community user raises an issue, feature request or an enhancement topic. These should connect to the larger organisational goals for the year to have focused resource on them and be wanted by the community of users.
2. Scoping and cinfirmation of UX and User Research exploration. This is where was assess whether the work can be done primarily by development with design support, advice and quick involvement or by a more detailed design exploration process. This typically happened when a critical feature was being discussed and the stakeholders had very strong differing evidence or opnions about direction.
3. Deeper design investigated design solutions, validated them with stakeholders and community, sometimes with structured usability testing or research conversations. If user validation was not possible we looked to the standards set by similar technologies.
4. Design exploration continues until user community and stakeholder approval was gained and all design acceptance criteria were met.
5. A 'good enough' design went over to development where if adaptions were made, we re-convened as a team and community to address the adaptions that often came from discoveries in implementation.

<br>

## Impact and Outcomes

<br>

The two features that produced the most impactful outcomes were **improving the don't stop the music** feature and improving the **player drawer speaker management** experience.

Don't stop the music was a feature that had a function twin. There were two features that produced an incredibly similar output of continuous music being played. Initial conversations explored the differences functionally and from a user's point of view of these features. We discovered they could be easily merged into a new feature called **'Autoplay'**. This name matched other music streaming platforms and we looked at these to aggregate the UI and UX implementation.

<br>

![Sketches of don't stop the music improvements](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/musicassistant-autoplay-1.png "Sketches of don't stop the music improvements")

*Above: Sketches of don't stop the music improvements*

<br>

![The mental map of 'don't stop the music' from a user pov](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/musicassistant-autoplay-2.png "The mental map of 'don't stop the music' from a user pov")

*Above: The mental map of 'don't stop the music' from a user pov*

<br>

A first simple phase focused on the visual design, from icons, colours and animations and progress to where this feature should live. After 3 rounds of design we settled on the player queue page since this was where a user views what music tracks are populating the autoplay queue and under what rules.

<br>

![Early visual design ideas for autoplay](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/musicassistant-autoplay-3.png "Early visual design ideas for autoplay")

*Above: Early visual design ideas for autoplay*

<br>

![Implementation close UX/UI design ideas for autoplay](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/musicassistant-autoplay-4.png "Implementation close UX/UI design ideas for autoplay")

*Above: Implementation close UX/UI design ideas for autoplay*

<br>

There was pushback from the development team on the positioning of button functions, how UI should appear when it's 'running' and also positioning a functional feature in the music track play queue. Presenting the design rationale for these choices took extensive research and conversation about the usability heuristic [recognition and recall in user interfaces](https://www.nngroup.com/articles/recognition-and-recall/) and that functions should be close in proximity to function they effect.

<br>

The second feature implementation is improving finding smart speakers, understanding the state of smart speakers (are they playing audio? How loud? Is speaker 1 grouped with speaker 2? etc.)

The main UX issue here was the way of viewing, editing, grouping, deleting, renaming smart speakers was all done in a single minimal slide out 'UI drawer'. This drawer UI offered high amounts of cognitive load in a small space (on larger screen sizes at least) with little opportunity to pace the cognitive load of that task-heavy section of the Interface.

<br>

![Early visual design ideas for the individual speaker section within the drawer.](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/musicassistant-drawer-2.png "Early visual design ideas for the individual speaker section within the drawer.")

*Above: Early visual design ideas for the individual speaker section within the drawer.*

<br>

Much of the early design work was focused on isolating the essential operations that users want to do and how they might be done in combnation of sequences and what we wanted to assert as the 'best' opinionated sequece of function.

<br>

![Finding layouts that optimise available screen size and don't default to the smallest mobile view if more space is available for users](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/musicassistant-drawer-3.png "Finding layouts that optimise available screen size and don't default to the smallest mobile view if more space is available for users")

*Above: Finding layouts that optimise available screen size and don't default to the smallest mobile view if more space is available for users*

<br>

I worked on moving functions to other nearby UI, like the 'now playing bar' along the bottom of the screen and seeing if we can have several menus that have a single main function and sub functions that connect to the primary function. This mean't eventually we created three sections on the right hand of the now player bar as a kind of 'menu' that allowed for 3 primary actions of volume control, speaker grouping and speaker overview with play/pause controls and focus change.

<br>

![Clear sectioning of the speaker overview UI where we cwanted to ensure a clear hierarchy of playing, idle and sleeping smart speakers.](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/musicassistant-drawer-4.png "Clear sectioning of the speaker overview UI where we cwanted to ensure a clear hierarchy of playing, idle and sleeping smart speakers.")

*Above: Clear sectioning of the speaker overview UI where we cwanted to ensure a clear hierarchy of playing, idle and sleeping smart speakers.*

<br>

<br>

![A snapshot of the three right hand menu options on the play now bar with contextual to the smart speaker icons to enable quick user recognition.](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/musicassistant-drawer-5.png "A snapshot of the three right hand menu options on the play now bar with contextual to the smart speaker icons to enable quick user recognition")

*Above: A snapshot of the three right hand menu options on the play now bar with contextual to the smart speaker icons to enable quick user recognition.*

<br>

## Watch the Livestream of a Music Assistant release party where UI updates were made

<br>

{{< youtube J0W_PgDxpzA >}}

<br>