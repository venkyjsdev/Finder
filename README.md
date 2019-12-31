# Finder

Finder is awesome tool for twitter community which let's you find the common friends between two different twitter accounts. 

---
## Requirements

Node.js, npm, [Twitter Dev Tools](https://developer.twitter.com/)

### Node
- #### Node installation on Windows

  Just go on [official Node.js website](https://nodejs.org/) and download the installer.
Also, be sure to have `git` available in your PATH, `npm` might need it (You can find git [here](https://git-scm.com/)).

- #### Node installation on Ubuntu

  You can install nodejs and npm easily with apt install, just run the following commands.

      $ sudo apt install nodejs
      $ sudo apt install npm

- #### Other Operating Systems
  You can find more information about the installation on the [official Node.js website](https://nodejs.org/) and the [official NPM website](https://npmjs.org/).

If the installation was successful, you should be able to run the following command.

    $ node --version
    v10.16.0

    $ npm --version
    6.9.0

If you need to update `npm`, you can make it using `npm`! Cool right? After running the following command, just open again the command line and be happy.

    $ npm install npm -g

## Installation

    $ git clone https://github.com/Venky33/Finder.git
    $ cd finder
    $ npm install (if this isn't work, use sudo npm install)
    $ npm start
   
## NOTE

 - You need to install the dependent packages(ref: package.json) to get up and running with the finder.
 - Add your twitter consumer and access token in config/default.json

## Routes

    app.get('/:source/:lookup', (req, res) => {
        friends.mutual(req, res)
    })

    app.get('/:type', (req, res) => {
        logs.read(req, res)
    })
