# Redux - Asynchronous Actions
## Review, Research, and Discussion
### How granular should your reducers be?

Generally, as granular as possible. This allows for easier organizion, debugging, and testing. It also allows you to more easily add new features or remove features in the future. src

Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched

PRO! Having multiple reducers fire on a shared action is a great way to handle complex state changes in a predicable, reliable, and modular way, as long as it is intended.

### Name a strategy for preventing the above

Use explicit names for each action to prevent unintended firing (i.e. don't use 'RESET' for every reducer... unless you want them all to reset at the same time!)

## Term

* store - the object created by redux that stores all states for a given application. This is the single source of truth for our application.

* combined reducers - a way redux allows us to 'export' many reducer files from a single source to our store, so that they are all available in different parts of an app.



## What is Redux?

Redux takes away some of the hassles faced with state management in large applications. It provides you with a great developer experience, and makes sure that the testability of your app isn’t sacrificed for any of those.

## Why use Redux?

One other reason a lot of developers love Redux is the developer experience that comes with it. A lot of other tools have begun to do similar things, but big credits to Redux.

Some of the nice things you get with using Redux include logging, hot reloading, time travel, universal apps, record and replay — all without doing so much on your end as the developer. 

Redux offers a tradeoff:

* Describe application state as plain objects and arrays.
* Describe changes in the system as plain objects.
* Describe the logic for handling changes as pure functions.
