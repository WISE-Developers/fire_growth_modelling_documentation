
# PSaaS Meeting May 25, 2022

## Attendance

- Rob Kruus
- Brad Armitage
- Franco Nogarin
- Neal McLoughlin
- Rob Bryce
- Robert J

## Meeting split into two sections

Group  Meeting till 2:30pm

Exec Meeting 2:30-3pm Franco and Neal - ZenHub Project Management

### Group  Meeting till 2:30pm

#### Current Budget

25k - From Sask for 2022
25k - From NWT for 2022
8k - Target NT - Spent on the Redapp work - Rob has been paid

We now have 50k

#### Future Work

- combo ciffc and agency directed funding
- we pay gst when we do a ciffc, and no gst when agency
- AB dropped the funding ball again :(

#### Conference

Conference abstract - Neal will get it in on time due on the 27th

Neals pres video for NZ, due end of the week. He will hsare to Franco and Brett who will share to the team

#### Franco Update

##### (UVF)Framework

Franco has created new nwt Branch called nt-2022-ops
This iwll be the NWT implementation of the UFW.
Intention is for this to be the groundwork for the entire API moving forward.

Implements a new TimeZone Service. see:
    <https://github.com/CWFMF/modelling_framework/blob/nt-2022-ops/src/preprocessing/timezone/timezoneService.ts>

also made a set of tests for the service here:
    <https://github.com/CWFMF/modelling_framework/blob/nt-2022-ops/src/preprocessing/timezone/tzTests.ts>

test results look like this:

```BASH
Testing timeZoneStringByLatLong(60,-111) should be: America/Yellowknife got: America/Yellowknife
Testing timeZoneStringToOffset(America/Yellowknife) should be -6 for MDT or -7 for MST got: -6
Testing timeZoneOffsetByLatLong(60,-111) should be -6 for MDT or -7 for MST got: -6
```

##### DIP Modeller for CFS Hosted at NT

Will be standing up a DIP modeller for CFS and will provide access to it for the team & CFS to view.

### Exec Meeting 2:30-3pm Franco and Neal - ZenHub Project Management

#### Franco and Neal Review Zen Hub Structure

- How BC Does it. - quick overview from Neal
  - Lots of cross over
- How Franco and Brett Implemented this structure
  - Neal is happy with our approach

#### Franco and Neal Discuss the EPICs ("VerifyAndClose" and "Next PSaaS Build")

- Neal is happy with this approach and these two epics.
  
#### Franco and Neal Discuss Budgets

- EPIC vs SPRINT for each budget
- Made 2 new EPICs for NT and SK Budget
- We may convert them to SPRINTS instead

#### Franco and Neal Discuss Issues for Rob

- Too many issues to address today, will plan a future session.
- General agreement that this is a good approach to ease Rob into these methodologies.

#### Franco and Neal Plan Session (May 26, 9am MDT)

- We agree to meet tomorrow and action as many issues as we can.
