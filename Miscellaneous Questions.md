1.	What is most difficult project you handled, please explain

I have worked on Ecommerce domain and I have involved developing both Node.js and React.js from scratch to deployment. In Ecommerce there are few important aspects as a developer we need to make sure are:

Authorization on all the subsequent requests(routes) that user make once logged in. This can be done with token-based authentication system.

In Ecommerce, 
1. To improve the performance of website, we have used Cloudflare CDN, React Router.
2. To improve the performance of web application (e-commerce) I will make sure to use smaller sizes of images
3. To improve the search engine performance, I will use debouncing
 
For Security:
1. HTTPS (adding secure socket layer to your website) SSL certificate
2. Http only (to avoid cross site scripting attacks)
3. Token based authentication for securing rest APIs

2.	What is your role in the project?

3.	What are the components in React?

4.	Which is better functional or class based?
Cannot say like that

5.	Is Redux for any other languages also

6.	How do we store data in Redux?

7.	What dispatch will do what action will do?

8.	What are stateless components in redux

9.	What is container and what it will do in Redux?

10.	What is a provider in Redux? 
The <Provider /> makes the Redux store available to any nested components that have been wrapped in the connect() function. Since any React component in a React Redux app can be connected, most applications will render a <Provider> at the top level, with the entire app's component tree inside of it.

ReactDOM.render(
  <React.StrictMode>
    <Provider store={store}>
      <App />
    </Provider>
  </React.StrictMode>,
  document.getElementById('root')
);

11.	What is global api in react

12.	Can we pass the value from child to parent?

13.	Can we set a state in render method?

14.	List view in React?

15.	How you set a background image in React

16.	What is a prop?
pass the data from 1 page to another page

17.	What are the types of components on which you worked?
    Both Functional and Class Components.

18.	What is a use state?

19.	Which is faster NODEJS or Quest?

20.	What is an event loop?

21.	How many phases event loop has?

22.	What is Async

23.	What is the difference between Call back hell and async?

24.	Promise vs async?

25.	How React works?

26.	Material-ui, data table?

27.	Props-drilling?

28.	What is ES6

29.	How can I write a text in HTML5?

30.	What is a promised based API?

31.	What is a flex box?

aims at providing a more efficient way to lay out, align and distribute space among items in a container, even when their size is unknown and/or dynamic (thus the word “flex”).

32.	What is a default direction of Flex?

    Row

33.	Grid and flexbox. 

The basic difference between CSS Grid Layout and CSS Flexbox Layout is that flexbox was designed for layout in one dimension - either a row or a column. Grid was designed for two-dimensional layout - rows, and columns at the same time.

## YouTube Interview questions:

1. How do you make configuration by using axios library so that some of the APIs get called with JWT token and some of them will not get called?

Ans: Server generates a token that certifies the user identity and sends it to the client. The client will send the token back to the server for every subsequent request, so the server knows the request comes from a particular identity.

2.  From Frontend we are going to call multiple APIs, how you will pass the token from frontend to backend? 

3.  How to create Protected Route?

4. A Page needs to be refreshed every 5 minutes (where you are going to use set Interval )

5.  If in the above page, we need a particular component needs to be refreshed (E.g.: About component, Home Component needs to be refreshed)

6. Any Form level components used

7. Features of React.js

10. How we achieve bi-directional flow in React?

12. React Fiber


13. How to copy an object in Javascript

Ans: let personObject = {
       firstName: "sachin",
       lastName: "goel"
}
let copyObject = personObject

14. positioning in css(which is the default position)
Ans: static

15. Differences between position absolute vs position relative 

16. inside <div> </div> element I have 4 <p></p> tags. For each <p> tag I need to display a $ icon. What is your approach?

17. Event Bubbling, 

18. Event Capturing

19. How many types of functions do we have in javascript?

21.  How do we update the state in react?

22. setState is synchronous or asynchronous

23.  After using setState, I want this setState to update a variable, will this work?

24. Why we need to write DOCTYPE?  Complete Syntax

25.  What is the box-model?


26. Lifecycle methods of React without Will methods (those where deprecated)

Ans:  Initial Render, Updates, Unmount

i) Initial Render: There are 2 lifecycles

getDerivedStateFromProps (old)

useEffect(()=>{},[prop1,prop2])  (new)

componentDidMount (old) this one runs only first time

useEffect(()=>{},[])  (new) , this one runs first time

ii) Updates:

getDerivedStateFromProps (old)

useEffect(()=>{},[prop1,prop2])  (new)

shouldComponentUpdate()   (old)

useMemo()

componentDidUpdate(old)

useEffect(()=>{})   (New)

getSnapshotBeforeUpdate (old)

custom Hook to hold previous state (new)

iii) Unmount

useEffect(()=>{return ()=>{//cleanup}}, [])

Error boundary
getDerivedStateFromError()  (old)
componentDidCatch()  (old) 
Currently nothing new

27. Pure Components and Impure components?

28. React render vs React hydrate?

29. How components interact each other? Other than props?

30. Jest and Enzyme

31. Styled Components in CSS

33.  While developing API's in Node.js, what are the security measures? (E.g: If I give the API's what is your approach)

34. What is JWT token and what it is doing?

35. How user come to know about token expire?

38.  Most challenging project in your career?

39.  How you deploy your code? QA and Production deployment? How QA will get the code?

40. What is the git command to push into particular repository

41. How to navigate between two pages?


44. How can I update Parent props from child? Ans: Props are immutable

45. A Array has 5 elements then I define  var B , if we assign B=A and if i change B[0]=5,  and now if we define console.log(A), what is the output? 

Ans [5, 2, 3, 4, 5]
-----------------------------------------------
46. what is Redux thunk?

Ans: Allows us to deal with Action Creators that can return action objects or functions.

47.  What difficulties you have solved in React.js?

48. What is the use of Key props? Ans: unique

50.  How to create props proxy for HOC?

54.  Which is good to use setState or componentWillMount

55.  Purpose of Redux?
Instead of mutating the state directly, you specify the mutations you want to happen with plain objects called actions. Then you write a special function called a reducer to decide how every action transforms the entire application's state.

56. Purpose of mapStateToProps and mapDispatchToProps?

As the first argument passed in to connect, mapStateToProps is used for selecting the part of the data from the store that the connected component needs. It’s frequently referred to as just mapState for short.
•	It is called every time the store state changes.
•	It receives the entire store state, and should return an object of data this component needs.
As the second argument passed in to connect, mapDispatchToProps is used for dispatching actions to the store. 
Providing a mapDispatchToProps allows you to specify which actions your component might need to dispatch. It lets you provide action dispatching functions as props. Therefore, instead of calling props.

57. Can I dispatch action in Reducer?
Dispatching an action within a reducer is an anti-pattern.
