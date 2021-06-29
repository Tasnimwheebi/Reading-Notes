# `<Login /> and <Auth />`
## Review, Research, and Discussion
### Why is the Context API useful?
It allows you to pass props down multiple levels of a component tree without having to manually pass the prop each time, essentailly providing a shortcut for props to granchildren etc. src

### Can a component outside of a provider get its context?
## What are some common use cases for using the Context API?
Passing UI Themes, local preferences, or any parameter which needs to be consumable to many different levels of components at the same time.

### Describe “Context Hell”
When you have too many nested contexts... This is similar to callback hell. Can be addressed with the 'React.cloneElement()' function which returns a new element using the initial 'element' as a starting point. src

## Document the following Vocabulary Terms
* global state - state which is declared at the app-level. src

* global context - context which is visible to the entire app.

* provider - a component who's context changes can be subscribed to by a consumer.

* consumer - A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component.


*** 
**The React Context API is a way for a React app to effectively produce global variables that can be passed around. This is the alternative to “prop drilling” or moving props from grandparent to child to parent, and so on. Context is also touted as an easier, lighter approach to state management using Redux**
### Role-Based Access Control (RBAC)
Role-based access control (RBAC) restricts network access based on a person’s role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

Employees are only allowed to access the information necessary to effectively perform their job duties. Access can be based on several factors, such as authority, responsibility, and job competency. In addition, access to computer resources can be limited to specific tasks such as the ability to view, create, or modify a file.

### Benefits of RBAC
* Reducing administrative work and IT support. 
* Maximizing operational efficiency.
* Improving compliance. 

