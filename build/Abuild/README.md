# Nginx defect report
Although Nginx has been ported, there are still some big issues in packaging and testing. Currently, around 0.01% (of ~5400) of the tests are failing.
# Features not working
## perl module
Nginx uses `dlopen()` to load modules dynamically, the rpath issue mentiend in [here](https://jira.bbqnx.net/browse/COREOS-130134) needs to be fix to enable perl support.
## http degration
sbrk/brk not supported

# Status
Not distributed yet, remain testing until further requirements