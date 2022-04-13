## Agenda
[1. Update on budget at CIFFC - thanks Rob Kruus](#1-update-on-budget-at-ciffc---thanks-rob-kruus)

[2. Presentation in Draft Form](#2-presentation-in-draft-form)

[3. BP3 Rewrite](#3-bp3-rewrite)

[4. PSaaS In House](#4-psaas-in-house)

[5. Community Changes Feedback](#5-community-changes-feedback)

[6. Update from Rob on Video (FireCast)](#6-update-from-rob-on-video-firecast)

[7. Renewed Interest from Lux](#7-renewed-interest-from-lux)

[8. Additional Topic - Brett, Franco, Rob, Jordan - Code Repos Across Canada](#8-additional-topic---brett-franco-rob-jordan---code-repos-across-canada)

### 1. Update on budget at CIFFC - thanks Rob Kruus
_Neal_ - If there is funding given to the project please let me know. Some of that funding doesn't go through CIFFC. Franco I'll need to chat with you later. I want to keep track of this data for better reporting.

_Franco_ - I have some ideas on this and I have a potentially better way.

### 2. Presentation in Draft Form

[Prometheus Slides Video]({../Video/PSaaS_Meeting_Prometheus.mp4} "Prometheus Slides Video")

_Neal_ - Intent of this is to deliver to canada wildfire / ciffc. Speak about End of life prometheus, psaas and what they can expect moving forward. There is no urgency for this as there is a waiting list. NZ wants a talk too, we will be just covering how we are using PSaaS. 

Big topics:

1) Why End of Life
2) Why Modernize
3) Ideals and Values

Brief history of Prometheus within that the business case for modernizing and developing a more formalized national development team around it. Underlying systems 30/40 years old. Prometheus is also very old, 2002 first publication, 2022 end of life. Takling about the start of Prometheus on Win 98 using COM from 1993. This new program is a fundamental shift and total rewrite.

Toolbox - Some of the values, moving towards open source, developing a community and a team of custodians and developers. Going through the process of ensuring extensibility and slow growth. Lots of questions on pace and updates and we want to really ruminate on those things and describe how we are moving forward with those thoughts in mind. 

Spend some time on the contribution towards modernization and define how it is a public/private/international funding effort. Nearly 600k for a fundamental rewrite and making PSaaS a reality.

End of Life - What is it? Why? The whole progression speaks to that. 

Stuck on how to show PSaaS off. How do we show off PSaaS and make it appealing?

2 Questions I foresee:
1) How do I do it now? Where is my UI?
2) How do I automate it in my organization?

Got lots from the FireCast demonstration, FireHawk, etc. But yea, big sticking point it how to show it off effectively.

Few FBANs that are trained specialists to use models like this. This tool can allow us to model multiple fires with time constraints.

_Franco_ - Present on the EOL of Prom and the transition from Prom to PSaaS, you cannot be thinking about day one of EOL as EOL is a year long. Prom will continue to exist until it is no longer supported by Windows. PSaaS does not work the way Prometheus does so its not worth mentioning. This is a break from the current paradigm. 2 part presentation, 1) Prom, why we are going to EOL, 2) PSaaS, no longer mentioning Prom. Nothing you can really show anyone as its an API and a technical diagram. 

_Brett_ - The longer this takes the more solid an understanding I'll have of the services the CFS intends to provide.

_Neal_ - Emerging research at Canada Wildfire, validating fire growth models at a seasonal scale.



### 3. BP3 Rewrite
_Brad_ - Status? Generally what is going on?

_Brett_ - Contract awarded, programming has begun, targetting fully live for next year.

_From Chris_ - Apex RMS to develop this, and that we already have functional prototype built and anticipate completion (i.e. deployment) before end of the calendar year

### 4. PSaaS In House (CFS)
_Brett_ - Can I use this in house for output generation?

_Neal + Franco_ - No issue here.

_Franco_ - V7?

_Brett_ - Yes, I'll need some help on that.

### 5. Community Changes Feedback
_Franco_ - Feedback on changes to the community?

_Jordan_ - Updating the vc name.

_Brett_ - Happy to see updates, things have been much more functional.

_Brad_ - We have suggestions but need to know how to put those forward.

_Franco_ - We can adjust those and we have utilities to achieve that in the website.

_Neal_ - Much better, very nice tool now and a great refresh to the site. Website puts PSaaS out there now and we need to discuss what we are going to call it. We don't necessarily need a new name but worth discussion. Thanks for the recovery on the Intel compiler. No additional suggestions/improvements at this time.

_Franco_ - Absolute no go on PSaaS I will begin making a naming suggestion system for the team initially and expand beyond that.

_Neal_ - A lot of the feedback mechanisms have been much nicer.

### 6. Update from Rob on Video (FireCast)
_Franco_ - Have things been upticking?

_Rob_ - I have been getting some interest on FireCast which has been encouraging, I did get a comment on the fact my presentation skills need some work. Seeing that the weather module is generating some excitement. Seems to be that PSaaS is changing how we are thinking about fire modelling in general.

### 7. Renewed Interest from Lux
_Franco_ - This group needs to decide how we are going to officially deal with corporate interest. There are currently 2 companies very interested. We need to be on the same page on how to manage expectations. Do you, Neal, have anything in mind on how we are going to deal with these processes?

_Neal_ - I have thought about it, I don't have THE answer but I have some thoughts. We can chat more after the talk otherwise I have 30 minutes later this afternoon.Let's deal with this today though. Now or postpone?

_Franco_ - Fine to postpone, if anyone else has thoughts happy to hear it.

_Neal_ - Teaser - One of the things we've stated in the standardized response for corporate interest is, you can gain early access but you need to be a part of the dev team. To become a part of the dev team you need to put forward what you can give to the team and give us a proposal for us to go over. For me its holding that up stronger and defining what we actually require so this team can determine if we want help. 

_Jordan_ - Timeline for publication?

_Neal_ - Towards the end of the calendar year.

_Jordan_ - List of what we need?

_Neal_ - Not yet no. We request a proposal but we don't have a list of what we need.

_Brett_ - Not if it jeopardizes timelines.

_Neal_ - It should speed us up.

_Franco_ - I'm good with the idea of waiting until we go public. However we have folks that we've told there is a way to get in but haven't given them the ability to do so. They have been using Prometheus and would like to use PSaaS. 

_Brett_ - Big opportunity for QA/QC

_Neal_ - Agreed, this could also bring us into the unit test area and to deliberatly ask for this kind of engagement from a stakeholder like this. We would also be able to request that they operate as a testing suite.

_Franco_ - They could write unit tests for us too.

_Brad_ - This is what Forsite thought that they could offer. This is where their heads are at though. 

_Neal_ - This is not intended to be a one off, this group would become the testing team and every release we would want them spooling this up.

_Brad_ - Randy is looking to be a part of the team.

_Jordan_ - If small groups why not all?

_Franco_ - Well we just don't currently have the capacity to support the whole world just yet. Currently a little hesitant to go wide open just because a number of folks are already fully committed to this project unofficially.

_Jordan_ - Currently available to assist with whatever you may need.

_Franco_ - Sounds good, there was no assumption of time committment for staffers. Happy to discuss further offline.

### 8. Additional Topic - Brett, Franco, Rob, Jordan - Code Repos Across Canada

