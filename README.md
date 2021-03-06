# Riak One Node Client Tester (Work in Progress)

A vagrant box containing an installation of the latest Riak (or Riak TS) build, installed and configured to provide you with a node on the same local machine. This script also provisions you the latest Basho supported Riak clients and a small sample script is downloaded to test for connectivity and esures that the client installation is configured correctly. (No more fumbling around trying to make the client installation work)

The premise of this is to get you up to speed in using Riak and developing stuff with the clients. Even if you have zero experience with a programming language, it will save you the frustration in downloading the client libraries and setting up dependencies. Provision the machine, edit the small test scripts and it just works.

Installing Riak and all of the clients and its dependencies from scratch would take around 45 mins. Running the box from power off after initialization would just be under a minute.

## Setup and Installation
Please make sure you have Vagrant installed.

```
git clone https://github.com/pogzie/riak-onenode-tester
cd riak-onenode-tester
vagrant up
```

## Riak TS Support
Riak TS support is experimental. You may set to install Riak TS (instead of Riak) via the config.cfg. It will create you a table based from the tutorial but I dont have any tests for it right now.

## Usage Notes
There is a short inline documentation on the source code for the riak-onenode-tester files which will help you debug or use the code properly.

## Todo
* DotNet client still needs some love
* Upgrade to Riak TS 1.5
* Riak TS test scripts
* Add a good list of Riak/Riak TS versions (commented) on the provisioning file so users would have the option to install older builds
* Update this from time to time since Basho Engineers are constantly updating client files and the Riak installer itself

## Updates
* 20170109 - Did some modifications to how NodeJS is installed. 
* 20161118 - Added support for Riak 2.2 including the new clients.

## Disclaimer
This code does not come with any warranty whatsoever. Do not blame the author for any untoward incident that happens to you, your family, your dog, or any of your property by using this code. Use wisely.

Despite this code being written by a Basho Client Services Engineer for the sole purpose of testing, this is not to be used in production environments and whatever is written here does not necessarily reflect the opinions of Basho as a company. You may freely distribute this with or without attribution since the world revolves around love and free stuff.
