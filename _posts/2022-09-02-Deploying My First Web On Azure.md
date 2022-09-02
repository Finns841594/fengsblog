---
toc: true
layout: post
description: I will recored all the problems I meet in this process of deployment, and solutions of them.
categories: [Notes]
title: Deploying My First Web On Azure
---

After finished the the problem set 9 "Finance" in CS50 course, I found this application for testing how good you can performance in stock market is worth sharing. So I decided to modify it and bring it online, so I can share this with my friends.

I encounterd several problems at the very first day. I will keep on updating this page for recording all the problems I meet, and all the solutions I found.

Here we go~

## 1. Hide the API_KEY

In the assignment, we need to register an API_KEY for checking the price of stocks at IEX. Everytime I run my finance program, I need to set the key as a environment variable(it takes me a while to get this). To not to modify the program too much, I find a way to set the environment variable in the program. But in this way, if I share my program online, for example on Github, all the people will see my API_KEY. I need to find a way to hide this.

## 2. Database

I decide to deploy this application on Azure servers from Microsoft. It is not so difficult to make it work, but here comes a problem about the database.

The database I used is SQLite, and it is part of the program which been uploaded with other files. I can register and trade successfully on the web, but I can not check the database like before, because there are no ways to access to the database file from the userside.