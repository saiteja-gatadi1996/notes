### Theory questions based on React and JS

- Redux state
- Async calls in Redux
- some other questions related to React

### Problem solving questions

- ##### Write a function to count the occurrence of each character in the input string.

  // Input: “abbcccd”
  // Output: a: 1, b: 2, c: 3, d: 1

  constraints: Use Array.reduce method to get the output

- ##### Write a function for the desired output as:

  // Input: sum(2)(3)()
  // Output: 5

  // Input: sum(2)(3)(4)()
  // Output: 9

- ##### Write a program to convert the below given input format into given output format

##### Input:
```js
{
   "user":{
      "name":"John",
      "tech":"Frontend",
      "address":{
         "home":{
            "add_1":"home_dummy_add_1",
            "add_2":"home_dummy_add_2"
         },
         "office":{
            "add_1":"off_dummy_add_1",
            "add_2":"off_dummy_add_2"
         }
      }
   }

```
##### Expected Output:
```js
 {
  user_name: 'John';
  user_tech: 'frontend';
  user_address_home_add_1: 'home_dummy_add_1';
  user_address_home_add_2: 'home_dummy_add_2';
  user_address_office_add_1: 'off_dummy_add_1';
  user_address_office_add_2: 'off_dummy_add_2';
}
```
