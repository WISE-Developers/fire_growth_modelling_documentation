# Agenda

## Attendees

Brett Moore
Rob Bryce
Robert Jagodzinski
Rob Kruus

### 1. Validation Work

Tried to use the stats file but they weren't archived. Moving to pull shapefiles directly and I'll filter down from there.

### 2. Status of Things on GitHub

Overall Status, two big groups of work, last minute development (changes that may impact protobuff or json formats [basically done]) and moving all the code into GitHub.
Repos made just before Christmas to group functionality which reorged the code on HSS side. Proceeded to move the code up and Travis has been testing builds with GitHub Actions. 3 builds Ubuntu 20, 22 and Windows. No one really using windows currently but didn't want to drop support.

As of 2 days ago all building working, but linking isn't working perfectly yet. Boost continues to be rude when not build "just so" (protobuff requirements). GitHub doesn't deterministically build, but so to VS didn't.

Need to wait until things tip over to find issues. Compilation / installation ready for Linux builds, not quite there for windows. Functional outputs exist even though we missed the target we are very close to final delivery.

### 3. GitHub Actions Limit

Free 2k per month. Paid after that.

Rates:

https://docs.github.com/en/billing/managing-billing-for-github-actions/about-billing-for-github-actions#per-minute-rates

Per-minute rates
Operating system|   Cores	| Per-minute rate (USD)
Linux	        |     2	    |     $0.008
macOS	        |     3	    |     $0.08
Windows	        |     2	    |     $0.016
Linux	        |     4	    |     $0.016
Linux	        |     8	    |     $0.032
Linux	        |     16    |     $0.064
Linux	        |     32    |     $0.128
Linux	        |     64    |     $0.256
Windows	        |     8	    |     $0.064
Windows	        |     16    |     $0.128
Windows	        |     32    |     $0.256
Windows	        |     64    |     $0.512