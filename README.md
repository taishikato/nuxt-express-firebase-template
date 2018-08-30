# Nuxt Express Firebase Template

This is the template to create web applications with
* [Nuxt.js](https://nuxtjs.org/)
* [Express](http://expressjs.com/)
* [Firebase](https://firebase.google.com/).

## Directories
* functions: For Firebase Cloud Functions
* src: For Nuxt.js Project
* public: For Firebase Hosting

## How to use
First of all, you need to set your FIrebase project with Firebase CLI.  
After that, you have to install npm packages.
```shell
$ vue init ambitiouzzz/nuxt-express-firebase-template my-project
$ cd my-project
# install dependencies in src and functions with npm install Or yarn
```
Next, let's make your app work on your computer😙
```shell
$ cd src && yarn build
$ cd .. && mkdir public
$ cp -R functions/nuxt/dist/ public/
$ firebase serve --only hosting,functions
```

## How to deploy
```shell
$ firebase deploy --only hosting,functions
```
