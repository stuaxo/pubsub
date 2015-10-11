Usage
=====

    import pubsub

    channel = pubsub.subscribe('channel')
    pubsub.publish('channel', 'hello world')
    channel.listen().next()    
    channel.unsubscribe()


Changelog
==========
* 0.1.2:
    * Updated to support Python 3
* 0.1.1:
    * Added channel unsubscribe helper: channel.unsubscribe()
    * Each published message now has a unique incrementing ID


Build status
============
[![Build status][ci-image]][ci-url]
[ci-image]: https://travis-ci.org/nehz/pubsub.png
[ci-url]: https://travis-ci.org/nehz/pubsub


The MIT License
===============

Copyright (c) 2012 Zhen Wang

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
