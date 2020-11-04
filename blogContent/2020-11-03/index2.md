---
date: "2020-11-03"
title: "How to deploy the Gatsby site to Github pages"
---

Gatsby new project <url>
Gatsby develop
Gatsby run build // you have your  local server

To Host on Github pages:
1. Create a new github repo //eg. with name = /my_blog




2. Add the following in gatsby-config.js
   module.exports = {
  pathPrefix: "/my_blog",
  }



3. Add the following in the package.json
{
  "scripts": {
    "deploy": "gatsby build --prefix-paths && gh-pages -d public"
  }
}

Back on terminal: 
npm install gh-pages --save-dev
git init
git add .
git commit -m "first commit"





git remote add origin <url>
git push
git run deploy

