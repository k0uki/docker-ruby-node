# Ruby + Node Docker Image

Docker image with Ruby and Node.js with Yarn installed and ready to roll.

And installed library for major gems.(e.g. nokogiri)

Run Rails App out of the box.

Maintaned combinations:

- Ruby: 2 (2.6.5) Node: 10.x (10.16.3)

## Why Node.js and Ruby together?

Some applications, like Jekyll, GitHub pages or Rails with Webpacker, requires both Ruby and Node.js
installed in the same image in order to run or fully function. This image do not install any other packages than both other images do.

## Differences with official Ruby and Node.js images?

Ruby: Same as official.

Node: Instead variables NODE_VERSION and YARN_VERSION is available variable NODE_MAJOR fullfiled with major version of node.js. Node is not executed on by CMD.

## How to use this image

```
$ docker run -v "$PWD":/usr/src/app -p "8080:8080" k0uki/ruby-node
```

## Default Locale

Versions 2-6, 2-8, 2-10 has defined locale C.UTF-8 instead default POSIX.

## License

This Docker image is licensed under the [MIT License](https://github.com/k0uki/docker-ruby-node/blob/master/LICENSE).

Software contained in this image is licensed under the following:

- Ruby: [GPLv2](https://github.com/ruby/ruby/blob/trunk/GPL)
- Node.js: [MIT License](https://github.com/nodejs/node/blob/master/LICENSE)

## Supported Docker versions

This image is officially supported on Docker versions v17, v18.

Support for older versions (down to v1.0) is provided on a best-effort basis.

## User Feedback

### Documentation

- [Docker](http://docs.docker.com)
- [Ruby](https://www.ruby-lang.org/en/)
- [Node.js](https://nodejs.org/en/)