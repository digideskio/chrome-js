Node-WebKit-REPL[![Build Status](https://travis-ci.org/o2platform/node-webkit-repl.svg?branch=master)](https://travis-ci.org/o2platform/node-webkit-repl)
==========

[![NPM](https://nodei.co/npm/node-webkit-repl.png)](https://nodei.co/npm/fluentnode/)

[![NPM](https://nodei.co/npm-dl/node-webkit-repl.png)](https://nodei.co/npm/fluentnode/)

**node-webkit-repl** is a collection of APIs and repls for [node-webkit](https://github.com/rogerwang/node-webkit)

**how to run (NOTE: these instructions and screenshots are a bit out-of-date with the latest version)**

```
git clone https://github.com/o2platform/webkit-repl-repl.git
cd webkit-repl
npm install 
```
as per documented at https://github.com/rogerwang/node-webkit/wiki/Chromedriver you need to download the chrome driver for your platform 
from http://dl.node-webkit.org/v0.11.2/ and copy it into the ```./node_modules/nodewebkit/nodewebkit``` folder.

In OSx the file to download is the ```chromedriver-nw-v0.11.2-osx-x64``` and you can open the folder to copy the unziped file using ```open ./node_modules/nodewebkit/nodewebkit```

Once that is in place you can start the version with chromedriver support using
```
coffee launch.coffee
```

... which should look like this:

![](https://cloud.githubusercontent.com/assets/656739/5246747/2af2d01c-7964-11e4-8747-3bdac1bda247.png)

and 

![](https://cloud.githubusercontent.com/assets/656739/5246763/60e65c2a-7964-11e4-8104-eaaa880d0460.png)

Note: in the current version, when you close the node-webkit window you will need to manually close the ```coffee launch.coffee``` process (since it is still running the
selenium server in the background)

If you want to just open the webkit-repl without chromedriver support, just run

```
./node_modules/.bin/nodewebkit 
```

... which should look like this:

![](https://cloud.githubusercontent.com/assets/656739/5246790/a68089ae-7964-11e4-9f0f-175cf9c3bc9c.png)

and

![](https://cloud.githubusercontent.com/assets/656739/5246824/e7fd8814-7964-11e4-8da4-8741b591885f.png)


**more script examples**
See these script examples to ideas on what to run there:  https://gist.github.com/DinisCruz/516417b0e70a2ba5e8bb#file-91-multiple-google-searches-js

**related issues**
[Is there a GUI REPL for node-webkit?](https://github.com/rogerwang/node-webkit/issues/2702)
