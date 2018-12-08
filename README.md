REOSC Network Intelligence API
============
[![Build Status][travis-image]][travis-url] [![dependency status][dep-image]][dep-url]

This is the backend service which runs along with reosc-node and tracks the network status, fetches information through JSON-RPC and connects through WebSockets to [reosc-netstats](http://stats.reosc.io) to feed information. For full install instructions please read the [wiki](https://github.com/REOSC).


## Prerequisite
* reosc-node
* npm

hi! 
## We would love to see your node working on stats page
    http://stats.reosc.io/

$ cd ~/

$ git clone https://github.com/My-Kings/reosc-api

$ cd eth-net-intelligence-api

$ npm install

## Now you must modify the file to connect to our stats server.

$ cd lib/node.js

## Find and Modify These Lines.

    Line 27: var WS_SECRET = "the_secret";

    Line 209: socket = new Socket( process.env.WS_SERVER || 'ws://stats.reosc.io:3001' );

## now run:
$ npm start
