## Review, Research, and Discussion
### Compare and Contrast Redux Toolkit with Redux "Ducks"
"Ducks" file structure proposes putting all of your Redux-related logic for a given slice into a single file
RTK follows the ducks pattern and combines reducers, actions, and constants in one file called a slice. Each slice will provide an initial state and a reducer function for an object in store. 
### What is the principle advantage of Redux Toolkit
* It allows us to write more efficient code, speed up the development process, and automatically apply the best-recommended practices. It was mainly created to solve the THREE MAJOR ISSUES with Redux:
  * Configuring a Redux store is too complicated
  *Have to add a lot of packages to build a large scale application
  *Redux requires too much boilerplate code which makes it cumbersome to write efficient and clean code. 
## Document the following vocab words
* redux toolkit slices: A function that accepts an initial state, an object full of reducer functions, and a "slice name", and automatically generates action creators and action types that correspond to the reducers and state. 
* namespace: In computing, a namespace is a set of signs (names) that are used to identify and refer to objects of various kinds. A namespace ensures that all of a given set of objects have unique names so that they can be easily identified. 




## Create native apps for Android and iOS using React
React Native combines the best parts of native development with React, a best-in-class JavaScript library for building user interfaces.
Use a little—or a lot. You can use React Native today in your existing Android and iOS projects or you can create a whole new app from scratch.


React Native lets you create truly native apps and doesn't compromise your users' experiences. It provides a core set of platform agnostic native components like View, Text, and Image that map directly to the platform’s native UI building blocks.
What is the difference between Reactjs and react native?
In Reactjs, virtual DOM is used to render browser code in Reactjs while in React Native, native APIs are used to render components in mobile. The apps developed with Reactjs renders HTML in UI while React Native uses JSX for rendering UI, which is nothing but javascript.
## Ejecting to ExpoKit

ExpoKit is an Objective-C and Java library that allows you to use the Expo platform and your existing Expo project as part of a larger standard native project -- one that you would normally create using Xcode, Android Studio, or react-native init.

Normally, Expo apps are written in pure JS and never "drop down" to the native iOS or Android layer. This is core to the Expo philosophy and it's part of what makes Expo fast and powerful to use.
However, there are some cases where advanced developers need native capabilities outside of what Expo offers out-of-the-box. The most common situation is when a project requires a specific Native Module which is not supported by React Native Core or the Expo SDK.
In this case, Expo allows you to eject your pure-JS project from the Expo iOS/Android clients, providing you with native projects that can be opened and built with Xcode and Android Studio. Those projects will have dependencies on ExpoKit, so everything you already built will keep working as it did before.
We call this "ejecting" because you still depend on the Expo SDK, but your project no longer lives inside Expo Go. You control the native projects, including configuring and building them yourself.

