#  Component Composition
##  The Component Lifecycle
A component can only be in one stage at a time. It starts with mounting and moves onto updating. It stays updating perpetually until it gets removed from the virtual DOM. Then it goes into the unmounting phase and gets removed from the DOM.

The lifecycle methods allow us to run code at specific points in the component’s life or in response to changes in the component’s life.

### Mounting
* Since class-based components are classes, hence the name, the first method that runs is the constructor method. 

* Next, the component runs the getDerivedStateFromProps.

* Then render method which returns your JSX. Now React “mounts” onto the DOM.

* Lastly, the componentDidMount method runs.

### Updating

* This phase is triggered every time state or props change.
* Next shouldComponentUpdate runs.
*  If shouldComponentUpdate returns false, this update cycle ends.

### Unmounting
The unmounting phase is that last stage of the component lifecycle. When you remove a component from the DOM, React runs componentWillUnmount right before it gets removed.
##  Higher-Order Components
A higher-order component is a function that takes a component and returns a new component.
##  React State and setState()
 The only way you should change state is via the setState method. This method takes an object and merges it into the current state.
setState is asynchronous. This means state won’t update exactly after you call setState and this can lead to some aggravating behavior which we will hopefully now be able to avoid!

###  React Context
The React context API allows you to create global context objects that can be given to any component you make. This allows you to share data without having to pass props down all the way through the DOM tree.

## Review, Research, and Discussion
* **Can a parent component access the state of a child component?**
To be able to access and update state from the child component, we can add a method that handles updating the state to the parent component and pass the method as a prop to the child component instead of the state itself.

* **What can be passed along in a prop variable?**
There is no way in React to set props (even though it was possible in the past). After all, props are only used to pass data from one component to another component React, but only from parent to child components down the component tree.
* **How can a child component “know” the state of another component?**
Step1: Create a Provider Component for the two children. Step 2: Pass the state and the callback function as props to all children inside the Provider Component. The provider is the boss for its children (the global store of all the states and callback functions to manipulate those states).

## **Term**
* **component props**
Props are arguments passed into React components. Props are passed to components via HTML attributes.
When React sees an element representing a user-defined component, it passes JSX attributes and children to this component as a single object. We call this object “props”.

* **component state**
React components has a built-in state object. The state object is where you store property values that belongs to the component. When the state object changes, the component re-renders.

* **application state**

The state is just a fancy term for a JavaScript data structure. If a user changes state by interacting with your application, the UI may look completely different afterwards, because it's represented by this new state rather than the old state. Make a state variable responsible for one concern to use efficiently.
