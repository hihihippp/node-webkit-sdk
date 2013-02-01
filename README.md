node-webkit SDK
===============

SDK for building installable node-webkit applications.

This is a set of tools to build cross-platform (currently Windows, Linux 32bit, Linux 64bit) applications.

## SDK

Install:

    git clone git://github.com/jsmarkus/node-webkit-sdk.git
    cd node-webkit-sdk
    ant sdk

Patience! It will download latest releases of node-webkit for all platforms and installjammer.

Create first project:

    ant create -Dtemplate=default -Ddir=/home/user/project1
    cd /home/user/project1

## Project

The following commands are run from your project's directory.

Pack nw-package:

    ant app.nw

Pack binaries for 32-bit Linux:

    ant bin.l32

Pack binaries for 64-bit Linux:

    ant bin.l64

Pack binaries for Windows:

    ant bin.win

Pack binaries for all platforms:

    ant bin.all

Configure installjammer project (still TODO):

    ant ij.conf.l32    #for linux 32bit
    ant ij.conf.l64    #for linux 64bit
    ant ij.conf.win    #for windows
