<!-- .slide: data-background="#000000" -->
## What is Block-Chain?

It is just a DB and it is immutable. DB has access with multiple users and they can only create new entries.

<!-- .slide: data-background="#000000" -->
## How block chain works?

No Idea, Let’s build ONE!!



<!-- .slide: data-background="#000000" -->

## Setting up the Environment

### Download and install all required Pre-requisites:

curl -O https://gist.github.com/arshpreetsingh/2e628aea04d8615766b2ce14de4e5888

Run the script:

./prereqs-ubuntu.sh

<!-- .slide: data-background="#000000" -->

## Installing the Development Environment

Essential CLI tools

npm install -g composer-cli

Utility for running a REST Server on your machine to expose your business networks as RESTful APIs:

npm install -g composer-rest-server

Useful utility for generating application assets:

npm install -g generator-hyperledger-composer

Yeoman is a tool for generating applications, which utilises generator-hyperledger-composer:

<!-- .slide: data-background="#000000" -->

npm install -g generator-hyperledger-composer

npm install yeoman-generator

npm install -g yo

<!-- .slide: data-background="#000000" -->

Install Playground
npm install -g composer-playground

<!-- .slide: data-background="#000000" -->
## Install Hyperledger Fabric
This step gives you a local Hyperledger Fabric runtime to deploy your business networks to.

In a directory of your choice (we will assume ~/fabric-tools), get the .zip file that contains the tools to install Hyperledger Fabric:
mkdir ~/fabric-tools && cd ~/fabric-tools

<!-- .slide: data-background="#000000" -->
curl -O https://raw.githubusercontent.com/hyperledger/composer-tools/master/packages/fabric-dev-servers/fabric-dev-servers.zip

unzip fabric-dev-servers.zip

<!-- .slide: data-background="#000000" -->
A tar.gz is also available if you prefer: just replace the .zip file with fabric-dev-servers.tar.gz1 and the unzip command with a tar xvzf command in the above snippet.

Use the scripts you just downloaded and extracted to download a local Hyperledger Fabric runtime:
cd ~/fabric-tools ./downloadFabric.sh

<!-- .slide: data-background="#000000" -->
## Start Hyperledger Fabric
Start the fabric:

./startFabric.sh

<!-- .slide: data-background="#000000" -->

## Generate a PeerAdmin card:

./createPeerAdminCard.sh

You can start and stop your runtime using ~/fabric-tools/stopFabric.sh, and start it again with ~/fabric-tools/startFabric.sh.

At the end of your development session, you run ~/fabric-tools/stopFabric.sh and then ~/fabric-tools/teardownFabric.sh. Note that if you’ve run the teardown script, the next time you start the runtime, you’ll need to create a new PeerAdmin card just like you did on first time startup.

<!-- .slide: data-background="#000000" -->

## Thank You
