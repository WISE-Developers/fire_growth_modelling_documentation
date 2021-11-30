# Agenda

Attendees: Brett, Franco, Rob, Mac, Brad, Peter, Rob

## 1. New Zealand Manual Mode

*Franco*: Rob bring people up to speed on this.

*Rob*: Okay, Wayne has been working on running PSaaS in an automated fashion but due to false positives/negatives, they would like to run PSaaS manually in the same environment. They are trying to move away from Veronica running Prometheus. They are wanting to get her to a point of being able to run PSaaS without a GUI.

*Franco*: Correct me if I'm wrong but they aren't using PSaaS as it was intended, they are not using Manager. It sounds like they need to use manager to me.

*Rob*: That's why I'm not sure what they are on about as Wayne doesn't want a GUI while Veronica does.

*Franco*: So why not use Prometheus?

*Rob*: Agreed, they have automatically generated the inputs, but beyond that I'm not sure how we can help them.

*Franco & Brett*: This could be an opportunity to use the abstraction API.

*Franco*: So why do they need the GUI? Are they watching something?

*Rob*: Some people still want a GUI.

*Franco*: Okay, but I still need to understand why they need the GUI and for what. The plan is to put a head back on it eventually, we are just ironing out the engine right now.

- [ ] Rob talking to Veronica
## 2. Lux Meeting

*Franco*: How are we feeling about Lux?

*Brad*: Chart out more how we can work together. Determine how the projects are intertwined. 

*Franco*: Looks like we have an opportunity to communication, who would like to see a presentation by lux? Anyone feel there is a reason to not have a presentation from them.

~Silence~ 

*Franco*: I will propose a meeting to them to describe to us what they are doing. Tentative plan moving forward is that they will present at the next meeting.

## 3. Abstraction API

We now have a project in the repository for the abstraction API. 

We are looking to frame out the what so we can later define the how. We now have a repository to define the skeleton for this API.

A number of words are getting tossed around, abstraction, integration, etc. We are also seeing a number of GUIs wanting to get developed. We want this to all utilize the abstraction API to ensure a standard that will remain unchanged while everything underneath may be changing. This abstraction API will be a part of a broader SDK. 

The goal is to have a frame for what this will do before it is ever done.

- [ ] Brett continuing documentation generation
## 4. KML PCOM - Engage Rob for Pandora issue

*Peter*: I have a Pandora user who wanted an upgrade to Pandora, so I thought I would at the same time use the latest greatest. This would put me in a position to be ready for the EOL Prometheus. Importing a KML ignition point did not work, it appears something has changed from 2 years ago to now. Rob would either answer my problem or fix my code. Where do I go for support on this now? 

*Franco*: I am going to try and answer this to unclutter some things. First thing to consider is the expectation. The expectation being that COM can read KML, why is that the expectation, has it done it in the past. Just file a bug.

*Peter*: Alright, I can do that, where do I go now that it's been cleaned up?

*Franco*: Peter has a PCOM issue, who is the stick handler?

*Neal*: Brett

*Franco*: We no longer have a staging area, we now have 2 areas we can make a bug. This would be a PSaaS with a sub-component PCOM issue. If there is an issue now just file it and it will get sorted out.

*Peter*: Alright, thank you.

- [ ] Peter making a bug

## 5. Issue 1180 - Needs testing, assigned to Brett

[#1180](https://ppm.redapp.org/issues/1180)

*Mac*: We have gotten this sorted out.

## 6. New Prometheus Build for Feedback

*Rob*: We got 00 out but have a 01 already and I'm not sure how that happened.

*Franco*: Let's pick this up after the meeting.

*Rob*: The other part of this is that there are 2 2021.04.00's there is a V6, V7 win and V7 linux. Although the v6 04.00 is a rebuild of 2021.03.00 V7 did have changes. Point of confusion that there are multiple versions of 00 that are moving at different rates.

## 7. CIFFC Updates

*Neal*: I met with Maria Sharpe and Emanuel and Van. There are ongoing changes at CIFFC and I am not sitting on any committees. Emanuel is taking over the IMIT portfolio. We had a discussion about the toolbox, and Emanuel thought it existed. Our team is holding up the tenets but isn't actually integrated in the toolbox. CIFFC has desire to build parts of the toolbox. In order to get this moving leadership should be a part of the IMIT group. Identify low hanging fruit each year. One of the things I brought forward was licensing and ownership. This group could provide us some support with how to provide our tool as an open source platform. This group may generate a framework around us that could be of benefit. One other thing, we did talk about the idea of an external foundation incase things don't work out with CIFFC. From Van:
 >It sounds like a good idea, but be careful as this is constructing another agency, but we should be able to do it at CIFFC.

This is a good sign for us as this support ensures that CIFFC wants to manage the tool without the generation of another organization.
