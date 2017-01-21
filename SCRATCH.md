# Wanna to create from scratch? #

## Prepare MongoDB ##
Install and run MongoDB without auth. Please, [read here for more details](MONGODB.md).

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

## Add app.js ##
Create [app.js](nodejs/app.js) file, add the following lines to it

    var MongoClient = require('mongodb').MongoClient,
        assert = require('assert');

    // Connection URL
    var url = 'mongodb://127.0.0.1:27017/myproject';
    // Use connect method to connect to the Server
    MongoClient.connect(url, function(err, db) {
      assert.equal(null, err);
      console.log("Connected correctly to server");

      db.close();
    });

save file and exit from editor.

## Run app.js ##
Run in command-line/shell

    node app.js

After this the following line should be shown

    Connected correctly to server

## TODO ##
TODO
