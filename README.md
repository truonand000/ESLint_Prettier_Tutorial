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

You'll want to start by installing the **ESLint** and **Prettier** plugins to your **VSCode** editor.

Click on the "Extensions" icon located on the left vertical icon menu. Search and install "ESLint" and "Prettier". Photos of these extensions are posted below:

![extension_menu](./images/ExtensionsMenu.png)

![ESLintVSCode](./images/ESLintVSCode.png)

![PrettierVSCode](./images/PrettierVSCode.png)

Next, you will want to install the **ESLint** and **Prettier** packages to your npm project:

Make sure that your npm installation is up to date (Node.js (^10.12.0, or >=12.0.0)). Also, make sure that you are at the root of your project. In the command line at the root of your project directory, type in the command:

```javascript 
npm i -D eslint prettier eslint-plugin-prettier eslint-config-prettier eslint-plugin-node eslint-config-node
```

Let these packages install. Once they are done, you will want run the following command to install **ESLint** globally. You will only have to do this once:

```javascript
sudo npm i -g eslint
```

Now that ESLint is installed globally, we can initialize a configuration file for eslint that will be named `.eslintrc.json`. ESLint has a that walks you through making initial configurations to your `.eslintrc.json`, which can be executed by entering in the following command into your command line (make sure that you are still at the root of your project directory):

```javascript
eslint --init
```

ESLint init will take you through a set of questions. Select the following answers for each question:

```
How would you like to use ESLint?
- To check syntax and find problems

What type of modules does your project use?
- JavaScript modules (import/export)

Which framework does your project use?
- React

Does your project use TypeScript?
- No

Where does your code run?
- Browser AND Node (select both by keypressing 'a', then hit enter)

What format do you want your donfig file to be in?
- JSON

Would you like to install them now with npm?
- Yes
```
