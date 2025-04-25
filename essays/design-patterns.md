---
layout: essay
type: essay
title: Patterns with Purpose: Crafting Better Software
date: 2025-04-24
published: true
labels:
  - Design Patterns
  - 
---

<img width="200px" class="rounded float-start pe-4" src="../img/difficulty/degree_difficulty.jpg">

## Recipes in the Kitchen and in Code

Picture yourself in a busy kitchen. You're asked to make spaghetti, but you don't have a recipe to follow. You're trying your best to make the spaghetti based on your own knowledge, but you overcook the pasta and forget to salt the sauce. The meal ends up edible, but not the best. The next person who tries to cook the same dish will most likely have a different approach on how to recreate the dish, as well as make different mistakes.

In software development, this kind of problem always happens. Developers face problems that other before them have already solved, but without shared guidance as to how to solve that problem, everyone ends up reinventing the wheel.

Design pattern are the solution. They are the recipes for common problems in coding. Instead of fumbling through every new dish, you can follow the steps that others have tested and perfected. You can get clean and maintainable code. Design patterns help teams speak the same language, avoid issues, and help you write code more efficiently.

## One Chef per Station: The Singleton Pattern

In a real kitchen, having two chefs fighting over the same pan or burner is a recipe for disaster. If they both try to salt the soup or stir the sauce, a lot of wrong things could go wrong.

In software engineering, this happens a lot. With previous projects, I've had to build a login system for a web application that needed to connect to a database. At first, every part of my code had its own connection, which overloaded the system and caused bugs in the code. The solution to this was the Singleton pattern.

Singleton patterns makes sure that only one instance of a class exists. Like assigning one check to the pasta station, I used it to assign one database connection for the entire app. Everyone shared that one connection, which helped keep things efficient.

Using the Singleton pattern also made my code easier to manage and helped avoid the chaos of having multiple conflicting access points.

## Ordering a Dish: The Factory Pattern

Imagine going to a restaurant and saying, "I want pasta." You don't care if it's spaghetti or ravioli. You want the kitchen to figure it out based on the menu or what's available. 

In coding terms, the Factory pattern allows you to do that. I used it in a notification system. The app would send different types of notifications: email, SMS, or push. To do this, you can simply use if-else statements to figure out which to send. Another way to do this is the Factory pattern. The code could say, "Make a notification", then the class would create it based on what it is (email, SMS, or push).

## Why do patterns matter?

Design patterns don't just solve technical problems, but they help people work together better. Patterns keep projects in it's top shape because code that is built with patterns makes it easier to read, test, and change. You can think of this as a restaurant because it will run much smoother when everyone follows the same recipes. Generally, software engineers will thrive when they use shared patterns. For example, you wouldn't build a skyscraper without blueprints and good software isn't about writing code, it's mainly about using patterns that provide structure and clarity.
