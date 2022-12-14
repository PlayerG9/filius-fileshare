# filius-fileshare
Decentralised filesharing in the local network

> This Project is currently under development is not usable yet

> This Program is currently developed for Linux based systems  
> Windows may be supported later on

# How does it work

Other users have access to the files you put into your filis folder

![how does this work](README.assets/how-does-it-work.jpg)

## In detail

If you create a new file. it's created in your filesystem.
But is accessible and editable by other users in the same system.
This means that you don't have all files of the others saved on your computer.
But as long as they are also running filius you can access them.

# Installation and running

## Installation

```commandline
user@PC:~$ git clone https://github.com/PlayerG9/filius-fileshare.git
user@PC:~$ ./filius-fileshare/scripts/setup
```

## Running

```commandline
user@PC:~$ /path/to/filis-fileshare/filius
```

# Technical Stuff

## File-System
[refuse](https://github.com/pleiszenburg/refuse) is a Python module implemented using [`ctypes`](https://docs.python.org/3/library/ctypes.html) that provides a simple cross-platform interface to:

- [libfuse](https://github.com/libfuse/libfuse)
- [FUSE for macOS](https://osxfuse.github.io/)
- [WinFsp](https://github.com/billziss-gh/winfsp)

# Communication

is based on the python socket library
the serialization is either done with the [msgpack](https://msgpack.org/) package
or the python-internal [marshal](https://docs.python.org/3.10/library/marshal.html) package
