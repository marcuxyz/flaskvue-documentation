<h1 align="center">
  Connect the Flask with VueJS.
</h1>

<p align="center">
<img alt="GitHub top language" src="https://img.shields.io/github/languages/top/pacotei/flask-vuejs">
</p>

# Introduction

**Flask-VueJS** is an extension the provides framework to develop the frontend layer in VueJS easily. With a few commands you will have the front up and running.

## Installing Flask-VueJS

Install with `pip`  

    pip install flask-vuejs

 (assuming that a virtualenv was previously creates)

## Requirements


#### NodeJS & NPM 

Follow the instruction for your OS [here](https://nodejs.org/en/download/package-manager/) to install **NodeJS** and **NPM**

When the installation finishes you can check with:    
```sh
$ node -v
v13.12.0

$ npm -v
6.14.4
```


## Creating your first application

```sh
(.venv) $ flask vue init
``` 


That will be create an configurations necessary for development good with flask and vuejs.


## Installing dependencies

To install all dependencies you need run the command

```sh
(.venv) $ flask vue install
``` 
This means that all dependencies for vuejs and webpack will be installed and configured correctly.


## How to use compile and watch flags...

For use compile and watch flags, you can run some these commands.

for compile:
```sh
(.venv) $ flask vue compile
``` 

for watch:
```sh
(.venv) $ flask vue watch
```

**But, what does that mean?**

It means that when you run only the `flask vue compile command`, the **webpack** will compile your component files created for vue only once. That is, every time you make a change to the component or even create a new component you will have to run the command again.

If you don't want this to happen all the time, run the command `flask vue watch` so that the webpack is watching all the changes in the `frontend` directory layer. After this, open the new terminal tab and execute `flask run` for running application.