# CS1300 Development Assignment Template

## Setup ##

### Clone Repository ###
Open up terminal, go to a folder where you want put this project and run\s 
`https://github.com/yarai/cs1300-development.git`

### Install Packages ###
In order to use React, we first need to install different external packages (aka javascript/css frameworks that other people wrote). I have already created a list of dependencies needed (in `package.json`) but you will need to install them into your local computer by doing the following:
* `cd` into `src` folder
* Run `npm install`
  * If you do not have npm installed, you can download it from [here](https://nodejs.org/en/)

### Install Gulp ###
[Gulp](http://gulpjs.com/) is "an automated task runner that runs in the background watching for changes to files in specified directories, then executing predefined tasks as a part of your build process." This probably doesn't make much sense, but basically in our code it takes the Reactjs code you write and compiles it into Javascript that the browser can read. It's constantly running in the background so whenever you make a change in the React file it'll update the javascript. To install this:
* Run `npm install gulp -g` (this -g means global so it will install it to your root)\s
Now just try running `gulp` inside `src`, you should see `using gulpfile` and a bunch of task being started and finished. You may notice that it is never stopping; this process will continuously run to watch for any changes you make.

## Developing ##
Now that you havve necessary dependecies setup, let's start making changes!\s
One important thing to note: **all changes you'll be making should be in `src/js` and `src/css`**

### Always Run Gulp ###
Whenever you are developing you MUST ALWAYS RUN GULP. If you don't, the changes you make won't show up in your browser. So when you are working on this project always do the following before you start:
* Open up a new tab on terminal
* `cd` into `src`
* Run `gulp`\s
Keep gulp running on this tab while you are developing.

### Making changes to React ###
To make changes to the React code you should first `cd` into `src/js`. There, you should see the file `index.jsx`. This will be your main React file that will take all the components and put the page together. Under the directory `components/`, you can create components that are relevant to your app (Dropdown, Filter, CardList, etc.)

### Making changes to CSS ###
To add style changes you can find `src/css` and find `main.css`.

### After making changes ###
After making changes in the `src` directory, always check back to the terminal tab that is running `gulp` as it will show you if there were any compiling error. If there are errors, go back to the source files, try to fix and check back on the terminal to see if it works. Keep repeating until everything compiles!

### Running a local server ###
Once you have made changes in your code and gulp successfully compiles, you can run a simple server to see your app in the browser. This can be done by using python's SimpleHTTPServer:
* `cd` back to `cs1300-development`
* Run `python -m SimpleHTTPServer`
  * This will create a server from the cs1300-development directory
* Now on your browser, go to localhost:8000 to see your app!

## More Resources ##

### React ###
https://facebook.github.io/react/docs/thinking-in-react.html

## For the curious ##
Here are some more technical things about this repository in case you are curious.
