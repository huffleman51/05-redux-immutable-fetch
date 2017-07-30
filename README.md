Tutorial that I followed is [here](https://github.com/verekia/js-stack-from-scratch/blob/master/tutorial/05-redux-immutable-fetch.md#readme).

# What I learned in this module

1. ImmutableJS (or just Immutable) is a library by Facebook to manipulate immutable collections, like lists and maps. Any change made on an immutable object returns a new object without mutating the original object. This approach follows the functional programming paradigm, which works really well with Redux.
```javascript
   const immutablePerson = Immutable.fromJS({
      name: 'Stan',
      friends: ['Kyle', 'Cartman', 'Kenny'],
    }) 
```
1. When creating immutable collections, a very convenient method is Immutable.fromJS(), which takes any regular JS object or array and returns a deeply immutable version of it.
```javascript
  const immutablePerson = Immutable.fromJS({
      name: 'Stan',
      friends: ['Kyle', 'Cartman', 'Kenny'],
    })
```
1. Redux is a library to handle the lifecycle of your application. It creates a store, which is the single source of truth of the state of your app at any given time.
1. react-redux connects a Redux store with React components. With react-redux, when the Redux store changes, React components get automatically updated. They can also fire Redux actions.
1. Components are dumb React components, in a sense that they don't know anything about the Redux state. They are logic-less, and just show whatever they are asked to show via React props.
1. Containers are smart components that know about the state and that we are going to connect to our dumb components.  Create smart containers that will feed the proper action dispatchers and data to dumb components.
1. Initialize a Redux Store with the reducers.  
1. Fetch is a standardized JavaScript function to make asynchronous calls inspired by jQuery's AJAX methods. Use fetch to make calls to the server from the client.
1. `fetch` is not supported by all browsers yet, so we are going to need a polyfill. isomorphic-fetch is a polyfill that makes it work cross-browsers and in Node too!
1. Asynchronous actions are usually split into 3 actions, which trigger 3 different states: a request action (or "loading"), a success action, and a failure action.
1. In order to perform these async actions, we need to extend Redux's functionality with the redux-thunk middleware.
1. How to test Redux Action fetch-mock and redux-mock-store
1. How to test Redux Reducer 

