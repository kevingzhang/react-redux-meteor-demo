# react-redux-meteor-demo

####Note
This demo is not meant to be a full-feature todos app and it's unpolished in many ways. I only focus on react/redux related improvements and discussions, and so should anyone with a pull request. Please don't spend time on polishing any other parts.

###Demo app using React, Redux, Meteor

To install:
```
npm install
```

To run:
```
meteor
```

The app will run at `http://localhost:3000`


###Inspiration
This app is created to demo how we can use React/Redux with Meteor. The basic idea is to save data in the Minimongo to the redux store and use only the store to render UI.

It uses the modules below:
* `redux` store as the single data source for the UI components
* `react-redux` to `connect` the state tree with components and pass the store as context through `Provider`
* `redux-thunk` as the middleware for business logic like async calls, Meteor subscriptions, etc. It provides __dependency injection__
