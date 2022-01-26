1.	What is JSX?
JSX stands for JavaScript XML. JSX allows us to write HTML in React. JSX makes it easier to write and add HTML in React.

2.	
 

3.	What is SPA?
A single-page application does not require page reloading during use.
SPAs are all about serving an outstanding UX by trying to imitate a “natural” environment in the browser — no page reloads, no extra wait time. It is just one web page that you visit which then loads all other content using JavaScript — which they heavily depend on

4.	Render prop
The term “render prop” refers to a technique for sharing code between React components using a prop whose value is a function.

5.	ServiceWorker vs Web Worker?





6.	Lazy Loading?
It is a new function in react that lets you load react components lazily through code splitting without help from any additional libraries. Lazy loading is the technique of rendering only-needed or critical user interface items first, then quietly unrolling the non-critical items later.

lazy(() => import('./OtherComponent')); This will automatically load the bundle containing the OtherComponent when this component is first rendered. React. lazy takes a function that must call a dynamic import() .

7.	SEO in React?
Prerendering, Server Side rendering, Isomorphic React apps, Next.js

8.	D3.js?

9.	Reconciliation?
Reconciliation is the process through which React updates the DOM. When a component's state changes, React has to calculate if it is necessary to update the DOM. It does this by creating a virtual DOM and comparing it with the current DOM. In this context, the virtual DOM will contain the new state of the component.

10.	Testing libraries?

11.	Babel and Webpack?
Babel is a transpiler which it converts JSX to JS, 
Webpack is a module bundler

12.	Disadvantages of React?

13.	Super keyword?
super() will calls the constructor of its parent class. This is required when you need to access some variables from the parent class. In React, when you call super with props. React will make props available across the component through this.props .

14.	This keyword?
The JavaScript this keyword refers to the object it belongs to. ... In a function, this refers to the global object. In a function, in strict mode, this is undefined . In an event, this refers to the element that received the event. Methods like call() , and apply() can refer this to any object.

15.	Fetch vs Axios?

16.	 Render() vs return()
In react, render is a method that tell react what to display. return in a method or function is the output of the method or function

17.	PropsType?
PropTypes is a library that helps in minimizing this problem in React by checking the types passed in the props object against a specification we set beforehand and to raise a warning if the types passed don't match the types expected.

18.	Differences between Class Components vs Functional Components?

19.	Lifecycle methods in react javascript? Explain each and every?

20.	Correct sequence of constructor, render, componentDidMount, componentWillMount?

21.	What is the use of hooks?

22.	Some of the hooks and their example

23.	useCallback hooks usage


24.	What is HOC

25.	How to add one component in another
Ans: 
 

26.	 How to pass function (ex: addTodo) from Parent component to Child?

 

27.	 What is redux
Ans: Redux is state container that helps in storing the entire application state by avoiding prop-drilling.

28.	 What is store?
A store holds the whole state tree of your application. The only way to change the state inside it is to dispatch an action on it.
A store is not a class. It's just an object with a few methods on it. To create it, pass your root reducing function to createStore.

29.	 How to communicate both the Child elements without props?

30.	 Components of redux 

31.	 Principles of Redux?

a.	Single source of truth. The global state of your application is stored in an object tree within a single store. ...
b.	State is read-only. The only way to change the state is to emit an action, an object describing what happened. ...
c.	Changes are made with pure functions.

32.	Redux thunk middleware?

33.	 Difference between props and state
Ans: Both store information of the components but state is managed within the component whereas props is used to pass the data from parent to child component.

34.	 Is react support two-way binding.
Ans: React support Uni Directional data binding. i.e(from Parent to child), 

35.	What is ref in react?
Ans: Refs are a function provided by React to access the DOM element and the React element that you might have created on your own. They are used in cases where we want to change the value of a child component, without making use of props and all.

36.	 How to focus the filed when the component is loaded
Ans: 
 
 

37.	 What is the use of reducers?
A reducer is a function which takes two arguments — the current state and an action — and returns based on both arguments a new state

38.	 Can I have more than one store in one application
Ans: No, in redux

39.	 How to pass data from A to C
Ans: Declare C component in A component

40.	 What is context API
React's context allows you to share information to any component, by storing it in a central place and allowing access to any component that requests it (usually you are only able to pass data from parent to child via props).
41.	 Import vs required
Ans The major difference between require and import , is that require will automatically scan node_modules to find modules, but import , which comes from ES6, won't. Most people use babel to compile import and export , which makes import act the same as require .

42.	 Explain ES6 Features, 
1)	const and let keywords
2)	forEach, map, filter, every, some, find,
3)	Arrow functions
4)	Classes
5)	Enhanced Object literals
6)	Template strings
7)	Rest and spread operators
8)	Destructuring
9)	Promises


43.	 What is the use of Object Destructuring?
It's a JavaScript feature that allows us to extract multiple pieces of data from an array or object and assign them to their own variables.

44.	 How I can migrate from current React 15 project to React 16.8?

45.	Virtual DOM vs Shadow DOM?
Ans: Virtual DOM is creating a copy of the whole DOM object, and Shadow DOM creates small pieces of the DOM object which has their own, isolated scope for the element they represent.

46.	How to control the re- render cycle in react js
Ans: useMemo()- stores the state in cache and prevents unnecessary rerenders

47.	useMemo vs memo
Ans: Both memo and useMemo are used to memoize the result of a function, the only difference is memo is a HOC (and can be used to wrap both class and functional components) which useMemo is a hook (and can only be used inside functional components)
48.	 combineReducers?
The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore . The resulting reducer calls every child reducer, and gathers their results into a single state object.


49.	 What actually setState does in Class components?

50.	 Client-side rendering vs Server-side Rendering?

51.	 setState inside constructor?
setState" causes React to re-render your application and update the DOM. If you use setState in constructor you would get error like this:Can only update a mounted or mounting component. This usually means you called setState() on an unmounted component.
