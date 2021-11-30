# Agenda

Attendees: Brett, Rob, Mac, Rob K, Peter
- [1. Discuss last weeks dev meeting](#1-discuss-last-weeks-dev-meeting)
- [2. What are we doing about Lux?](#2-what-are-we-doing-about-lux)
- [3. Multithreading - Rob](#3-multithreading---rob)
- [4. Code signing certificate](#4-code-signing-certificate)
## 1. Discuss last weeks dev meeting
- Item on Prometheus Core Lock

Mac: We do currently have some thread management. 
Rob: Those settings are scenario specific, we do this for one scenario at a time to maximize throughput. This should be turned off in BP3 to allow it to max out throughput.
Mac: When there are many cores I allow prometheus to use more threads to attempt to speed it up. 
Rob: Bottlenecks are found in the simulation itself were we break up the perimeter over threads to about 8 threads. BP3 should keep each simulation single threaded to change the bottleneck origin. If we are running 8 simulations and 2 cores per simulation then you're in an area we haven't tested. 
Mac: Any work on the locks to assist multithreading.
Rob: We are single threading each simulation and then running many simulations.
Mac: Still has a tipping point.
Rob: Yes, we usually use 5-6 but never past 10 as then we start to lose performance. This could be a memory zone allocaiton issue, I would like to move to a per thread zone allocation.

- [ ] create an item for per thread memory zone allocation
> End of the day this is a shared resource bottleneck

Rob: The other thing to note here with regard to thread affinity and number of threads for Burn-P3. Prometheus would suggest threads and cores to give affinity.
Mac: OpenMP has a limited future as it is moving on but microsoft is not supporting further versions. 
Software is ignorant of NUMA nodes, so its starting up too many threads and they are getting queued and generate their own bottleneck.

- [ ] Brett: Add issue in redmine for mac to update how he talks to GDAL. Within process use Robs semafor for GDAL atomic access

This will stop process boundary crossing crushing and failures of the program walking on itself. Synchronization among threads within a process.

## 2. What are we doing about Lux?
- yes because, no because?

Results:
| Name      | Verdict                          |
| --------- | -------------------------------- |
| Brett     | Yes, invite to next meeting      |
| Franco    | Yes, invite to next meeting      |
| Rob Kruus |                                  |
| Peter     | Yes, invite, what is their role? |

Can we also get some additional information on how Lux will be participating?
How will we introduce them to the project?
## 3. Multithreading - Rob
3 different modes here:

1. Interactive - prometheus, limit the number of threads used in the system overall, maximum 8 per simulation but as many as possible when generating statistics
2. Large batch job - similar, 1 thread per simulation, but a maximum of 8 simulating at once. When generating outputs we need to lock to the same number of cores.
3. Real-time operation - maximize throughput for simulation but also allow for all cores to generate stats within a NUMA node.

Rob thinks that BP3 is in the second. 2 bit masks, cores used for simulation and cores for stats generation.

Mac: How is 1 and 3 different?
Rob: 1 is interactive, while 3 is programmatically operating. Different in overall system utilization. End of the day we have to ensure they don't step over the NUMA node.

Mac: Bit mask for core allocation?
Rob: for thread yes, i treat them as cores as thread is a system term.
Mac: Yes we discussed this this morning as the terminology is all the same but the words mean different things.

Rob: Either I suggest to you what cores to use or you tell me with a bit mask what cores you will be using.
Mac: This makes BP3 obliged to take a look at the hardware that it is being run upon. 
Rob: I can manage the system assessment side of things, and I can give you cores that you ask for by me looking for them rather than you being the hunter for resources.
Mac: I think I'd rather have BP3 control where it wants to run, as it goes through the process of generating threads we would pass it off single threaded to Prometheus already on a thread assigned to a location.

Mac: Biggest challenge is that the user can make changes to affinity irrespective of what the software tells the system.
Rob: The OS has to give us credentials to do this work and I've never had an issue with the system not giving me credentials. We can do the affinity assessment programmatically.
Mac: Are cores listed by NUMA node?
Rob: They are listed by group, then you can query each core for its NUMA set.

Rob: Independent solutions are appropriate here. PSaaS already solves the issue with Manager. If BP3 and Prometheus are not running at the same time, it'll be fine to stay independent.

Rob: We require process awareness so a shared memory block may be the way to go. This is a shared memory region that will be the easiest IPC available utility.

For reference, NUMA Node - the memory space that multiple sockets talk to one another inside of.

## 4. Code signing certificate

Given proof of existence both provincial and federal, they need proof of physical location, mail was insufficient. Google did not want to put the address on my location as I do not have a sign. Dunns and Bradstreet is adding the phone number, currently unable to validate due to it being a cell. One course needs everything to get the certificate completed. This will be difficult. This will likely take another 2 - 3 weeks to sort things out. May investigate other locations to see if other places can assist in getting this done sooner.