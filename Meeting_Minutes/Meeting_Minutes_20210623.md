- [1. Prometheus Releases](#1-prometheus-releases)
- [2. Testing](#2-testing)
- [3. Budget](#3-budget)
- [4. Redapp convo](#4-redapp-convo)
- [5. NZ update](#5-nz-update)
- [6. Fireshed learnings](#6-fireshed-learnings)

## 1. Prometheus Releases

Next month getting back on track. Dev builds should only have 1 item in there. Only things tested should be put into the monthly builds. The first of the month is intended to be an automatic build. Monthly will come out regardless of progress being made.

This allows us to properly stage our development builds.

Release build has been requested as a release for BP3 is needed for the public offering. I'm leaving at the end of the next week and the new features requested aren't necessary for Burn-P3 and may not be necessary for the broader prometheus community (correct me if I'm wrong here). 

## 2. Testing

Tasks and items have been assigned without instruction or guidance. We are also missing a category "ready for release". If tickets are properly elucidated it will make it much easier for us all to work forward and close tickets out.

Getting Liz up to speed should help us get moving faster.

Rob Krus - testing datasets to ensure tests can be redone. Do we have a repository?

Franco currently building containerized structure for Psaas 7.

## 3. Budget

Working on moving over 100k, if that fails we will use provincial contracting to perform work. Should know on budget approvals by next week. Now and in the coming weeks, if you have additional budget, and can send it to CIFFC please do. Otherwise you can contract the individual you require directly.

## 4. Redapp convo

RedApp hasn't had a release in a while, though one is anticipated. Went and met with Rob and Brett to assess the state of development. There were a number of build requests piled ontop of one another. I have sorted this out and stripped away some of the feature requests to get us closer to a proper build. In this way we are pulling back and getting all the fixes out in an effort to get something out to the user community. 

What I would like to do is fast track a bug release for RedApp. 

**Neal:** A release of Prometheus means a release of RedApp. Liz had done some testing, but none of that made it into RedMine so that'll get in there pending our discussion. Bug fixes now, features later.

## 5. NZ update

PDE approach is problematic, thus we are moving forward on integrating some levelset work. They have issues due to all the vectors they are using. Otherwise we have hit many of their validation targets. They found some more funding, which has been dedicated to levelset. Will be hosted within Scion.

## 6. Fireshed learnings

We can run multiple instances of PSaaS on 1 machine and multiple machines at 1 time (up to 20). Has load balancing. The load balancer has been moved up to AWS, which addresses some of the scaling issues. This should help with some scaling as loads increase as machines need to be brought on and dumped.