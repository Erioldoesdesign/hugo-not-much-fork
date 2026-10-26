---
title: "How developers understand package security information: UI for Attestations"
date: 2026-10-16
slug: "openssf-attestations"
description: "Portfolio page for OpenSSF/Securing software repos working group attestation style guide"
keywords: ["UI", "UX", "User Research", "OSS", "Security", "Usability Testing",]
draft: false
tags: ["UI", "UX", "User Research", "OSS", "Security", "Usability Testing", ]
summary: Working with the Linux Foundation's OpenSSF/Securing software repos working group on understanding attestations and developing an open source attestation style guide.
---

## Project Overview: Making sense of the complex world of open source package supply chain security with attestations, provenance and SBOMs

<br>

In December 2024 the [OpenSSF's Technical Advisory Council wrote](https://github.com/ossf/tac/issues/424) of the need for a UI and UX professional to understand and address how developers, software repositories and package registries present information and assertions around the package supply chain security information 'Attestations'. We worked with the [Securing Software Repositories Working Group](https://repos.openssf.org/) as our key Stakeholder alongside the staff members in the OpenSSF assigned to this work.

Attestations are a fairly new way of understanding a software packages supply chain security. Alongside Provenance information and Software Bill of Materials (SBOMs), Attestations are used to re-enforce legitimacy and indicate a 'safe' software package.

The [entire project can be found in this website](https://repos.openssf.org/attestations-style-guide)

The [Github repo is also available](https://github.com/ossf/wg-securing-software-repos/tree/main/docs/attestations-style-guide)

*"A software attestation is a trust mechanism that allows a verifier (i.e., a customer) to independently validate the integrity of something asserted by the provider (i.e., the vendor). For example, an attestation can be used to programmatically verify an application is built in a secure manner using uncompromised code. In other words, attestations make it easier for users of third party code to trust that code."*

 Definition via https://danacrane.medium.com/everything-developers-need-to-know-about-attestations-f5051ff3b007

 <br>

 ![Current visuals of package registry pages package information](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/attestions-1.png "Current visuals of package registry pages package information")

 *Above: Current visuals of package registry pages package information*

<br>

## Goals and Constraints 

<br>

This project asked of a 3 person team of designers, user researchers and documentation writers to better understand:

- Who is looking at software package supply chain security and what is the nature of their work/interest.
- Why package supply chain security is important to them (if at all) and what are the risks if they do not assess security well.
- What information to they find, understand and use to inform their assessment of the security of packages in their supply chain.
- What actions do different consumers of attestations make to assure themsevles of the security of their package supply chain (if any).

<br>

The initial request defined the deliverables here as a 'style guide' that can be applied specifcally to 3 pilot package registries ([npm](https://www.npmjs.com/), [RubyGems](https://rubygems.org/), [PyPi](https://pypi.org/)).

<br>

The implementation stage would be done by a independant implementation party post design, user research and documentation delivery, therefore we endevoured to make as much of our process, conversation and outputs open source and transparent as well as prioritising clear information, drawn from user research as to why certain design choices were made.

<br>

 ![Early mood boarding with stakeholders revealed similar information comprehension patterns such as food nutrition labels](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/attestions-2.png "Early mood boarding with stakeholders revealed similar information comprehension patterns such as food nutrition labels")

 *Above: Early mood boarding with stakeholders revealed similar information comprehension patterns such as food nutrition labels*

 <br>

### User goals

<br>

We isolated [3 different personas](https://github.com/ossf/wg-securing-software-repos/issues/70) for 1 round of initial user research and a subsequent round of usability testing for prototype solutions.

- Users needed to know the critical security information before making a risky package choice.
- Users typically did not want to spend long amounts of time parsing complex documentation and would often rather rely on a combination of [social proof](https://en.wikipedia.org/wiki/Social_proof) and the [web of trust](https://en.wikipedia.org/wiki/Web_of_trust) to make decisions. Attestation information neede to be minimal, clear, have pathways to more information that progressively enhanced in complexity as the user chose to follow information.
- Not all users have the highest threat models for package supply chain security. Those that did typically worked in finance software, software deployed on hard to reach hardware (e.g. space tech, deep ocean tech) and people that worked with privacy/security tools and high amounts of PII data on users.

<br>

 ![Personas profiles](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/attestions-3.png "Personas profiles")

*Above: Personas profiles*

 <br>

### Organisation goals

<br>

The style guide's intention was to be universally applicable as to be useful across any website or ecosystem's branding style and **prioritise the understanding of attestations within the wider context of package supply chain security**.

These goals extended into what makes for good UX layout, positioning of critical information, unique symbols for key information and what additional information/documentation is needed, by what personas at what points in their process.

<br>

## Methods and Process

<br>

This was a 12 week project where timelines were tight and turn-around from user research to UI treatments and rationale was critical. As the main designer working on this project (with support from a documentation writer and technical support) I was responsible for the project from start to final delivery. 

The rough outline of the project was:

1. Stakeholder engagement and desk research
2. Concept understanding and preparation of user research protocols, documents and recruitment
3. Conducting user research, synthesising research
4. Developing testable prototypes
5. Usability testing of prototypes
6. Final UI style guide edits, complilation of style guide and documentation writing

It is worth noting that due to the nature of this work the recruitment and conducting of user research was planned and conducted with the highest security protocols possible.

All the tools we used preferenced open source tools where possible.

<br>

 ![Synthesis on virtual stickies from the user research process](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/attestions-4.png "Synthesis on virtual stickies from the user research process")

 *Above: Synthesis on virtual stickies from the user research process*

 <br>


## Impact and Outcomes

<br>

The outcomes and impact were not only to the client but to the wider OSS ecosystem. In the broadest sense, we brought critical user behaviour insight to the people working on the security of open source software. These insights still impact and inform the conversations about what is shown to users regarding package security.

<br>

![Development of uniue symbols for attestations in relation to packages](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/attestions-5.png "Development of uniue symbols for attestations in relation to packages")

 *Above: Development of uniue symbols for attestations in relation to packages*

<br>

On a more granular level there were several discoveries. One of the most prominent was that the words you choose for information content is vital in a security context and can be easily assumed or misunderstood. The word choice *'build confirmed'* and any use of *'verified'* suggested to users that everythings fine - and many users in usertesting stopped reading the details and trusted the words. 

Confirmed and Verified are not 100% accurate in attestations because *'an authority'* makes a claim of safety, but it cannot take liability if it ends up not being true.

We also learned and passed on information:
1. All personas factor in social proof (who is the maintainer listed, are they well known, is the registry sitereputable) as a key trust factor for a packages safety and source. 
2. Only the Seurity Architect and some Pragmatic Developers investigate attestations further such as setting up a sandbox test environment etc.
3. People working on more risky systems or hard to reach systems have more incentive to find out if a package is safe and to be trusted a.g. banking/finance/crypto wallets or hardware systems in human-hostile locations e.g. space, deserts, underwater etc.
4. All personas are fine with critical information being repeated when it's important as the rationale is there are less chances to 'miss' important details.
5. All processes for checking build, key signing, hashes etc. took similar steps but in different orders. 
6. People trust that there will be accurate and human understandable documentation somewhere.
7. Quick visual references in sidebars like badges, symbols, icons etc. combined with dedicated security pages were prefered. Not every visit is a high security scrutiny visit.

<br>

 ![Visuals of the icons and the explainations of what users understand of them when used](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/attestions-7.png "Visuals of the icons and the explainations of what users understand of them when used")

*Above: Visuals of the icons and the explainations of what users understand of them when used*

 <br>

This project didn't particularly invent new revolutionary design processes or UI ideas. But instead moved design practices into an aspect of FLOSS that is routinely overlooked and under-resourced from a usability and design perspective.

<br>

![Final UI style guide treatments](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/attestions-6.png "Final UI style guide treatments")

*Above: Final UI style guide treatments*

<br>

We also took an extra effort to communicate that this work did not contain translation and localistion efforts.

<br>

 ![Some examples of the differences in UI when translated/localised](https://raw.githubusercontent.com/Erioldoesdesign/erioldoesdesign.github.io/master/images/attestions-8.png "Some examples of the differences in UI when translated/localised")

*Above: Some examples of the differences in UI when translated/localised*

<br>

## Watch a presentation of this work from FOSDEM 2026

[Watch the embedded video over on the FOSDEM Website](https://video.fosdem.org/2026/ub4132/HCQRVT-designing_attestations_ui_the_security_and_safety_of_oss_package_supply_chain.av1.webm)

<br>