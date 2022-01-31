Jordan working on making Firestarr work without grabbing 100 gb
Franco work on PSaaS Framework will only point at PSaaS per NWT funding
PSaaS as primary model in CWFIF
Robert to work on intigrations of PSaaS, C2F and Super Duper

### ** Build a workplan **

Management is good with it so far, may have more models for the future.

_Franco_ - CI build schedules - weather file generation

_Robert_ - getting familiar, things are running, want to work on what is the priority and facilitate the workflow. Get us towards standardizing inputs. Containerization and batching within a pipeline for a test case. Delegation of tasks as the team gets moving ahead.

_Franco_ - need to integrate GH into assana, clear understanding of what is missing from GH PM wrt pushing dev work up foodchaing to non dev decision makers. What is out track and where are we having stumbling blocks. Build a Kan Ban board. Less project plan needed more guideline requirements. I am weak at stop and tell before I go and define what's going on to the folks above. Looking to standardize disparate tools for consistent reporting. Just did that with pushing work back up to assana. Establish milestones as well. Much of what we are doing have complex dependencies, so we can't define what can start when and what needs to be done. Establish larger milestones and then bucket the work under those target dates. Establish a list of milestones with dates and then frame the work around those milestones. Then when we start cutting code it'll be much easier for us to push our work into other PM tools.

1. establish milestones
2. build kanban

This is a method for us to develop the community based ideal of this work. We're doing what we can to actually show what collaboration looks like.

_Franco_ - Demo repo changes due to dependabot. Additionally newer versions appear to be shipped with an older version of the API. Made some changes this morning to migrate JSAPI from bitbucket to the dev team reposet on github. Modified the versioning from Datever to semver, thsi is most important for yarn, it will fail without semver compatibility. Re-versioned the current version to be semver compatible, the github repo now has the yarn compatible structure.
Not sure how the administation of this project will work, the assumption is to use consensus or majority vote, what is the tie breaking structure? When we are in conflict, how do we manage issues.

How do we feel about a live version of this running? Test implementation of the framework that is just up on a test server that Franco has as a temporary holding of the project. If yes, utilize the pipeline to push the new live system.

This is a method to ensure we are public facing all the time and we stop worrying about the system being perfect and ready to display.
