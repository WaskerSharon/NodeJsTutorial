# 0103 - NodeProject

- NodeJs is a JS runtime environment build on to of [Chrome V8](https://github.com/v8/v8) 
- NodeJs comes with several pre-installed packages.
- NodeJS packages are namaged using the **npm** - **N**ode **P**ackage **M**anager
- Additional packages can be installed globally and than they will be available for all node project or we can install locally which is the prefered way. 
- In Node project we distribue the list of the required packages along side with the src code.

### Creating NodeJS project
- Create new directory for your project
```bash
    mkdir nodeApp
```
- Log into this folder
```bash
    cd nodeApp
```
- Create the node project with the npm init command
```
    npm init

    package name: (scripts) nodeapp
    version: (1.0.0)
    description:
    entry point: (script.js)
    test command:
    git repository:
    keywords:
    author:
    license: (ISC)
    About to write to <path>\package.json:

    {
      "name": "nodeapp",
      "version": "1.0.0",
      "description": "",
      "main": "script.js",
      "scripts": {
        "test": "echo \"Error: no test specified\" && exit 1"
      },
      "author": "",
      "license": "ISC"
    }

    Is this OK? (yes)
```

- A New file named `package.json` was created.
- This file will contain the list of our dependencies

### Setting the script to be exexuted
- Add the following to the `package.json` under the `scripts`
```js
  "scripts": {
    ... 
    "start": "node script.js"
  },
```
### Running the srcipt
```js
   npm start
```

Now we should see our output in the console.