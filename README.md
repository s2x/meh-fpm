meh-fpm -- Meh! fastcgi process manager
===========

Are you looking for a fastcgi process manager written in C/C++? 
It's mostly based on [chenyf/fcgid](https://github.com/chenyf/fcgid) but i also stealed some ideas from spawn-fcgi.
Now it only support multi-process model 

Features
===========

* Works as process supervisor
* Run as daemon
* Multi-process model
* Process/socket uid and gid settings (ony if run as root)
* Can listeon on port or socket 
* Minimal/maximal/spare process configuration
* Dynamic worker allocation based on load
* Command line/file configuration

Dependencies
===========

* Git for source download
* G++ compiler with support for C++11,
* boost library
* libfcgi++

On Debian based distributions just type:
<code>apt-get install g++ libfcgi-dev libboost-dev git</code>

Build
===========

```
git clone https://github.com/s2x/meh-fpm.git
cd meh-fpm
cmake .
make
```
To install type `make install`, if you want to build `.deb` package use `cpack`.


Usage
===========
  ./meh-fpm -h
  ./meh-fpm -c conf/fcgid.conf -p 11111 



