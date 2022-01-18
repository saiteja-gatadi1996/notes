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

```js
> const name = "john"
> name // john
```

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

#### i) OS Module Examples

![image](https://user-images.githubusercontent.com/42731246/149820442-10ad6dc7-1594-43ba-a149-ba826c9e30c3.png)

##### Few other methods :

![image](https://user-images.githubusercontent.com/42731246/149820642-e1912518-24cf-4881-bad3-da6764a9544f.png)

#### ii) PATH Module Examples

![image](https://user-images.githubusercontent.com/42731246/149821213-3d57f5cb-6867-4eb0-88cb-eaa953e911cf.png)

##### Few other methods :

![image](https://user-images.githubusercontent.com/42731246/149821465-862dde43-655f-4b85-8fbd-ea320de450e1.png)

##### Output :

![image](https://user-images.githubusercontent.com/42731246/149821493-a1d22d7c-b2cf-41ee-80c3-301bc4756cd8.png)

##### Few other methods :

![image](https://user-images.githubusercontent.com/42731246/149821877-0efaa915-3e72-43a4-a3a7-da77c6be238a.png)

![image](https://user-images.githubusercontent.com/42731246/149821895-9af5148d-9ab9-4369-aa38-e64de73f280a.png)

#### iii) FS Module (Sync) Examples

![image](https://user-images.githubusercontent.com/42731246/149822521-c6555443-fb18-48f4-994d-b6d1c36d1467.png)

writeFileSync would create the file if doesn't exist, initially there was no file created with result-sync.txt, it gets created by node and the .txt file should have the result printed twice(due to the reason of flag object mentioned as append(a)).

![image](https://user-images.githubusercontent.com/42731246/149822726-65cb2446-86b5-4b70-8ad4-cad5b1aab8fa.png)

#### iv) FS Module (Async) Examples

![image](https://user-images.githubusercontent.com/42731246/149823297-788050e5-3594-494d-b221-32e1bd206502.png)

similarly write the code for reading the second file inside the call back

Ex:
![image](https://user-images.githubusercontent.com/42731246/149918682-b9a02f95-ff01-4c77-91dc-343b9e6678e5.png)

Now after reading both first and second, we are writing it to a new non-existing file like below

![image](https://user-images.githubusercontent.com/42731246/149919033-a21e9674-1942-4fb9-b84a-dbfc26e69e1c.png)

O/P:
![image](https://user-images.githubusercontent.com/42731246/149918880-3ab2d173-00e3-45fa-a340-0be89aedfb13.png)

##### --> Synchronous Programming:

Code gets executed line by line, no matter how much it takes time

Cons: Impacts the application when there are users hitting the app simultaneously

![image](https://user-images.githubusercontent.com/42731246/149921078-041defc9-baf0-458c-a1e8-58c110310723.png)

##### --> Asynchronous Programming:

Code doesn't waits for anything, this gets executed based on the least response time.

Ex:
(done with the task) is actually inside the writeFile module which usually takes some time to perform the write operations and then complete it and then log this message to the console. Meanwhile Async prints the next task (starting next task) and then it looks for another logs (for us there is only one remaining) and finally prints the done with the task

![image](https://user-images.githubusercontent.com/42731246/149922212-7444be7e-e08c-48c3-852e-0974665db017.png)

#### v) HTTP Module

![image](https://user-images.githubusercontent.com/42731246/149926011-a47b2741-534a-4145-ac5a-ffb69b278689.png)

##### We will see this below one only if the server keeps running (After entering node app.js (in the terminal, we don't see the exit)

![image](https://user-images.githubusercontent.com/42731246/149925952-66c853db-1832-47fe-834e-92268aa9d191.png)

##### Playing with req object

![image](https://user-images.githubusercontent.com/42731246/149927647-9f49966a-eb5b-4406-bc25-386f93a81284.png)

If you provide /about in the request it will showcase the 8th line.

Whereas if you try to provide something other it will be printing like below (there is not mandatory to provide error as a keyword, you can put anything that doesn't exist)

![image](https://user-images.githubusercontent.com/42731246/149927807-378e0596-b233-45ad-80a2-796536dc54af.png)

### 8. NPM (Node Package Manager)

![image](https://user-images.githubusercontent.com/42731246/149929037-b1bedc4f-d671-4652-9ca0-7f04b88fa09b.png)

![image](https://user-images.githubusercontent.com/42731246/149929305-73a14145-26dc-40a7-9a6f-00bb015e9501.png)


##### Install package as a dev-dependency(this package is not required when our application is deployed into production, only using this package for development purpose and makes no sense in Production)

![image](https://user-images.githubusercontent.com/42731246/149930692-ad46d0a3-ffc8-4beb-9971-daaa4c170796.png)

