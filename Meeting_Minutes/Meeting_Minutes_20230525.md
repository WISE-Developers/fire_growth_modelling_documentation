# Agenda

| Attendees |
|---|
|Brett|
|Franco|
|Robert J|
|Rob Kruus|
|Brad Armitage|
|Rob Bryce|
||
||
||

## 1. WISE as an operational modeller [Franco]

In short, built a dip modeller, handed this to CFS, CFS moved it to use WISE. Sequential point based dip modeller running in Azure. Partially in Azure, partially in backend and it's working. 

Haven't been running WISE locally, had PSaaS going, when I wanted to move to WISE I used the CFS version, currently rejigging it to get it to the point of modelling points again. Next we are moving to polygons. The code already exists in there it's just not being used. We are going to point to the FireM3 polygons first. 

 - 1 Model dip fires again
 - 2 Enable dip fire modelling from M3 polygons
 - 3 Push and share this code
 - 4 Warp it into just being a modeller for the NWT (fork at this point)

Expecting a week out for most of this, running points by tomorrow on the lastest release of WISE. (beta 6)

## 2. Experiences over the last month with FireCast [Rob]

Version being used?

AB put WISE to the test.

23 machines 4 locations, 1000 cores, 6 Tb of RAM, no crashes of WISE. Standard outputs that were nice. Lots of issues with network and data feeds and k8s but WISE stood through it. In this process we are running 200 sims at a time. Performance issues noticed. Det runs were no issues, ensembles were a struggle.

Getting into non-standard stuff now and gusting.
