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

### 4. First Component

###### This is mentioned in the index.html file in public folder

```js
<div id='root'></div>
```

```js
import React from 'react';
import ReactDom from 'react-dom';

function Greeting() {
  return <h4> this is SaiTeja and this is my first component </h4>;
}

ReactDom.render(<Greeting />, document.getElementById('root'));
```

### 5. JSX Rules

![image](https://user-images.githubusercontent.com/42731246/159543496-b224585f-2690-48cd-b585-129012574a5a.png)

### 6. Children Prop

i) Component Book is now written in below format and we are inserting paragraph (p tag) at line 26 which is in between the Book component

```js
<Book></Book>
```

![image](https://user-images.githubusercontent.com/42731246/159547988-b3f1c590-2480-4318-b104-907bd7811e80.png)

To access the p tag, the Book Component should have a children prop like below

![image](https://user-images.githubusercontent.com/42731246/159548627-8ee13592-f041-4a5a-9dba-191b317ab21f.png)

![image](https://user-images.githubusercontent.com/42731246/159548776-af11b923-3d8e-43c7-a8c5-43c186be9044.png)

### 7. Event Basics

i) We can declare a clickHandler function (line 43) and use this function as a reference at (line 58)

ii) If we don't want to declare a function like clickHandler then we can directly write the logic by passing a callback function syntax like we did on (line 56)

Both i) and ii) works same

iii) In case if we are having any parameter in our function like ex: author is the parameter in the complexExample function (line 48) then in order to use this in onClick event we need to write this like we did on (line 61) which is passing a callback function (this runs during component loaded) and the reference function which actually works when we perform onClick.

![image](https://user-images.githubusercontent.com/42731246/159846195-a142a82e-a650-42c5-a227-f1dcc3a63ca6.png)

### 8. Import and Exports

i) Are the modules as part of ES6 (which are not react specific)
ii) Allows us to split up our app in small chunks which makes easier to manage our app in general

#### Default Exports:

```js
export default Greeting;
```

To import default export component, the syntax is like below (We can write any name apart from Greeting)

```js
import Greeting from './Greeting';
```

Ex:

```js
import Wishing from './Greeting';
```

#### Named Exports:

```js
export const Greeting
```

#### Named Exports must match the function naming which is Greeting:

```js
import { Greeting } from './Greeting';
```

#### Another Few examples of Default and Named Exports

##### Here we declared as Named Export on line 1

![image](https://user-images.githubusercontent.com/42731246/159847866-99fe703b-b957-40e9-802f-37461512ad32.png)

##### While importing this Named Export we should match the name with books

In our case we wrote as data in (line 7) and that is why browser failed to compile

![image](https://user-images.githubusercontent.com/42731246/159847926-f996626c-f74b-4654-abab-b30074c6171d.png)

##### For default export in this case, we need to write as export default books

##### import this as import books or any name from './books'

i) We only need to have one default export in a file which there can be any number of Named Exports in a single file

### 9. Advanced React

![image](https://user-images.githubusercontent.com/42731246/159848930-582c1a0e-6add-4f94-9ee6-d5cdd41c3c8c.png)

i) Basic Example of state change

If in our handleClick function we change the value of title, we observed that the Random Title naming is not changed to Hello People.

Now, the problem is that we are not rendering the component. So we change the value and we're not rendering the component. That's the reason why we cannot see any changes.

Now, the second thing is that we have no way to preserve this value in between the renders as well. So essentially, we would want two things.

We would want to keep the value between the renders, but also we would want to trigger that and this is where the useState comes into play, where it will allow us to do just that.

![image](https://user-images.githubusercontent.com/42731246/159856053-1230418f-4b79-4611-bf4d-2b5f3fcaa7a0.png)

### 10. Advanced React- useState

useState is a function

![image](https://user-images.githubusercontent.com/42731246/160236968-2f541e12-ad65-479d-981c-3a7ca8dc3f66.png)

on line 5, if we invoke this function, we would see that returns an array, and the first argument is actually a state value (at the moment it is undefined because we haven't passed a default value like a empty string or boolean or an empty array or empty object for example), and the second arg is the function which actually controls the value
![image](https://user-images.githubusercontent.com/42731246/160237205-c16aea74-4576-458d-9491-5de33516aa2f.png)

### Good example of useState

![image](https://user-images.githubusercontent.com/42731246/160237562-84e5a1c1-12bd-433c-99f3-2b5b01f189ec.png)

### General use of Hooks

i) a Hook should start with use

ii) a Component that use Hooks should start with Uppercase, otherwise it throws an error saying like

##### your component is neither a react function component or a custom React Hook function

iii) the hooks you are defining should be written inside the function body,

##### below is the wrong way of defining hooks

![image](https://user-images.githubusercontent.com/42731246/160237786-c83647dd-f269-4cbe-8589-5128052bef41.png)

![image](https://user-images.githubusercontent.com/42731246/160237612-1b785852-3c7a-4a2d-aa2a-d2edbd890905.png)

### useState Array Example

##### Data is an array and having objects and this is a named export.

![image](https://user-images.githubusercontent.com/42731246/160237991-01c234a5-ca50-4901-8aff-497a19588a43.png)

##### utilizing the data and holding the data value in people useState hook, now the people value holds the entire data (which was defined inside data.js),

##### we are iterating the people array using map (Higher Order Function) and destructuring the id,name from the person and returning the name

![image](https://user-images.githubusercontent.com/42731246/160237963-e1a4a9d0-c1e8-41a2-8b7a-2958bc7587e0.png)

##### a single button was created to clear items, as we are not referencing to a function and directly using the function (we need to pass a callback/arrow function to avoid running in a infinite loop, in our case data is an array, so to clear the data we need to pass the empty array)

![image](https://user-images.githubusercontent.com/42731246/160238220-7c0f7f89-d5ef-4d81-9871-575fb13036e2.png)

##### To only remove a singe person, we need to follow two approaches

i) Filter and show out (all the users) whose id doesn't match with the remove user id. (Read it twice).

This happens because we are using setPeople(newPeople) which holds latest value (that is filtered users).

In shorter terms: Our list will be filtered and shown without that removed user

ii) As we are passing a parameter inside the removeItem function, to use this in onClick we need to write like a (callback/arrow function) syntactical.

![image](https://user-images.githubusercontent.com/42731246/160238310-ca71ea3d-e070-4710-ad3b-320102db8286.png)

#### Another good way of re-writing function (functional approach)

![image](https://user-images.githubusercontent.com/42731246/160239773-f6f0951b-6929-4cc7-8918-5df48273055d.png)

### useState Object Example

Clearly observe that our person value is now object, so to change this we also need to pass an array inside setPerson function,

###### the reason we use spread operator was, we only want to disturb the message property and want to keep out the remaining properties as it is.

![image](https://user-images.githubusercontent.com/42731246/160238826-25960005-182f-4c9e-b0a5-a126f2df9e36.png)

###### we can also define in a separate hooks for name, age, message like we did below, and the good thing is now we can directy write setMessage and change the text message to whatever we need

![image](https://user-images.githubusercontent.com/42731246/160238930-6097f159-f85d-4c27-98fa-468f426c50bc.png)

#### Simple Counter Example using useState

![image](https://user-images.githubusercontent.com/42731246/160239237-2a4b4f48-fd38-4505-a290-3a5a5516cb55.png)

Added a new button which should increase the counter value after 2 seconds

##### IF we write like below (as we are holding the prevState value) this exactly holds our correct value (for Ex: If we clicked 10 times, it should update the value to 10). This is happening due to asynchronous way of handling the value due to setTimeout

##### If we click the button 10 times, it will only update once (if we use commented way of setValue(value+1) code)

![image](https://user-images.githubusercontent.com/42731246/160239864-03b39355-e7cf-4854-a952-432e9e71ac7d.png)
