# Prepare MongoDB #

## Install ##
TODO

## Add path to MongoDB bin dir ##
TODO

## Prepare data directory ##

### Windows ###
Run the following in command-line/shell:

    md c:\data\db

### Linux ###
TODO

## Run MongoDB server ##
Run the following in command-line/shell:

    mongod

### Run with additional options ###
Run the following in command-line/shell:

    mongod --help

For example, if you wanna run server without auth, please run:

    mongod --noauth

## Connect to MongoDB server ##
On Windows OS run the following in command line:

    mongo
