# Agenda

Attendees:

Rob Kruus
Brad Armitage
Brett Moore
Franco Nogarin
Neal McLoughlin
Rob Bryce
Robert Jagodzinski

## 0. Round table

_Brett_ - Uninstall seems to hang the installer which is weird.

_Neal_ - Moving the family, been very busy, haven't had time to get situated so I have a backlog. News for this team, abstract was accepted. Presentation will be less technical and more a story of the experience managing a national modelling project. What it has taken to develop the team and the struggles and successes we've had. 

_Rob_ - Accepted at the conference for a 20 minute talk on FireCast and what was learned over the season.

_Robert_ - Updates on deploying PSaaS on Azure and Kubernetes. Tasked with getting this stuff up on the CWFIF on Azure. I do have PSaaS returning the version number and I've tried creating an ingres but there may be some other permissions needed for more information. I have set up the MQTT broker but I haven't really had a chance to use PSaaS to know how to pull things out.

_Franco_ - To Robert. Curious, are you attempting to do this as a service oriented architecture where each component is its own or just one container? 
_Robert_ - One containter. 
_Franco_ - Looking to be close to the time where we deploy the dip modeller at the CFS so we may be able to just move that across. Perhaps we try deploying that? 
[Action] - Meeting at 1530.

## 1. What's Happened

From #88 what is the backlog? Initially it was the proposal, we chose item 2. Brett is going to chat with Rob more on where things are going. Additional discussions on the depth of our backward compatibility.

## 2. What's in flight

_Rob_ - From #62. Do not have automated builds need to fix and issue with tests on wtime, the other is the installer. 1 done, 1 ready for review.

From #78. One of the 2 installer items, need to review travis' work and move it to another set in zenhub.

From #60. 


## 3. Testing/Review

#61 - 

#91 - Done some testing with sunset, sunrise, seems to be working well.

May I deploy for testing or do I need to do anything prior to testing? 
_Franco_ - Yup test it as it stands right now

_Neal_ - Code review from external devs in the future.

#81 - Fixed and tested on OVH machine. 

#69 - FBPT and C are currently both 2015 so they are in line

#73 - .Net is problematic for folks, we could fix it, but there is no action currently. Known issue for .Net programs using PCOM. Provide a sumamry of the issue and we will publish that to the website.

#59 - Updated and ready for integration. Hard to show it has been fixed.