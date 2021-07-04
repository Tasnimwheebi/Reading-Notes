# Redux - Combined Reducers
## Review, Research, and Discussion
### Why choose Redux instead of the Context API for global state?
Because it enforces single-source-of-truth, and allows us to standardize how our state is updated across our app. It also allows us to easily modularize our state updates and simplify our interactions with increasingly complex states.

### What is the purpose of a reducer?
A reducer is a pure function that handles updating the state of our application, so that we can only update state from a single, deterministic source.

### What does an action contain?
An action contains an object with properties type and payload. The type tells our reducer what kind of action we want to take, the payload passes data to the reducer which can be used to update state.

### Why do we need to copy the state in a reducer?
State in react is immutable, so we must pass a new copy to our reducer in order to re-set it. This allows us to track state over time and as changes take place.

## Document the following Vocabulary Terms
* immutable state - In redux, the state of an object is immutable. This allows for simpler debugging, change detection, and prevents unwatnted state changes from happening as side-effects elsewhere in your app.

* time travel in redux - by tracking state, redux allows devs to "time travel" by reversing state. Because redux is predictable, you can reliably recreate previous states by passing those state objects into the application state.

* action creator - a function that actually returns an action object to our reducer. By abstracting the call to the action, we simplify our implemented code.

* reducer - a switch function that handles updating the application state (by creating a new state object) depending on the given action call made to it.

* dispatch - the act of passing (or, dispatching) an action from an action creator to a reducer.

### Using combineReducers
The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key. Similarly, the most common approach to writing reducer logic for that state shape is to have "slice reducer" functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of state. Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.

### combineReducers(reducers)
The state produced by `combineReducers()` namespaces the states of each reducer under their keys as passed to `combineReducers()`.
