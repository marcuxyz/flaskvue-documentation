# Commands

Guide on how to use the commands.


## Create

```sh
(.venv) $ flask vue init
``` 

## Install

To install all dependencies you need run the command

```sh
(.venv) $ flask vue install
``` 
This means that all dependencies for vuejs and webpack will be installed and configured correctly.


## Compile
Compile all components with output to static/main.js 

```sh
(.venv) $ flask vue compile
```

## Watch
Make the webpack listen to all the modifications of its components

```sh
(.venv) $ flask vue watch
```

## Restore
Restore application to factory default, removing **package.json**, **webpack.config.js**,
**package-lock.json**, **frontend and node_modules files**.

```sh
(.venv) $ flask vue restore
```