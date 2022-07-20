## Agenda

### 1. Rob issues regarding Ubuntu

_Rob_ - Briefly, on the windows builds we discovered and did a lot of work to tie processes to specific cores and nodes to mitigate NUMA issues. We have tried a few methods in Ubuntu but they don't seem to be doing that.

_Franco_ - Is this a real issue?

_Brett_ - Yes this was something I needed as when you have multiple physical nodes bad things happen.

_Franco_ - Is it documented somewhere? 

_Brett_ - Yes, redmine, we can bring it forward to GitHub.

_Rob_ - Physical machines multiple AMD rigs, different reactions by the software.

_Franco_ - Ultimately the only issue is in Ubuntu but we need to test more platforms.

_Rob_ - Correct, we have shortlisted Linux systems but we have not tested across all of them, at least not the way the fix in Windows worked.

_Rob_ - Will make an issue for this.

_Franco_ - Short meeting today, ciao for now.

_Rob Kruus_ - Suggested version of linux for PSaaS?

_Rob_ - Ubuntu 20.04