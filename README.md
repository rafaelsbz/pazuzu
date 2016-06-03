# pazuzu
[![Travis BuildStatus](https://travis-ci.org/zalando/pazuzu.svg?branch=master)](https://travis-ci.org/zalando/pazuzu)
[![Coverage Status](https://coveralls.io/repos/github/zalando/pazuzu/badge.svg?branch=master)](https://coveralls.io/github/zalando/pazuzu?branch=master)

What is Pazuzu?
---------------
Pazuzu is a tool that builds Docker images from feature snippets, while
resolving all dependencies between them. One of the common use cases is
Continuous Integration environment, where jobs require specific tooling present
for building and testing. Pazuzu can significantly ease that process, by
letting user choose from a wide selection of predefined Dockerfile snippets
that represent those dependencies (e.g. Golang, Python, Android SDK, customized
NPM installs).

### Build
Make sure you setup Go acording to: https://golang.org/doc/install#install
```
go get -v
go build
```

### Usage

```
pazuzu -h
NAME:
   pazuzu - Build Docker features from pazuzu-registry

USAGE:
   pazuzu [global options] command [command options] [arguments...]

VERSION:
   0.1

COMMANDS:
     build	build docker image
     verify	verify docker image against

GLOBAL OPTIONS:
   --docker-endpoint value, -e value	Set the docker endpoint (default: "unix:///var/run/docker.sock")
   --help, -h				show help
   --version, -v			print the version
```

License
-------

The MIT License (MIT)
Copyright © 2016 Zalando SE, https://tech.zalando.com

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the “Software”), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
