### 1. What is Javascript?

JavaScript is a scripting language used to create and control the dynamic Web site content. So in the context of major building blocks of the Web, we have HTML which is responsible for the structure of our Web project and We have CSS for styling but with Javascript we can make a web page dynamic by allowing users to interact with it.

Ex Scenario: Filter users

### 2. Internal Javascript using script tag

![image](https://user-images.githubusercontent.com/42731246/167200450-663e21cd-e66f-4367-a9a5-5c436f35ae72.png)

### 3. External Javascript

![image](https://user-images.githubusercontent.com/42731246/167204971-0e1574df-6226-40ef-8afe-080f20db4f18.png)

### 4. Statements and Comments

- Statements are the set of instructions
- Comments are the code helper suggestions
- Comments are of two types
  i) Single Line
  ii) Multiline

![image](https://user-images.githubusercontent.com/42731246/167202896-9766f4aa-33ba-4849-9cce-fc09bc827ecb.png)

// are the single line comments and we do see this for every line

```js
/* for start and */ to end are multi line comments
```

![image](https://user-images.githubusercontent.com/42731246/167204813-8fbcbe37-77d6-4ddf-aa24-4f3ed635d3ba.png)

### 5. Variables declaration and assigning it later

![image](https://user-images.githubusercontent.com/42731246/167204455-887f4259-03ee-44bf-83e4-8b7a10cc48d7.png)

### 6. Variables and their naming Rules

- must start with letter, $, \_
- cannot start with number
- case sensitive (you cannot declare it as fullname and access it as Fullname)
- camelCase or underscore (is a good way of assigning the variables)
- we cannot use reserved keywords for variable naming

##### For Ex: You cannot do like below

![image](https://user-images.githubusercontent.com/42731246/167238535-409fc9d0-9878-415c-8f1b-1e8ee07444fd.png)

### 7. var, let, const

- var : Is being a traditional way of declaring the variables ever since the creation of JavaScript all the way back to 1995.

##### let and const are introduced as part of ES6 (ES 2015)

- let : Is being a traditional way of declaring the variables ever since the creation of JavaScript all the way back to 1995.

- const : Is being a traditional way of declaring the variables ever since the creation of JavaScript all the way back to 1995.

###### The main difference with var, let and const is the re-assigning the variables. With const, once assigned cannot be re-assigned

![image](https://user-images.githubusercontent.com/42731246/167238773-4c2e5a34-1ca7-4be0-9b05-6ec6fd1451d3.png)

### 8. Implicit Type Conversion

```js
Ex: 1

var name1 = 'John'
var name2 = 'James'
var sub1 = name1 - name2
console.log(sub1) // NAN (number type)

Ex: 2

var name1 = '10'
var name2 = '23'
var sub1 = name1 - name2
console.log(sub1) // -13 (Number type)

Ex: 3

var name1 = '10'
var name2 = '23'
var add1 = name1 + name2
console.log(add1) // 1023 (string type)

Ex: 4

var name1 = 10
var name2 = '23'
var add1 = name1 + name2
console.log(add1) // 1023 (string type)

Ex: 5

var name1 = 10
var name2 = '23'
var sub1 = name1 - name2
console.log(sub1) // -13 (Number type)
```

### 9. Data Types in Javascript
