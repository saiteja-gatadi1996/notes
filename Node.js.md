### 1. What exactly is Node.js

![image](https://user-images.githubusercontent.com/42731246/148641702-e6489a07-5e05-4d35-80a2-b9de2be26ad0.png)

### 2. Browser vs Node.js

![image](https://user-images.githubusercontent.com/42731246/148641801-db97750f-66b2-4bbb-adbe-ba6358eb8693.png)

### 3.

![image](https://user-images.githubusercontent.com/42731246/148687257-44f274f7-0a85-4e7c-b5c2-287773ddcb73.png)

![image](https://user-images.githubusercontent.com/42731246/148687290-6e6a3104-455d-4277-8366-42bc8da2660e.png)

### 4. How do we get node to evaluate code ?

##### i) REPL (Read-Eval-Print-Loop, just press node in the terminal and hit enter, you can write something similar to the Browser Console)

Ex:

> const name = "john"
> name (prints john)

![image](https://user-images.githubusercontent.com/42731246/149760220-5d29aa58-2d08-4036-b13e-454a862ad96e.png)

##### ii) CLI (Command Line Interface, which means running the Application code in Node)

### 5. Globals or Global variables in node

![image](https://user-images.githubusercontent.com/42731246/149764083-5efd9c72-6d28-4ef6-aa28-4d6b5ed7029a.png)

### 6. Modules in node

![image](https://user-images.githubusercontent.com/42731246/149765925-02b060be-b2f1-4b6f-a9ed-151b05258baa.png)

##### running the specific file name on terminal to see what module logs out, We have found that exports is print as object

![image](https://user-images.githubusercontent.com/42731246/149766102-3665baff-04ac-43bd-bf28-e0d31e3516bb.png)

##### module.exports is how we share the information from one file to another file and these constant variables are now can be accessed to another files

![image](https://user-images.githubusercontent.com/42731246/149766541-ef0472a6-0c78-4c84-9be4-4f8abfb8551b.png)

##### module.exports for function:

![image](https://user-images.githubusercontent.com/42731246/149767432-8902c678-7725-418e-9c38-4796b75fc034.png)

##### Code:

![image](https://user-images.githubusercontent.com/42731246/149767263-b93938ef-e097-4b6c-8d20-43520f1de2e1.png)

##### Alternative Syntax for module.exports

![image](https://user-images.githubusercontent.com/42731246/149768251-9ae1c18f-b46a-45fb-8693-9a23c3e5ab8a.png)

##### Whenver we try to log this 6th file in any of the file (ex: app.js) then we would see like below

![image](https://user-images.githubusercontent.com/42731246/149768161-fb7eba15-d2e9-44f1-8bb9-f7f35eba4cd7.png)

### 7. Built-in Modules

![image](https://user-images.githubusercontent.com/42731246/149769069-e5ce98be-b27b-4f99-a32e-38765d5073d0.png)
