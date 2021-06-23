# Routing
React Router v4 is a pure React rewrite of the popular React package. Previous versions of React Router used configuration disguised as pseudo-components and could be difficult to understand. With v4, everything is “just components”.
### Installation
React Router has been broken into three packages: react-router, react-router-dom, and react-router-native.
## The Router
When starting a new project, you need to determine which type of router to use. For browser based projects, there are `<BrowserRouter>` and `<HashRouter>` components. The `<BrowserRouter>` should be used when you have a server that will handle dynamic requests (knows how to respond to any possible URI), while the `<HashRouter>` should be used for static websites (where the server can only respond to requests for files that it knows about).
## Matching paths
React Router uses the path-to-regexp package to determine if a route element’s path prop matches the current location. It compiles the path string into a regular expression, which will be matched against the location’s pathname.
`<Route>`s can be created anywhere inside of the router, but often it makes sense to render them in the same place. You can use the `<Switch>` component to group `<Route>`s. The `<Switch>` will iterate over its children elements (the routes) and only render the first one that matches the current pathname.

**Routes have three props that can be used to define what should be rendered when the route’s path matches. Only one should be provided to a `<Route>` element.**
* component — A React component. When a route with a component prop matches, the route will return a new element whose type is the provided React component.
* render — A function that returns a React element 5. It will be called when the path matches. This is similar to component, but is useful for inline rendering and passing extra props to the element.
* children — A function that returns a React element. Unlike the prior two props, this will always be rendered, regardless of whether the route’s path matches the current location.

## Review, Research, and Discussion
* **Do child components have direct access to props/state from the parent?**

 we can see there is no way to pass props from a child component to a parent component. However, we can always pass around functions from the parent to child component. The child component can then make use of these functions. The function can then update the state in a parent component.

* **Can a component, such as `<Content />`, which is a child also be used as a standalone component elsewhere in the application?**

Create a callback function in the parent component. This callback function will get the data from the child component.
Pass the callback function in the parent as a prop to the child component.
The child component calls the parent callback function using props.

## **Term**
* **props.children**
children is a special property of React components which contains any child elements defined within the component.  {this. props. children} includes those children in the rendered result.
* **composition** 
composition
is a natural pattern of the component model. It's how we build components from other components, of varying complexity and specialization through props. Depending on how generalized these components are, they can be used in building many other components.
