# Props and State
## Workings of `setState()`
`setState()` is the only legitimate way to update state after the initial state setup.

`Object.assign()` is used to copy data from a source object to a target object. If the data being copied from the source to the target all have same keys.

So instead of the call happening three times, it happens just once. This can be fixed by passing a function to `setState()`. Just as you pass objects to `setState()`, you can also pass functions.

## Access State Using Updater
 You cannot always trust this.state to hold the correct state immediately after calling `setState()`, as it is always equal to the state rendered on the screen.

 `setState()` should be treated asynchronously — in other words, do not always expect that the state has changed after calling `setState()`.

 **When working with setState(), these are the major things you should know:**

* Update to a component state should be done using `setState()`.
* You can pass an object or a function to `setState()`.
* Pass a function when you can to update state multiple times.
* Do not depend on this.state immediately after calling `setState()` and make use of the updater function instead.

## Components and Props
Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. 

## Forms
HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state.

### Controlled Components
In HTML, form elements such as `<input>`, `<textarea>`, and `<select>` typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

In HTML, an `<input type="file">` lets the user choose one or more files from their device storage to be uploaded to a server or manipulated by JavaScript via the File API.

## Handling Events
Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:

React events are named using camelCase, rather than lowercase.
With JSX you pass a function as the event handler, rather than a string.

## Review, Research, and Discussion
* **Does a deployed React application require a server?**

You don't necessarily need a static server in order to run a Create React App project in production. It also works well when integrated into an existing server side app.
* **What does npm run build do?**

npm run build runs the script "build" and created a script which runs your application - let's say server.js.
npm start runs the "start" script which will then be "node server.js"

* **Describe the actual composition / architecture of a React application**

Unlike other UI libraries and frameworks, Reactjs doesn't enforce an architecture pattern. It is just a view that caters to the user interface. Just beneath the user interface lies a tree of several React components.

## **Term**
* **BDD** : Behaviour Driven Development

Behaviour Driven Development (BDD) is a synthesis and refinement of practices stemming from Test Driven Development (TDD) and Acceptance Test Driven Development (ATDD).

* **Acceptance Tests** :
This is a type of testing done by users, customers, or other authorised entities to determine application/software needs and business processes. It is also known as user acceptance testing (UAT), operational acceptance testing (OAT), and end-user testing.

* **Mounting** : is the process of outputting the virtual representation of a component into the final UI representation (e.g. DOM or Native Components). In a browser that would mean outputting a React Element into an actual DOM element (e.g. an HTML div or li element) in the DOM tree.

* **build** represents the path to our final production build. This folder would actually be created after we run the npm build. We can see all the "dependencies" and "devDependencies" required by our React app in node_modules. These are as specified or seen in our package. json file.

