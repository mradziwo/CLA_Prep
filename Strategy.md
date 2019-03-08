

# Strategy for CAL with AF

# Action Plan

## Documentation


## ToDo

* All individual actor methods will be static dispatch
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
