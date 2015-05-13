[![Build Status](https://travis-ci.org/ganskef/LittleProxy-parent.png?branch=master)](https://travis-ci.org/ganskef/LittleProxy-parent)

LittleProxy-parent is a container to build the Man-In-The-Middle extension in conjunction with [LittleProxy](https://github.com/adamfisk/LittleProxy). Now the dependencies should be found to automate within Travis CI.

Use LittleProxy-mitm with the following commands:

```
$ git clone git://github.com/ganskef/LittleProxy-parent.git --recurse-submodules
$ cd LittleProxy-parent
$ mvn clean install
$ cd LittleProxy-mitm/target
$ java -jar littleproxy-mitm-1.1.0-beta1-SNAPSHOT-shade.jar
$ curl -k -x localhost:9090 https://www.google.com/humans.txt
```
Please refer the documentation of [LittleProxy](https://github.com/adamfisk/LittleProxy) and [LittleProxy-mitm](https://github.com/ganskef/LittleProxy-mitm).

---------------
