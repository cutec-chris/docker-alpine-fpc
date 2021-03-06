[![Docker Stars](https://img.shields.io/docker/stars/frolvlad/alpine-fpc.svg?style=flat-square)](https://hub.docker.com/r/frolvlad/alpine-fpc/)
[![Docker Pulls](https://img.shields.io/docker/pulls/frolvlad/alpine-fpc.svg?style=flat-square)](https://hub.docker.com/r/frolvlad/alpine-fpc/)


FreePascal Compiler (fpc) Docker image
======================================

This image is based on Alpine Linux image, which is only a 5MB image, and contains
[FreePascal Compiler](http://www.freepascal.org/).

Download size of this image is only:

[![](https://images.microbadger.com/badges/image/frolvlad/alpine-fpc.svg)](http://microbadger.com/images/frolvlad/alpine-fpc "Get your own image badge on microbadger.com")


Usage Example
-------------

```bash
$ echo "begin writeln('Hello World'); end." > qq.pas
$ docker run --rm -v `pwd`:/tmp frolvlad/alpine-fpc fpc /tmp/qq.pas
```

Once you have run these commands you will have `qq` executable in your current directory and if you
execute it, you will get printed 'Hello World'!
