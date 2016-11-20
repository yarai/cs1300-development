# CS1300 Development Assignment Template

## Setup ##

### Clone Repository ###
Open up terminal, go to a folder where you want put this project and run 
`https://github.com/yarai/cs1300-development.git`

### Install Packages ###
In order to use React, we first need to install different external packages (aka javascript/css frameworks that other people wrote). I have already created a list of dependencies needed (in `package.json`) but you will need to install them into your local computer by doing the following:
`cd` into `src` folder
Run `npm install`
* If you do not have npm installed, you can download it from [here](https://nodejs.org/en/)

### Install Gulp ###
Gulp is "an automated task runner that runs in the background watching for changes to files in specified directories, then executing predefined tasks as a part of your build process." This probably doesn't make much sense, but basically in our code it takes the Reactjs code you write and compiles it into Javascript that the browser can read. It's constantly running in the background so whenever you make a change in the React file it'll update the javascript. To install this:
* Run `npm install gulp -g` (this -g means global so it will install it to your root)
Now just try running `gulp` inside `src`, you should see `using gulpfile` and a bunch of task being started and finished. You may notice that it is never stopping; this process will continuously run to watch for any changes you make.

## Developing ##
Now that you havve necessary dependecies setup, let's start making changes!
One important thing to note: **all changes you'll be making should be in `src/js` and `src/css`**

### Run Gulp ###
Whenever you are developing you MUST ALWAYS RUN GULP. If you don't, the changes you make won't show up in your browser. So when you are working on this project always do the following before you start:
* Open up a new tab on terminal



# Client #
```cd cs1300-development/src``` <- the main frontend source folder

```npm install``` <- downloads dependencies according to the package.json file

```./node_modules/gulp/bin/gulp.js ``` <- runs gulp

## Before you start developing ##



# Server #
There are two options for serving the site.

### Server - Static ###
```cd cs1300-development```

```python -m SimpleHTTPServer```` <- statically hosts the compiled html files 

