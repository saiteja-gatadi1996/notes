1.	Full Stack development architecture


2.	Advantages of react
a)	React uses Virtual DOM
b)	React is a view library but not an entire MVC framework
c)	React follows uni-directional data flow
d)	React uses JSX
e)	React supports server-side rendering

3.	what is indexing in mongodb

i)	Indexes support the efficient execution of queries in MongoDB. 
ii)	Indexes are special data structures [1] that store a small portion of the collection's data set in an easy to traverse form. 
iii)	The index stores the value of a specific field or set of fields, ordered by the value of the field.

4.	advantages of context api over redux

iv)	It’s built into React and you therefore need no extra third-party dependencies - a smaller bundle and improved project maintainability
v)	You also don’t need a package like redux-thunk to handle asynchronous actions.

5.	why you use node as backend(reasons)

a)	Node.js is very efficient with real-time applications like chat, video, online gaming apps, ecommerce transactions.
b)	It facilitates handling multiple client requests, enables sharing and reusing packages of library code, and the data sync between the client and server happens very fast.
c)	Node’s ability to process many requests with low response times, as well as sharing things such as validation code between the client and server, make it a great fit for modern web applications that carry out lots of processing on the client’s side.
d)	For these reasons, Node.js is a popular choice among "single-page application" sites, where all the rendering is done on the client’s side, and the backend only provides a JSON API.
e)	Node.js also comes in handy, when you want to process high volumes of IO-bound requests. Historically, it wasn’t really that efficient if a lot of CPU processing was involved, mainly due to how your code is being run on a single-threaded process. 

6.	currying in javascript

Currying is a transform that makes f(a,b,c) callable as f(a)(b)(c) . JavaScript implementations usually both keep the function callable normally and return the partial if the arguments count is not enough

7.	semantics in html
![image](https://user-images.githubusercontent.com/42731246/151152867-5b40e0ac-f098-4477-b916-bd240b104b81.png)

 

8.	Doctype in html
![image](https://user-images.githubusercontent.com/42731246/151152848-dc86e18d-6fb4-4870-9d5f-4a9a112722b2.png)

 
If document type is not mentioned, browser will go to Quirks mode. Quirks mode depends upon the web browser version, If it is older version then this will not support HTML5 tags (Example: header tag, footer tag, section tag)

9.	Css: grid and its advantages

In CSS Grid Layout, rows and columns are really equivalent. You can place your element anywhere on your grid. You can span it across rows and columns, place it in a particular place, or rely on automatic placing.

10.	advantages of redux

11.	table row alternate color. how we can acheive using nth using Css

:nth-child(number) {
    // CSS Property
}

12.	How to switch web page n number of components using single button for dark mode or light mode


13.	While developing application, what all the security attacks you should be aware of

1: Injection flaws
2: Broken Authentication
3: Cross Site Scripting (XSS)
4: Insecure Direct Object References
5: Security misconfiguration
6: Sensitive data exposure
7: Missing function level access control
8: Cross Site Request Forgery (CSRF)
9: Using components with known vulnerabilities
10: Unvalidated redirects and forwards

14.	how will you design application before developing

 	Wireframe

15.	What are all the tools use for Ui design

          Blasmaiq, sketch, moqups, wireframe.cc

16.	redux flow
 ![image](https://user-images.githubusercontent.com/42731246/151152823-b9e5baa7-f7bc-4f1a-98cb-310c318b4227.png)


17.	how will you encrypt password

 ![image](https://user-images.githubusercontent.com/42731246/151152677-90f4522c-2127-4742-bbaa-a679d4fdfc8f.png)


18.	how will you improve screen reader

a)	Implement Consistent And Meaningful Content Hierarchies
b)	Include Skip Links
c)	Give Your Page A Meaningful Title
d)	Always Include Alt Text In Images
e)	Use Meaningful Anchor Text
f)	Organize Content From Top To Bottom

19.	how will you save password in database

20.	specificity in JS

If there are two or more conflicting CSS rules that point to the same element, the browser follows some rules to determine which one is most specific and therefore wins out.

The universal selector (*) has low specificity, while ID selectors are highly specific! 

21.	fragments in React

Fragments let you group a list of children without adding extra nodes to the DOM.

22.	Can we combine rest and destructuring in JS

23.	MongoDB to fetch the request fetched search

db.getCollection("COLLECTION_NAME").find({"createdAt":{$gt:new Date(Date.now() - 24*60*60 * 1000)}})
