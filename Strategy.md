

# Strategy for CAL with AF

# Action Plan

## Documentation


## ToDo

* All individual actor methods will be static dispatch
*  if pure while - Helper loops stopped by local variables (set to false  at start of Actor core and set to stop at end) OR'ed with error from enqueuer
* if Event loops - Create event ref in prelaunchInit.vi and destroy it in stop core.vi
* in prelaunchinit delete event if parent method failed - if there is error actor core will not be launched, so stop core will not execute as well.
* events in private data should be in clusters (allow direct writing to register for events)
* Errors fron helper loop needs to be handled!
## GUI

* put all references to controllable gui objects to class private data
### Overrides

#### Base Actor
Implement some functionality common to all actors
* Make sure error will not stop on its own! - document!

#### Handle error 
Error handler can stop other modules.


### Root actor
* derived from Base actor
* Should launch all nested actors (starting from error handler)
* should stop all needed actors
