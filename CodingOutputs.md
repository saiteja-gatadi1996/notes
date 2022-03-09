## 1.

console.log(0.1+0.2==0.3) //false
console.log(0.1 + 0.2) // 0.30000000000000004

## 2.

‘use strict’;
(function(){
var a = b = 3;
})();

console.log("a defined? " + (typeof a! == 'undefined')); undefined! =='undefined';
console.log("b defined? " + (typeof b! == 'undefined')); true! =='undefined';

## 3.

function foo1()
{
return {
bar: "hello"
};
}

function foo2()
{
return
{
bar: "hello"
};
}
O/P: Both doesn’t return same(return keyword in foo2() acts like the end of the statement by assigning ;

## 4.

(function() {
console.log(1);
setTimeout(function(){console.log(2)}, 1000);
setTimeout(function(){console.log(3)}, 0);
console.log(4);
})();

O/p: 1 4 3 2

## 5. Will this work?

var x=10,y=11,
z=x+y;
O/p: Yes, this will work

## 6. find second largest number from Array

## 7.

let i;

for (i = 0; i < 3; i++) {
setTimeout(()=>console.log(i), 100);

}

Ans: 3 3 3
Reason: in for loop i acts as global scope

## 8. 

function sum(a,b,c){

    return a+b+c;

}

function sum(a,b){
return a+b;
}

var result=sum(1,2,3)
console.log(result); //3
Reason: Overriding

## ------------------------------------------------------

## 1. Prime Number

![alt text](https://user-images.githubusercontent.com/42731246/142737068-e44fd4f6-bcaa-4bcd-8877-02fc87bcb420.png)

## 2. Fibonacci

![alt text](https://user-images.githubusercontent.com/42731246/142737071-a6361b5c-f22c-4063-be79-f0aba66870e6.png)

## 3. Armstrong

![alt text](https://user-images.githubusercontent.com/42731246/142737076-63406336-d4e7-4745-bd13-3864ba8f6955.png)

## 4. Star pattern

![alt text](https://user-images.githubusercontent.com/42731246/142737082-e39bda74-694b-4b1c-bdb1-74c5e47067e2.png)
![alt text](https://user-images.githubusercontent.com/42731246/142737086-21951694-10a3-406a-b729-64b6e3323a1d.png)

![alt text](https://user-images.githubusercontent.com/42731246/142737090-43ab3984-dc3e-4e89-9974-60c7746effcb.png)
![alt text](https://user-images.githubusercontent.com/42731246/142737093-88975450-44bd-4d05-870e-e8ea5664eb14.png)

## 5. Fizzbuzz

![alt text](https://user-images.githubusercontent.com/42731246/142737101-b325b893-8fcc-4599-a9cb-a03681620d23.png)

## 6. Sort an float array

![alt text](https://user-images.githubusercontent.com/42731246/142737104-3226d003-513c-4cdd-8e3b-35fc619adb44.png)

## 7. Maximum and Minimum values

![alt text](https://user-images.githubusercontent.com/42731246/142737114-fbbb5a7f-7ba9-495b-8905-64f75b007a89.png)

## 8. Output as per the questions

![alt text](https://user-images.githubusercontent.com/42731246/142737118-1193f2c3-8e47-4fe7-a218-6fab385907cc.png)

## 9.

![alt text](https://user-images.githubusercontent.com/42731246/142737137-e5ef3dca-6caf-4779-93c5-b57f4850c009.png)

## 10.

![alt text](https://user-images.githubusercontent.com/42731246/142737142-305bb31e-d5fc-4dbb-a489-6e3203a3c409.png)

## 11.

![alt text](https://user-images.githubusercontent.com/42731246/142737148-891f1992-82e2-4752-a55d-59cc5523a2f4.png)

Output

![alt text](https://user-images.githubusercontent.com/42731246/142737151-320d4b41-8754-4b7e-b64e-83a4f83197e0.png)

## Add Function

![alt text](https://user-images.githubusercontent.com/42731246/142737161-14d6d336-870c-4340-b3d7-1b3828e657a5.png)

## 12. React Router Example:

![alt text](https://user-images.githubusercontent.com/42731246/142737167-66209883-e033-41dd-9d14-e04f54f492d2.png)

## 13. Palindrome

![alt text](https://user-images.githubusercontent.com/42731246/142737175-6267b973-398c-45e2-94a8-f9c179357d9d.png)

![alt text](https://user-images.githubusercontent.com/42731246/142737178-1dd8c547-439f-4fec-bffe-e2d909788267.png)

## 14. Count the duplicate number that has repeated more number of times

![alt text](https://user-images.githubusercontent.com/42731246/142737180-f7b2c61c-726b-43c8-9d91-291d5aff0bbf.png)

![alt text](https://user-images.githubusercontent.com/42731246/142737184-77289625-f001-4606-bf83-9068a3252ebe.png)

## 15.

Javascript is by default a synchronous

![image](https://user-images.githubusercontent.com/42731246/149968745-ec192ac9-2ba5-4ddf-8d0a-65d4f88d32b4.png)

using Browser API's to offload the tasks
![image](https://user-images.githubusercontent.com/42731246/149968037-2d87d91a-2666-4adf-a135-3873e833fb75.png)

## 16. setInterval keeps on running until we kill the process

![image](https://user-images.githubusercontent.com/42731246/149972934-d770c51d-22b3-4a49-85db-1b5db28a60a5.png)

## 17. listen is asynchronous so it keeps on running,

Every time you hit the request on the browser, you get that logged in as (request event)

![image](https://user-images.githubusercontent.com/42731246/149973561-26003a5b-e3c6-43b6-9e2f-728459bc5bff.png)

## 18.Blocking code in callbacks (async code),

Cons: Not only /about page will take time to load, but this now affects other page routes also getting blocked (Home page route)

![image](https://user-images.githubusercontent.com/42731246/149974975-7415bcff-3c8a-4887-9629-5e3b60c2e58f.png)

## 19

a=10;

console.log(a);

var a=20;

O/p:
![image](https://user-images.githubusercontent.com/42731246/151492687-63fd27a2-884e-4693-a412-2bda304522b3.png)

## 20

var obj1={type:"Fiat", model:"500", color:"white"};
var obj2 = obj1;
obj2.model= "600";
console.log(obj1);
console.log(obj2);

![image](https://user-images.githubusercontent.com/42731246/151492604-e45cf218-d91c-4afd-8be2-1cc28b6a249b.png)

## 21

let a=10;
let a=20;

![image](https://user-images.githubusercontent.com/42731246/151492543-669e6cdd-3443-4929-be10-1ce173521f80.png)

## 22

1 + "12"

## 23
0 - "10"

## 24
"11" + 1

## 25
"10" + -1

null === undefined

null == undefined


## 26

let a =10;

function func(){

console.log(a)

}


func()


## 27 
'use strict'

var a= 10

console.log(a

var a= 20

## 28 Without use strict
var a= 10

console.log(a)

var a= 20

console.log(a)

## 29

function func(a){
let fname = "Singh";
a()
}

func a (fname){



});

Ans:
function func(a){
let fname = "Singh";
a(fname) //pass
}

func a (fname){
console.log(fname)


});


## 30

let array = [1,1,3,6,5,6];
let result = [...new Set(array)];
console.log(result);


## 31

const a = "12";
a = 11
console.log(a);

## 32

const Employee = {
firstname: 'John',
lastname: 'Doe'
};
Employee.firstname = "Singh";
console.log(Employee.firstname);

## 33 CSS related

div, p

div+p

div p

div > p


## 34 sum of the even numbers (which has to be squared)

const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const evenNumbers = array
  .filter((item) => item % 2 == 0)
  .map((item) => item * item)
  .reduce((item1, item2) => item1 + item2);

console.log(evenNumbers);


## 35 What will this print ?
const filteredItems = array.filter(() => 0);
console.log(filteredItems);


## 36 Print the value based on the query params and second key value pair (&)

const url =
  "https://codesandbox.io/s/little-darkness-qsymi?file=/src/index.js:205-267&name=saiteja";

console.log(url.split("=") )


## 37

var objA = {prop1: 42};
var objB = objA;
objB.prop1 = 90;
console.log(objA)


## 38
(function() {
var objA = new Object({foo: "foo"});
var objB = new Object({foo: "foo"});
console.log(objA == objB);
console.log(objA === objB);
}());


## 39
for (var i = 0; i < 3; i++) {
setTimeout(() => console.log(i), 1);
}


## 40
for (let i = 0; i < 3; i++) {
setTimeout(() => console.log(i), 1);
}


## 41
var x = {name:10};
var y = {...x};
y.name=20


console.log(x);
console.log(y);


## 42 Exercise with React.js 

Create a search bar which:
1.Fetches data from an API : https://dummy.restapiexample.com/api/v1/employees

2. Display the search results that match the employee name typed in search bar (api should be called after a minimum of three characters typed in search bar)

3. On clicking any searched Employee name, take to a dummy page, pass that employee name to the URL which opens when you select from the searched results.

4. A cross mark to clear the search bar.



## 43
var a = 2;
a++;
console.log(a); // 3
const d = [1, 2, 3];
d.push(5);
console.log(d); // [1,2,3,5]
const b = 2;
b++;
console.log(b); // TypeError: Assignment to constant variable
const c = [2]; //nothing prints from this line
c[0]++;
console.log(c);



## 44

var a = b();
console.log(a);
var c = d();
function b(){
return c;
}
console.log(a);
var d = function(){
return b();
}
console.log


## 45

function a(){
for(var i =0; i<10; i++){
setTimeout(() => {
console.log(i)
}, i*1000)
}
}
a();


## Design this in less than 30 minutes
![image](https://user-images.githubusercontent.com/42731246/152519562-3d8001fd-f083-4e54-976c-8617519eeec4.png)

##
var myObject = {
    foo: "bar",
    func: function() {
        var self = this;
        console.log("outer func:  this.foo = " + this.foo);
        console.log("outer func:  self.foo = " + self.foo);
        (function() {
            console.log("inner func:  this.foo = " + this.foo);
            console.log("inner func:  self.foo = " + self.foo);
        }());
    }
};
myObject.func();

outer func:  this.foo = bar
outer func:  self.foo = bar
inner func:  this.foo = undefined
inner func:  self.foo = bar

##
function foo1()
{
  return {
      bar: "hello"
  };
}

function foo2()
{
  return
  {
      bar: "hello"
  };
}

## Output:
foo1 returns:
Object {bar: "hello"}
foo2 returns:
undefined 


## Output of the question

var output = (function(x) {  

delete x;  

return x;  

})(0);  

console.log(output); 


## How to empty an array
let a = [1, 6, 8, 9]

## only print defined values
let b = [1, 2, , 4, 5] 

output should be [1, 2, 4, 5]

## Remove duplicates
let c = [1, 2, 3, 2, 5, 3] 

## Nested Arrays
let a = [1, 2, [3, 4, [5, 6, [7, 8, [9, 10]]]]]; 

output should be [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

![image](https://user-images.githubusercontent.com/42731246/157431479-ca9028f4-596b-4541-9b53-e2cf67892cd6.png)




