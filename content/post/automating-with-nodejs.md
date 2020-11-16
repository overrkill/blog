---
title: "Automating With Nodejs"
date: 2020-11-16T12:03:03+05:30
draft: false
tags: ['nodejs', 'automation', 'npm', 'script']
keywords: ['nodejs', 'automation', 'npm', 'script']
---
Table of Content
1. [Initializing](#init)
2. [writing the script](#script)
3. [Install globally](#global)(on your system😜)

Description  - setting up the environment to write scripts to automate tasks with nodejs and publishing to npm
part I - setup , hello world , testing locally 

#### Initializing <a name="init"></a>
*prerequisites*
- nodejs
- npm

create a folder for your project

cd to the folder -> do npm init

```bash
mkdir npm_script
cd ./npm_script
npm init -y
```
#### writing the script <a name="script"></a>
create an index.js file(starting point of your script)
##### adding the hashbang!

`#!/usr/bin/env node`

it specifies the the environment the script will run on

without hashbang
```
node ./filename.js
```
with hashbang
```
./filename.js
```
at this point your files would look like this
![added hashbang](https://dev-to-uploads.s3.amazonaws.com/i/g4z1l0n65b6pk6z238uq.PNG)

we would add some code to test our script
```javascript
const myAwesomeFunction = () => {
 console.log("Hello World")
}
```
which would look like 
![added hello world](https://dev-to-uploads.s3.amazonaws.com/i/ag6qgvvbml8d9clqi487.PNG)

*now we can test if our code runs*
by just typing
`./index.js`

#### installing the script globally <a name="global"></a>

```
npm install -g  // in your script directory
```

>now you can access the script anywhere on your system

**to be continued* (writing script to organize files, publishing to npm)
