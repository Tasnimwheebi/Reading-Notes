# Context API
## Review, Research, and Discussion
### Describe use cases for useMemo() and useReducer()
'useMemo()' memoizes large functions so that you can avoid calling them on every render, instead only re-rendering when a passed value is changed. This is good for when we have large, expensive functions that we want to avoid running on every render. src

'useReducer()' is analogous to useState(), but give a more structured approach for updating complex values. This works well for states that contain multiple variables which may be inter-dependent. src

### Why do custom hooks need the use prefix?
Semantics - this helps us as developers quickly identify them as hooks.

### What do custom hooks usually do?
Usually they are designed to remove logic from the UI layer and allow common code functions to be shared among different components (api calls, for instance).

Using any list of custom hooks, research and name one that you think will be useful in your applications
useToggle will come in handy in any number of use cases. Gotta love toggles.

### Describe how a hook that fetches API data might work
Using state and useEffect to fetch API parameters from the UI, then make an API call using axios or some other service on the server side.

## Document the following Vocabulary Terms
* reducer - A built-in hook that can change an application's state using a given dispatch function.

## Use Context
Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. 

### What is a Context :
Context provides a way to pass data through the component tree without having to pass props down manually at every level.

### Before Use Context :
Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.
* If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

* Context.Consumer: A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component.

* Context.displayName: Context object accepts a displayName string property. React DevTools uses this string to determine what to display for the context.
