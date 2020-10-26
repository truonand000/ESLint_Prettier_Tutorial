# Adding ESLint and Prettier to your React/NPM Project
## CS5610 Web Development

### Introduction

**ESLint** is a popular NPM package that is used to check your Javascript code for possible syntax errors, and allows you to quickly reference rules through provided links that can help guide you to correct these errors. It also comes with a recommended extension for React code, which we will also make use of.

**Prettier** is an auto-formatting tool that gives you the option to automatically format code based on a set of style rules you supply it. In this tutorial, we will provide you a set of style rules that we will use for this class and will also show you how to configure ESLint to work in conjunction with Prettier to help point out to you places in your code where you might be violating any of these rules and give you the option of automatically correcting them.

The goal of these two packages is to standardize the "Clean Code" portion of your assignment grades, help teach you to follow specific Javascript style guide lines, and help you practice writing clean code. Of course, the style rules that are provided are unique to this class. There are many other style guides (like google, airbnb, and mozilla) that are much more detailed, but we have decided to only provide very basic rules for the sake of simplicity. This is by no means perfect, but it is a nice and easy way to start to standardizing code style for this class.

Starting with Assignment 2, this will be made as a requirement for your React Projects. We will be using these packages to check your style, and will mark you down for any **ERRORS** (red-underlined indications) that appear in your code. **WARNINGs** (yellow-underlined indications) will not be counted against you, but it is **HIGHLY** recommended that you correct these warnings.

### Getting Started

For this tutorial, we will need [**VSCode**](https://code.visualstudio.com/)  editor. Make sure that you have this editor downloaded and installed on your local machine.

Once you have that installed on your machine, go ahead and open your `React` project in the VSCode editor and open up a new integrated Terminal (From the menu bar, go to *Terminal* > *New Terimal*):

![vscode_start_screen](./images/vscode_start_screen.png)

You want to start by installing the **ESLint** and **Prettier** 

Make sure that your npm installation is up to date (Node.js (^10.12.0, or >=12.0.0)). Also, make sure that you are at the root of your project. In the command line, type in the command:

```javascript 
npm i -D eslint prettier eslint-plugin-prettier eslint-config-prettier eslint-plugin-node eslint-config-node
```

