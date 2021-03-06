
secret-hitler
======================

[![styled with prettier](https://img.shields.io/badge/styled_with-prettier-ff69b4.svg)](https://github.com/prettier/prettier)

Secret Hitler is a dramatic game of political intrigue and betrayal set in 1930's Germany. Players are secretly divided into two teams - liberals and fascists. Known only to each other, the fascists coordinate to sow distrust and install their cold-blooded leader. The liberals must find and stop the Secret Hitler before it’s too late.

Current production/stable is found at [Secret Hitler IO](https://secrethitler.io).

![Screenshot](http://i.imgur.com/6M56f6I.jpg)

Considering contributing to this project?  Please read our very brief guidelines found at ./CONTRIBUTING.md.  Contributors get a cool orange playername color!

Front end: React, Redux, Sass, Semantic UI, jQuery, SocketIO.

Back end: Node, Express, Pug, Passport, Mongodb with Mongoose, SocketIO.

Build: Gulp, Browserify, Babel (front end).

## Installation ##

Install node.js.  Production is on node LTS currently v6.11.0 and is recommended you use that for development.

Install mongodb, have it in your path.

Make a .env file, add the following to it:

> MONGOPORT={5 digit number here}

then

> git clone https://github.com/cozuya/secret-hitler.git

> cd secret-hitler

> npm i -g gulp nodemon

> npm i

## Running in dev mode ##

build assets (first time only):

> gulp build

start mongo:

> npm run db {your port here}

start express server:

> nodemon bin/dev

start development task runner:

> gulp

navigate to: http://localhost:8080

You'll most likely need a browser extension such as Chrome's openMultiLogin to have multiple sessions on the same browser.  No, incognito will not work.

## Running in production mode ##

I'll leave you to figure that out.  SH.IO is currently a $10/month digital ocean box using nginx, lets encrypt, and PM2.

## Tests ##

> npm test

## License and Attribution ##

Secret Hitler is designed by Max Temkin (Cards Against Humanity, Humans vs. Zombies) Mike Boxleiter (Solipskier, TouchTone), Tommy Maranges (Philosophy Bro) and illustrated by Mackenzie Schubert (Letter Tycoon, Penny Press).

This game is licensed as per the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/) license.

## Alterations to the original game ##

Minor image alterations and editing (from scans, assets available upon request).

Veto power is slightly adjusted so that chancellors need to select a policy prior to saying yes or no to vetoing that policy.

Adapted the rules explanation to account for online vs physical play.