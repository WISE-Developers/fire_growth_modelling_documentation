<!-- vscode-markdown-toc -->
# Agenda
1. [Draft log4j document](#Draftlog4jdocument)
2. [Small update on Phase 1 Open Source Project](#SmallupdateonPhase1OpenSourceProject)
3. [Firehawk Presentation CIFFC to Youtube](#FirehawkPresentationCIFFCtoYoutube)
4. [Update on Business Case Regarding Funding Alberta - CIFFC](#UpdateonBusinessCaseRegardingFundingAlberta-CIFFC)
5. [Showcase the HSS Weather Service Primer](#ShowcasetheHSSWeatherServicePrimer)
6. [Robert J working with Wx service and modelling framework for CWFIF](#RobertJworkingwithWxserviceandmodellingframeworkforCWFIF)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->

##  1. <a name='Draftlog4jdocument'></a>Draft log4j document

_Franco_ - Short synopsis: There is a vulnerability in our software. This has generated significant IT panic due to threats of removal of RedApp and Prometheus. I've been taking a number of calls and emails, the one that tipped me over was from CIFFC saying "you have AB money, fix it". Rather than responding to that individual email, I have drafted a notice for all agencies that I'd like to vet through the group first. I'd like to read that document to you now.

Draft doc is as follows:
> PSaaS Project Update - log4j Vulnerability
>
> This document will serve to update you of the current understanding of the Log4J Vulnerability threat and its relationship to the tools which The PSaaS Team is responsible for.
>
> Log4j Security vulnerability
>
> Microsoft and the U.S. Department of Homeland Security and others -- warn that threat actors are working on the ransomware and cybersecurity attacks based on Log4j. So, this may be the "lull before the storm." And it is our “Red Flag” to act.
>
> Apache log4j is one of the most widely used Java logging libraries. The vulnerability assigned as CVE-2021-44228 (along with CVE-2021-45046) is easily exploitable and allows attackers to run their code on your server.
>
> Apache Log4j2 2.0-beta9 through 2.15.0 (excluding security releases 2.12.2, 2.12.3, and 2.3.1) are the versions of concern and are vulnerable to this exploit.
>
> Analysis
>
> Sadly, there is no funding to perform a deep analysis to find a suspected vulnerability. Despite this lack of funding, this week, members of the PSaaS team voluntarily began assessing the vulnerability on their own time and tested our code with the best log4j scanners available to us.  The sheer number of panic emails and calls and the many reports of IT departments finding vulnerabilities in or near our software drove us to act without funding.
>
> Findings
>
> Our unofficial findings are summarized as the following:
>
> The current versions (Available for download from their respective websites listed below) of REDapp & Prometheus do not use log4j at all, they do not represent a threat. If your IT department, detects log4j in your REDapp or Prometheus install, it is likely from old libraries hanging around, we suggest you uninstall the tool, clean the computer, and reinstall the tool and retest, we are confident that Both REDapp and Prometheus are safe to continue using for this fire season.
>
> The current version of PSaaS (Both 6.x brand and the 7.x branch) Both use a vulnerable version of Log4j. At this time, all stakeholders that are using PSaaS are aware of this and know that we are actively working on implementing a short term workaround (A script to secure the existing installation) and a long term fix to eliminate the dependancy on the vulnerable version. We expect the “Work around” to be available next week and the long term fix soon after.
>
> PSaaS Team Tool Status
>
> REDapp Vxxxx - SAFE - log4j is not used.
> Prometheus Vxxx - SAFE - log4j is not used.
> PSaaS V6.x - VULNERABLE - uses log4j 1.x and 2.x
> PSaaS V7.x - VULNERABLE - uses log4j 1.x and 2.x
> 
> If you have any further questions you can contact us at foobar@foo.com

_Neal_ - What about the pending releases of Prometheus and RedApp?

_Rob_ - Just PSaaS Manager specifically. We are not using the other libraries directly but we may be using them indirectly.

_Neal_ - Can better define PSaaS to ensure agencies know what it is. We need to inform the agencies that it is a development product.

_Franco_ - Trying to avoid offering any opinion and just stating the facts.

_Franco_ - since the issue was raised with CIFFC, our management team wants to assist with this issue and Manny has generated the documents. He has funding to sovle our issues.
##  2. <a name='SmallupdateonPhase1OpenSourceProject'></a>Small update on Phase 1 Open Source Project

_Franco_ - Rob is readying all the inital redapp source code for open sourcing. This is a substatial step towards our dream of automated builds. This will require some time for the developers to work with the CI/CD build pipeline. Its important as it establishes a new workflow for HSS to apply to Phase 2, which is the remainder of the PSaaS source code. The update is that the money is now moving to CIFFC, they have invoiced us and CIFFC now has the money. Not sure if the money is actually with CIFFC, but it has been paid. This is a smaller contract, 8000$, but it is a key step towards our goals.

_Neal_ - One question - In preparing this we would need to finalize the license decision right?

_Franco_ - No, not A license, this will end up being multiple licenses. Some of the libraries are more complicated and require a more restrictive license and we will have an array of licenses for different libraries. At this time 3 licenses, one for math, one for time and one for RedApp proper.

_Neal_ - No need to rehash the license discussion, but BC has had a number of discussions using redapp code, instead they are using the CFFDRSR code but it is GPL and that is a roadblock.
##  3. <a name='FirehawkPresentationCIFFCtoYoutube'></a>Firehawk Presentation CIFFC to Youtube

_Brett_ - Jon Boucher would like to know if we are okay with CIFFC publishing the Firehawk presentation on YouTube. I have some personal feelings on this, but I would like to hear from the group prior to tainting the water.

_Brad_ - It's already up.

_Neal_ - Need for our team to do a follow up through CIFFC.

_Franco_ - It would be good to request an addendum with any issues we've seen. 

_Jordan_ - Issues with licensing?

_Franco and Brett_ - Yup, working through it with Jon.
##  4. <a name='UpdateonBusinessCaseRegardingFundingAlberta-CIFFC'></a>Update on Business Case Regarding Funding Alberta - CIFFC

_Liz_ - Submitted to business lead on the correct forms. Fin/Admin has requested a grant developement request to allow a proper ask for funding. All things are submitted and going through the process. Optimistic that it will be approved, no timelines at this time.

_Jordan_ - Has anyone asked about fundign from other agencies?

_Neal_ - No, because we wanted to have some centralized ask rather than an agency asking.
##  5. <a name='ShowcasetheHSSWeatherServicePrimer'></a>Showcase the HSS Weather Service Primer

_Rob_ - Self initiated work (4casts.ca), data is presented in many ways and many projection. For Prometheus all we need are weather streams. The Canadian and US models all incorporated. Standard data frame, this service caches all this data. Presenting a basic API for fire weather and fire modelling. Trackign stats so we can see if we're having issue with the data feed. Looking to do in memory caching to get away from GRIB. This visualizer is really just to help people get used to the API.

_Franco_ - My experience, this is an openAPI 3.0 application. Works like all openAPI services, in that respect its great. Had it running on my infrastructure where its doing all the downloading. Doesn't use as much bandwidth as I had expected. Stats tab let me know if it was doing its job without going under the hood. Comparable to the initial interface to SpotWx but it's now providing so much more weather than SpotWx. I don't really think this puts Garth in jeopardy. People using SpotWx for gathering weather, this would replace SpotWx. Ideally we would have multiple agencies with this system up to ensure guaranteed uptime.

Will require a deeper dive with Jordan, Robert and Rob

##  6. <a name='RobertJworkingwithWxserviceandmodellingframeworkforCWFIF'></a>Robert J working with Wx service and modelling framework for CWFIF

_Robert_ - Working on gathering and unpacking the data. Good to look into other ways of acquiring these data streams in an effort to have multiple methods to achieve the same goal. 

_Franco_ - Meet with Rob, Robert, Jordan, Brett and myself to talk about collaboration. Make it so we are all working on it.

_Brett_ - Can I add Alex to that to ensure FireHawk is a part of it too?

_Franco_ - Yup.

_Neal_ - Good to see this becoming a national initiative. How do we tell the nation about HSS WX?

_Brett_ - Could be a good topic for a CIFFC National Conversation.