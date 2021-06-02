# **How to Deploy a react App in Github Pages**

---

## Create react app

```cmd
~$ npx create-react-app brandmine
```



## Run the server

```cmd
~$ cd brandmine
~$ npm start
```

## Add Github Page Supports

```cmd
~$ npm install gh-pages --save-dev
```

## Modify `package.json`

```js
  "homepage": "http://brandmyself.github.io", //should be added and same as github link
  "name": "brandmine",                          //name of the project
   ...
  "scripts": {
    "predeploy": "npm run build",           //line 1 should be added
    "deploy": "gh-pages -d build",          //line 2 should be added
    ....
  }
  "devDependencies": {
    "gh-pages": "^3.2.0"
  }
```

## Git Initialization

```cmd
~$ git init
```

## Link Github Repo with this Git folder

```cmd
~$ git remote add origin https://github.com/brandmine/portfolio.git
```

## Show the status of git

```cmd
~$ git status
```

## Add all files to github

```cmd
~$ git add .
```

## Commit those added files

```cmd
~$ git commit -m "changes"
```

## Deploy React App

```cmd
~$ npm run deploy
```

## Push git files

```cmd
~$ git push -u origin master
```














