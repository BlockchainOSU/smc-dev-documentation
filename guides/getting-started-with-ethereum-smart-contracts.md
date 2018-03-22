# Getting Started with Developing Ethereum Smart Contracts


## Overview

This will be a guide to get you up and running with the truffle testing enviornment, the ganache private ethereum network, reactjs, and developing smart contracts.

Truffle is the development suite to help you build and test your smart contracts.
Ganache is the private network where you will deploy your smart contracts.

The web user interface will be created with reactjs. We will use `npm` to manage react packages and truffle packages.

All of these tools have pretty good documentation.

  - [Solidity Documentation for getting started with Smart Contracts](http://solidity.readthedocs.io/en/latest/)
  - [Truffle Documentation Exists for the Development Suite](http://truffleframework.com/docs/)
  - [Truffle has Step-by-Step tutorials](http://truffleframework.com/tutorials/)
  - [Reactjs Documentation](https://reactjs.org/docs/hello-world.html)
  - [Reactjs Tutorial](https://reactjs.org/tutorial/tutorial.html)
  - [NPM package manager](https://docs.npmjs.com/)



## Installation


### Installing Truffle

[TruffleSuite](http://truffleframework.com/) is the most popular development framework for Ethereum with a mission to make your life a whole lot easier.

  - [Truffle Installation](http://truffleframework.com/docs/getting_started/installation)
  - [Windows Configuration](http://truffleframework.com/docs/advanced/configuration#resolving-naming-conflicts-on-windows)
  - [Installing Node](https://docs.npmjs.com/getting-started/installing-node)

Truffle's installation is as easy as `npm install -g truffle` from a command line. 
For this to work, you will need `npm`, the node package manager (make sure to have all the dependencies as well). 
[Node can be downloaded here.](https://nodejs.org/en/download/)

After you have node installed, you should be able to install truffle with the command listed above.

### Installing Ganache

[Ganache](http://truffleframework.com/ganache/) is a quick way to fire up a personal Ethereum blockchain which you can use to run tests, execute commands, and inspect state while controlling how the chain operates. 
It is also part of the TruffleSuite.

You can download the ganache tool which comes with a pretty User Interface, or you can do what I do which is run a docker container and use the command line to run your test network with [ganache-cli](https://github.com/trufflesuite/ganache-cli). 
I highly reccommend the downloadable User Interface.



## Setup

After you have everything installed you basically need 4 things to run at once to develop your contract application: 
  - your private ethereum network (usually on localhost:8545)
  - a truffle development environment
  - Node Enviornment with `npm start`
  - your IDE (Visual Studio Code because it supports `.sol` files) 
  - web browser.

The commands for this are:
  - `cd ~working directory~`
  - (next step may change depending on how you run your private network, but start your private ethereum blockchain)
  - `docker run -p 8545:8545 trufflesuite/ganache-cli:latest -a 10` (for me)
  - `truffle compile`
  - `truffle migrate`
  - `npm run start`


## Common Errors and Fixes

### Incorrect Port Numbers

Nodejs sometimes gives a description of the error on the website.

The most common error I run into is my `app.js` or my `src/utils/getWeb3.js` file is not using the correct port number for my private blockchain. 











