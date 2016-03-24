# Angular 2 Demo Project

View the ASP.NET 5 version which comes with a backend here: https://github.com/jmackay/angular2-demoproject-aspnetcore

**Please note**: This was created for use as a demo project for a 6hr workshop at Boise Tech Fest. *It is not an example of best practices* and was meant to be used for multiple examples of how the Angular 2 works compared with Angular 1.

Slides are available at https://goo.gl/EQoPMJ

This is an angular 2 demo with an example scrum type board and users.

## Requirements

1. VSCode or your favorite editor
2. NodeJS / NPM (install 4.4 from https://nodejs.org/)

## Setup Required

    git clone https://github.com/jmackay/angular2-demoproject-node.git

or download / unzip into your folder of choice

Navigate to the install directory in a command prompt 

> *TIP: You can open command prompt in that folder by **holding shift + right-clicking** the empty area and selecting the command prompt option if using windows*

    npm install

Open in VS Code and make sure all typescript files create their js files and map by running tsc.

    tsc

### Reading plain .json files - READ ONLY

I've included .json files for each api which you can use by modifying the data.service.ts file. This will not allow you to save information but will allow you to load it :)

You will need to go to `app/shared/services/data.service.ts` and change `useStatic` to `true`

### Using another backend

This will require you to DIY but you should be able to easily hook into other databases by using something like **Firebase** in `data.service.ts`

## Using the Demo Application

Run the project from command line it should open to localhost:##### by typing

    npm start

You will be able to view users, and add new cards. Please feel free to add more functionality (and submit pull requests if you want!).

To be able to actually save you will need to create a backend api instead of just using the .json files. I've created a asp.net mvc 5 version here: https://github.com/jmackay/angular2-demoproject-aspnetcore

We use [JS-Data](http://www.js-data.io/) to help us read and save data as well as tie our relationships back together very easily client side, to allow for a very rich experience.

## Disclaimer

Please note that things will change and break as both Angular 2. I'll try to keep the project updated with the changes, but no guarantees!