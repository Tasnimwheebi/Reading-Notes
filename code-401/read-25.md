# Custom Hooks

## Review, Research, and Discussion
### What does a component’s lifecycle refer to?
The process of each component Mounting, Updating, and Unmounting to the DOM. There are several functions that can be called at each stage, but render() is the only required function for Mounting and Updating.

### Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect
This can be used to prevent rerenders of a function if it is passed to a child as a prop.

### Why are functional components preferred over class components?
They are simpler for deveopers to work on, as they

### What is wrong with the following code?
import React, {useState, useEffect} from 'react';

    function MyComponent(props) {
    const [count, setCount] = useState(0);

    function changeCount(e) {
    setCount(e.target.value);
    }

    let renderedItems = []

    for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update');
    }, [count]);

    renderedItems.push(<div key={i}>Item</div>);
    }

    return (<div>
     <input type='number' value={count} onChange={changeCount}/>
      {renderedItems}
    </div>);
}
useEffect should not be called from inside a loop - react hooks should only be called at the top level.

## Document the following Vocabulary Terms
* state hook - the basic hook of react, equivalent to this.state = {} in a class-based component.

* effect hook - performs side effects in a function component. Can trigger on any page re-render, or specific component renders.

* reducer hook - instead of a state hook which modifies a state in place, a reducer takes a state and a dispatch function, and returns a new state src.
## Using a Custom Hook
* useToggle:
it takes a parameter with value true or false and toggles that value to opposite. It’s useful when we want to take some action into it’s opposite action.

* useAuth:
A very common scenario is you have a bunch of components that need to render different depending on whether the current user is logged in and sometimes call authentication methods like signin, signout, sendPasswordResetEmail, etc.
