# Wanna to create from scratch? #

## Prepare MongoDB ##
[Read here](MONGODB.md)

## Create NodeJS directory ##
Run in command-line or shell:

    mkdir nodejs
    cd nodejs

## Create NodeJS project files ##
Run in command-line or shell:

    npm init

and set the following values for the appropriate keys:

Key             | Value
:-------------- | :-----------------------------
name            | nodejs-and-mongodb
version         | 1.0.0
description     | Play with Node.js and MongoDB
entry point     | index.js
test command    | TODO
git repository  | TODO
keywords        | TODO
author          | TODO
license         | MIT
                |
Is this ok?     | yes

As result the [package.json](nodejs/package.json) file will be created.

## Add dependencies to package.json - variant 1 ##
Edit [package.json](nodejs/package.json) file, add the following lines

    "dependencies": {
      "mongodb": "~2.0"
    },

before

    "author": "TODO",

line, save file, exit from editor and run in command-line/shell

    npm install

## Add dependencies to package.json - variant 2 ##
Or just run in command-line/shell

    npm install mongodb --save

## TODO ##
TODO
