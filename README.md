[![Build Status](https://travis-ci.org/ganskef/LittleProxy-parent.png?branch=master)](https://travis-ci.org/ganskef/LittleProxy-parent)

LittleProxy-parent is a container to build the Man-In-The-Middle extension in conjunction with a patched version of [LittleProxy](https://github.com/adamfisk/LittleProxy) with additional offline features enabled. It's not longer needed to build the master branch of [ganskef/LittleProxy-mitm](https://github.com/ganskef/LittleProxy-mitm).

Use the `enable_offline_caching_with_mitm branches` of [LittleProxy](https://github.com/ganskef/LittleProxy/tree/enable_offline_caching_with_mitm) and [LittleProxy-mitm](https://github.com/ganskef/LittleProxy-mitm/tree/enable_offline_caching_with_mitm) with the following commands:

```
$ git clone git://github.com/ganskef/LittleProxy-parent.git --recurse-submodules
$ cd LittleProxy-parent
$ mvn clean install
$ cd LittleProxy-mitm/target
$ java -jar littleproxy-mitm-1.1.0-beta1-SNAPSHOT-shade.jar
$ curl -k -x localhost:9090 https://www.google.com/humans.txt
```
Please refer to the documentation of [LittleProxy](https://github.com/ganskef/LittleProxy) and [LittleProxy-mitm](https://github.com/ganskef/LittleProxy-mitm).

-----
