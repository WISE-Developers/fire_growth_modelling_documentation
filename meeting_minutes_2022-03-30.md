# March 30, 2022 PSaaS meeting minutes:
Thanks to Rob K and Neal for taking notes ;-)
 

## Forsite Request to join PSaaS Development Team

* Forsite has approached Franco and Neal to join the development team.
* Neal has provided Forsite with the FAQ responses from Discord regarding early access to PSaaS and joining the development team.
* Next step is to provide Forsite with an orientation to the PSaaS project. Neal and Franco will organize this. Liz and Brad have expressed interest in attending.
* Following the project orientation we will require a written proposal from Forsite.
* _Jordan Said_: Need to be careful getting too many invloved before a formal release.

## Update on BCWS and Canada Wildfire Presentations

* Neal and Robert Bryce presented on Prometheus EOL, PSaaS modernization, and Firecast demo on March 29. The presentation was well received and confirmed that automated fire growth modelling is valued by BCWS.
* The presentation also highlighted that organizations who have not been involved with the project have low awareness of Prometheus EOL and PSaaS.
* Mike Flannigan has connected Neal to Canada Wildfire to provide a national webinar in early spring 2022.
* Neal will present a draft presentation to the PSaaS development for critique and feedback during our next meeting on April 13.
* Neal will schedule a national webinar with Canada Wildfire once the development team is happy with the presentation.
 

# Burn-P3 update

*  Brad requested a status update on BP3
*  _Franco said:_ Brett is building a new release that is compatible with Prometheus 2021.12.03.
* _Neal said:_ I Will ask Brett to add further updates to these meeting minutes.
 
# New Website and Releases

* Franco provided a demo of the new firegrowthmodel.com website.
* Look and feel is updated, but main structure is the same.  Backend technology is much different.
* Better location for download files needs to be worked on (currently securely hosted by Franco).
* All downloads point to a release with the build number. 
* log4j safety is highlighted.
* Support will be mainly be via Github or Discord. Github feedback will notify Franco, Brett and Neil.
* Discord links will encourage use of discord, join the server or direct to a channel, depending if user already has discord.
* Bugs and feature requests will go through github with sane defaults in templates.
* All pages will be served though Github, single source to make changes. Only really need to pay for domain names.
* Some typos and errors were pointed out during the meeting and fixed live .
* Burn-P3 and Pandora point out reliance on Prometheus COM and EOL.
* The website will be deployed overnight on March 30.
* Updates and changes submitted over the past two weeks have been incorporated.
* SOP's/FAQ's are also available in the Discord, Franco will add a tol to find stuff in discord.
* The New builds will be made available for Prometheus, REDapp, and Burn-P3 on the new site.
* Release notes are still required for Prometheus, but will not postpone the website release.
* French translation will need to be worked on -- Brad mentioned Ember has a person to review it as an in kind donation.
* Neal is to read the EOL statement and provide revisions through Github.
* Software support tabs point to Github and Discord (not email addresses). Burn-P3 and Pandora are the two exceptions that still provide email addresses for support.
* Other websites like redapp.org will be updated to point at the new website.
 

# New SK Funding Support

* Robert Kruus will be transferring ~$25,000 to the CIFFC account for this project.
* Neal would like to be notified when this happens so he can confirm our account balance is correct.
 

# Modelling Framework Update

* Robert J. has been coding separate modules in the spirit of the API that help prepare inputs for Prometheus based on what was done last summer, eg.) raster clipping.
* Modelling framework/Model input generation code i.e rate buffering/ clipping etc.
* Code is up on Github.
* Jordan commented that some of the code points at data sources that are only accessible to CFS, and not the public.



