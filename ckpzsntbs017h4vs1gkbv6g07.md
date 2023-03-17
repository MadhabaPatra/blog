---
title: "Deploy Node.js on Firebase"
seoTitle: "Deploy Node.js on Firebase"
seoDescription: "Deploy Node.js on Firebase
Fully explained step by step to deploy your node(express) application on firebase"
datePublished: Wed Jun 16 2021 18:10:41 GMT+0000 (Coordinated Universal Time)
cuid: ckpzsntbs017h4vs1gkbv6g07
slug: deploy-nodejs-on-firebase
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1623858826595/BqS2jPGKF.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1623867147293/4CZKyqEq8.png
tags: hosting, deployment, firebase, nodejs, web-application

---

[Firebase](https://firebase.google.com/) is Google's platform that helps you quickly deploy your web apps, and provides NoSQL databases and file storage.

**You only need a** [**Gmail**](https://www.google.com/gmail/) **account.**

### Setup

1. Open the [firebase console](https://console.firebase.google.com/) and create a project.
    

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1623857080363/S3PNAViVC.png align="left")

1. Verify that you have installed the latest version of [NodeJs](https://nodejs.org/) in your system.
    

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1623857618348/XFW3pLWQX.png align="left")

1. After that, you need to install [Firebase CLI](https://www.npmjs.com/package/firebase-tools) on the terminal.
    

For *Windows* users

```plaintext
npm install -g firebase-tools
```

For *Linux* or *Mac* users

```plaintext
npm install -g firebase-tools
```

### Configure your firebase account

1. Open up the terminal and type
    

```plaintext
firebase login
```

1. Authenticate from the browser or click the generated link on the terminal.
    

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1623859242991/_GAFfrOv4.png align="left")

### Setting up firebase project on local

1. Initialize firebase project, open the terminal, and type
    

```plaintext
firebase init
```

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1623860295939/RutHzsB6-D.png align="left")

1. Move the cursor `↓` to ***Functions*** and `space` to select (\*) and hit `enter⏎`
    

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1623862338176/AfMlyob1e.png align="left")

Do the following little things.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1623862739198/DqwH9FmaQ.png align="left")

### Understanding the file structure

> Root folder

2.`functions` folder is created which is the project folder of our firebase application

3.`cd functions` to change the directory

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1623864175403/qqki8qyUJ.png align="left")

### Write Hello world project

1. Install [Express](https://expressjs.com/) inside the `functions` folder
    

```plaintext
npm i express
```

1. Delete the `index.js` file from the functions folder.
    

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1623864610475/WdUqm6b17.png align="left")

1. Create a file named `index.js` in the functions folder and open the file in any editor. 4. Write the following **hello world** program.
    

```plaintext
const functions = require("firebase-functions");
const express = require("express");
//  express app
const app = express();

app.get("/", (req, res) => {
  res.send("Hello World!");
});

//  export app to firebase functions
exports.helloWorld = functions.https.onRequest(app);
```

5.`cd ..` to go back to the root folder of firebase.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1623865175058/DoSvfAfst.png align="left")

### Setup firebase billing account

1. Upgrade to `Blaze plan`.
    

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1623865338036/yrmTZfMlA.png align="left")

1. Now you can deploy your application.
    

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1623865754455/D_SY0aq20.png align="left")

### Deploy

1. Go to the firebase project folder.
    

```plaintext
firebase deploy
```

1. Click the `Function URL`.
    

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1623866618377/Zi7yhwqvX.png align="left")

### Finished

That's it for today!

Hope you liked the post, if you’ve got any questions your can Mail us at madhabapatra@gmail.com.

Thanks