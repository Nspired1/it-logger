# Practice with Redux - IT Logger

## Summary

This is a simple IT Department Logger app that is practice working with Redux, React, and React-Redux. It uses React for the UI, Redux for state management, React-Redux to connect the two, and JSON Server as a fake rest API for a server with full Create Read Update Delete (CRUD) for logs.

## Technology

- [React](https://reactjs.org/) Front end library
- [Redux](https://redux.js.org/) App state management
- [React-Redux](https://react-redux.js.org/) Library that connects React with Redux
- [Redux-Devtools-Extension](https://www.npmjs.com/package/redux-devtools-extension) Easier way to install the browser Redux dev tools
- [Redux Thunk](https://www.npmjs.com/package/redux-thunk) Allows asynchronous functions inside Redux actions to send http requests
- [JSON Server](https://www.npmjs.com/package/json-server) Fake rest API so you can focus on the frontend
- [Materialize CSS](https://materializecss.com/) CSS Framework like Material UI, but less code

## General Information

This app simulates an IT Department's internal tool. Users can create, update, and delete an IT log (task) and assign a technician to that task. Also, users can search for either IT log or technician with the Search Bar at the top of the app. Logs and technicians are saved by JSON Server in the db.json file to save data. This is from a React and Redux tutorial, which I used for practice working with Redux.

## Setup

Clone this repository, change directory into it, type `npm install`. To run both the front and back end type `npm run dev`. With the Concurrently library and run scripts in package.json file the React server and JSON server will run at the same time.

## Screenshots

![Screenshot1](/screenshots/screenshot1.png)

![Screenshot2](/screenshots/screenshot2.png)

![Screenshot3](/screenshots/screenshot3.png)

![Screenshot4](/screenshots/screenshot4.png)

## Deeper Dive

Redux isn't a long library (about 90 lines of code), but per its co-creator Dan Abramov, Redux is dense. Some of the concepts they used are difficult, but they wanted to make a capable state management library that was easier to use than Flux.

The biggest difference between Redux and Flux is that Redux has only one state object to manage datea, while Flux has many for different parts of state. For small/medium applications there are few issues. For large applications with many different states, it is difficult to synchronize and update all state objects. To simplify that, they created Redux.

However, recently Dan Abramov said the React Context API is updated and improved, so for many applications he recommends using Context. For bigger or more complicated application, he recommends Redux, but it is good to understand and know both.

Per Brian Holt in his Intermediate React v3 course, he recommended starting with Context, then if the need arises to transition to Redux. There is more boilerplate and more code with Redux, so Redux adds a layer of complexity to components, but it can manage more features.

And in Steve Kinney's Redux Fundaments, he emphasizes there are only 9 (NINE!) Redux methods. Redux does a lot of hard things, but simplified them down to basic methods. Much of the boilerplate code comes from React-Redux library connecting the two. This is a good class that splits Redux from the React-Redux library in an effort to teach Redux itself.

## Additional References

- [Dan Abramov: Fundamentals of Redux](https://egghead.io/courses/fundamentals-of-redux-course-from-dan-abramov-bd5cc867)

- [Frontend Masters: Redux Fundamentals, by Steve Kinney](https://frontendmasters.com/courses/redux-fundamentals/)

- [Frontend Masters: Intermediate React v3, by Brian Holt](https://frontendmasters.com/courses/intermediate-react-v3/)

## Contact

- repo created by Don Spire [Nspired1](https://github.com/Nspired1), email: don.spire1@gmail.com
