### 1. What is React?

##### Ans:

i) React is a Javascript library for building User Interfaces.

ii) Developed by Facebook in 2011.

iii) When it comes to react, it's all about components. And you can think of components as independent chunks of user interfaces. Components can be as small as one html element.

iv) In reality, we probably will avoid the one component, since it's somewhat defeats the purpose

v) You see, the benefit of the component is that you can build a bunch of independent, isolated and most importantly reusable user interfaces. You can build independent pieces of user interfaces, meaning changing logic or layout in one command will not break your whole up.

vi) So if you ever need to make some changes, you simply locate the component, apply the changes and all the instances will be automatically updated.

vii) You say behind the scenes react is using something called virtual dom, where only the component that needs to be updated is effective. And what's really cool, it's done without rendering the whole which in turn, of course, increases the speed of your final product and as a result, the user experience as well.

### 2. Webpack

![image](https://user-images.githubusercontent.com/42731246/159537443-eb97b9ed-18d0-4dcb-81e1-85d9e99e0469.png)

Essentially, Webpack works as a module bundler, the main features of Webpack would be bundling our resources, watching for changes and running Babel transpiler.

### 3. Babel

Babel is a JavaScript transpiler that converts the newest JavaScript into the good old JavaScript so we can use all the newest features of the JavaScript language. So think things like an spread operator, destructuring and all the other goodies that come with ES6. And behind the scenes babel will turn into ES5, which in turn will make sure that our app runs smoothly in the older browsers as well.
