![c-bit](https://github.com/c-bit/c-bit/blob/master/c-bit.png)
C-Bit Core integration/staging tree
=====================================

[![Build Status](https://travis-ci.org/c-bit/c-bit.svg?branch=master)](https://travis-ci.org/c-bit/c-bit)

https://BTC-BIT.com

What is C-Bit?
----------------

C-Bit is an experimental new digital currency that enables instant payments to
anyone, anywhere in the world. C-Bit uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. C-Bit Core is the name of open source
software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the C-Bit Core software, see https://www.btc-bit.com

License
-------

C-Bit Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/c-bit/c-bit/tags) are created
regularly to indicate new official, stable release versions of C-Bit Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

The developer [mailing list](https://lists.linuxfoundation.org/mailman/listinfo/bitcoin-dev)
should be used to discuss complicated or controversial changes before working
on a patch set.

C-Bit IRC can be found on Freenode at #cbit

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](/doc/unit-tests.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`

There are also [regression and integration tests](/qa) of the RPC interface, written
in Python, that are run automatically on the build server.
These tests can be run with: `qa/pull-tester/rpc-tests.py`

The Travis CI system makes sure that every pull request is built for Windows
and Linux, OSX, and that unit and sanity tests are automatically run.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

### Add nodes to connection

addnode=144.202.48.183:39302
addnode=158.69.126.193:43023
addnode=158.69.248.93:8289
addnode=176.9.25.79:8289
addnode=5.9.14.199:8289
addnode=51.15.162.24:8289
addnode=95.95.58.37:59742
addnode=[2001:0:9d38:953c:c74:4d6:b356:cc47]:8289
addnode=[2607:5300:120:85d::]:8289
addnode=[2a01:4f8:150:2344::2]:8289
