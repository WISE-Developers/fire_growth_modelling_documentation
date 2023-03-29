## Agenda

### 1. Rob Bryce - New Zealand, Automated Systems

_Rob_ - NZ workshop last week to help them decide where to take the next 3-4 years of dev and planning. First 2 presentations were on PSaaS. Wayne and Rob presented on the topic and discussed a major fire on the north island. Got to compare and contrast methods of using PSaaS, saw similar outputs. Next 3-4 years has a focus on smoke modelling and its in the registry now. They require a translation table from US models to FBP, they are also looking at superior data capture with UAVs etc. Looking at ensemble modelling as well. We are now to a point where we can generate too much information. They are looking at ways to better inform through data distillation rather than mass generation. Half day workshop, informal talk after lasted an hour. Automatic PSaaS -> UAVs -> info overload.

_Neal_ - Didn't get an invite to that, am in another one. There are a number of themes and I'm delivering a talk to that talk on YouTube and then they will have a live Q&A later in the summer. Heard back from Canada Wildfire about a presentation hoping to do something early season but there is a waiting list and we are invited to talk either October 14 or early November. Looking to after Wildfire Canada Conference, then Canada Wildfire / CIFFC National Conversations.

### 2. Robert - Brief overview of PSaaS and Framework Stuff

_Robert_ - Continuing work on the modelling framework there are now streams that hit the ftp and CWFIS layers. Also added on an additonal weather service from the WCS at ECCC in addition to GRIB and I'm now testing AMQP. I would like to test some of these inputs in PSaaS but the PSaaS demo does not seem to like PSaaS anymore.

_Brett_ - Updated lately?

_Robert_ - Internal broker.

_Brett_ - Still on 6 we'll move you to 7 soon enough, no longer has an internal broker, gets a little more sticky.

### 3. Franco - What we're up to with containerization

_Franco_ - 3 fully operational psaas systems last year. BC, NT and National using CWFIS and DIP feed. All those modellers were built on an early version of PSaaS 7 and in theory should still work out of the gate however they are using a 2021 version of 7. Re-written to use the most recent in the develop er group. Which is Version 03.01. 

So far I have set up and built a new cutter. These services exist in containers and in theory you need 2 containers for the whole system. 1 container handles input pre-processing by running a cron job that will launch the container, examine the fires and see if they have changed at all and if yea then it will re-evaluate the ignition input and recuts the dataset to fit the new size of the fire. The second container is the builder that contains builder and psaas executable and it uses the information from the 1st container to model a fire. This is a sequential modeller not a concurrent modeller and each of these systems were run independently and periodically. I intend to get NT and National up and running again this year and when those are cleaned up they will be public repositories which will allow you to leverage these modellers via docker. Of course these modellers are a little more NWT centric but the DIP modeller is powered by public information. Used that public model to generate one for BC and SK. These provide a cutter and a modeller and the modeller can be attached to a website so the information can be viewed as it is populated. This will all be made available to the team so you all can get things going in your workflows. I intend to refactor all of this back to the universal API once its stood up.

### 4. Wildfire Canada Submission Abstract - (Franco, Neal, Brett)

_Brett_ - Focus on the story of how we got here. 

_Neal_ - Encouraging others to put in abstracts. We are aware of FireHawk making a submission. These are front end talks but we wanted to get a talk in to really discuss the drive for sustainable fire modelling and the story of this team. Essentially we have gotten to where we are because of volunteerism, grit and determination. We'd like to really show off this team and what we've accomplished. Originally presented on with a RedApp lens and now 10 years later we're about to realize our vision.

_Franco_ - Concept of our story works really well with others layering on what they are doing with our work. Big opportunity for things like firehawk / firecast to show the underpinnings of these front end systems. 

_Neal_ - Putting the abstract in as a multi-author abstract but not who would be giving the talk. There are also travel approvals that could get in the way. 