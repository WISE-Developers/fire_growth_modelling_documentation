<!-- vscode-markdown-toc -->
1. [Release candidate for Prometheus](#ReleasecandidateforPrometheus)
2. [Bug / Task update](#BugTaskupdate)
3. [New Export Options](#NewExportOptions)
4. [RedMine Death](#RedMineDeath)
5. [FireHawk](#FireHawk)
6. [Website](#Website)
7. [GitHub Admin](#GitHubAdmin)
8. [File Storage](#FileStorage)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->
##  1. <a name='ReleasecandidateforPrometheus'></a>Release candidate for Prometheus

We are getting there, a number of GUI related items to address. Version numbers and some unicode symbols. Had developed a new fuel consumption and FRP statistics, but they are not ready for the public due to a lack of performance. They are hidden for now but will be available for testing.

Outstanding item for testing - how we go about providing stats from vertices to grids. 

Require some help with [#1249](https://ppm.redapp.org/issues/1249) in Redmine PSaaS Perimeter Rotation Problem. Some rotations are standard and consistent, some methods are not consistent. This will help ensure that holes are declared holes. 

Issue found doing work for various agencies. Found that some fires would just stop burning, and this was due to the file format. Some formats do compas rotation and others do cartesian rotation. Compass is clockwise, Cartesian is counter-clockwise. New JSON spec defines rotation, old versions did not. Intending to have more than 1 shapefile with many rotations to ensure prometheus is performing it correctly.

Testing the system to detect the rotation and adjust it if necessary. Preferrably we would need to tell the user there was an issue but reject the polygon. This will help us define and adhere to a specification wrt polygonal rotation.

##  2. <a name='BugTaskupdate'></a>Bug / Task update

Remove the cell discretization meterics, otherwise should be good to go.

##  3. <a name='NewExportOptions'></a>New Export Options

Landscape vs Fire Simulation. Landscape is just a point in time. Fire Simulation is for the fire specifically. 

Outstanding item here is the number of vertices in each polygon. Sometimes cells are skipped completely, so producing a grid output its using surrounding vertices.

New approach for the fire grid statistics, potentially determine the time of the burn then use the base grids to calculate the FBP outputs.

##  4. <a name='RedMineDeath'></a>RedMine Death

Redmine hosting is at NT and on the oldest infrastructure, so everything needs to be purged out. GNWT wants us off RedMine to remove the VM. Stop putting items in RedMine and move them to GitHub after the release.

##  5. <a name='FireHawk'></a>FireHawk

Federal meeting discussing FireHawk. This is intended to be a friendly version of prometheus. Sounds like this is the work that Alex is up to.

##  6. <a name='Website'></a>Website

Redapp website is an old system that cannot be nicely updated. It will fail within a month. Migrate the community to discord potentially? Franco has low level websites that could be of use. Potentials on what we can do, but need some direction. We need to determine where this will live though as this project has no physical real estate. 

Websites needed, PSaaS, RedApp, Prometheus.

_*Neal*_ - Put forward request to Manny with CIFFC for assistance on this asap. See if they have interest in hosting this from the toolbox perspective.

Perhaps we scope this over to GitHub pages. Purchase the domain name, point it at github pages.

##  7. <a name='GitHubAdmin'></a>GitHub Admin

Getting another github account, we need an organization account (this is around 300$ a year). This will allow us to perform all the tasks we need to perform. If we are good to go in this group then I think teh investments we make will only service us into the future.

Just need to point the domain name at the github pages endpoint.

##  8. <a name='FileStorage'></a>File Storage

This is the history of promtheus. Uplaoding to a solution made by Franco.