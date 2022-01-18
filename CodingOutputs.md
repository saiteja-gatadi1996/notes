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

## 7. let i;

for (i = 0; i < 3; i++) {
setTimeout(()=>console.log(i), 100);

}

Ans: 3 3 3
Reason: in for loop i acts as global scope

## 8. function sum(a,b,c){

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