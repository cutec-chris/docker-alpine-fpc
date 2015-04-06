FreePascal Compiler (fpc) Docker image
======================================

This image is based on Alpine Linux image, which is only a 5MB image, and contains
[FreePascal Compiler](http://www.freepascal.org/).

Total size of this image is only 65MB!


Usage Example
-------------

```bash
$ echo "begin writeln('Hello World'); end." > qq.pas
$ docker run --rm -v `pwd`:/tmp frolvlad/alpine-fpc fpc /tmp/qq.pas
```

Once you have run these commands you will have `qq` executable in your current directory and if you
execute it, you will get printed 'Hello World'!