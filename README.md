[![Build Status](https://travis-ci.org/litecoins-project/litecoins.svg?branch=master)](https://travis-ci.org/litecoins-project/litecoins)

https://litecoins.tech

LiTeCoinS Core integration/staging repository
=================================================

LiTeCoinS (LTS) is a sustainable cryptocurrency modeled after Satoshi Nakamoto’s vision for Bitcoin. It is a decentralized, peer-to-peer transactional currency designed to offer a solution to the problem posed by the exponential increase in energy consumed by Bitcoin and other proof-of-work currencies. Proof-of-work mining is environmentally unsustainable due to the electricity used by high-powered mining hardware. 
LiTeCoinS utilizes the Tier Protocol, an energy efficient proof-of-power algorithm inspired by LITECOIN, can be mined on any computer, and will never require specialized mining equipment. The Tier Protocol offers a simple solution to Bitcoin sustainability issues and provides a faster, more scalable blockchain that is better suited for daily transactional use.
Fast transactions featuring guaranteed zero confirmation transactions, we call it SwiftTX.
- Fast transactions featuring guaranteed zero confirmation transactions, we call it _SwiftTX_.
- An experimental digital currency that enables instant payments to anyone, anywhere in the world. 
- LitecoinS uses peer-to-peer technology to operate with no central authority: managing transactions and issuing money are carried out collectively by the network. 
- LitecoinS Core is the name of open source software which enables the use of this currency.

More information at [LiTeCoinS.Tech](https://www.litecoins.tech)

Please reach out at LiTeCoinS. help@litecoins.tech


LiTeCoinS Core integration/staging repository
=====================================

LiTeCoinS is a brand new digital currency that combines all the positive aspects of successful digital currencies, while taking into account their flaws and weak points.
The project brings tangible benefits not only to the digital world but also to the real one.


Coin Specs
=====================================
<table>
<tr><td>Name & ticker</td><td>LiTeCoinS</td></tr>
<tr><td>Consensus algorithm</td><td>PoW</td></tr>
<tr><td>PoW block reward</td><td>200 LTS</td></tr>
<tr><td>Estimated LiTeCoinS supply during POW</td><td>1,000,000,000</td></tr>
<tr><td>Premine</td><td>500,000,000 LTS</td></tr>
<tr><td>Blocksize</td><td>1 MB</td></tr>
<tr><td>Blocktime average</td><td>1 min (DGW3)</td></tr>
<tr><td>Number of transaction confirmations</td><td>6</td></tr>
<tr><td>Maturity</td><td>288 confirmations</td></tr>
</table>


Development Process
=====================================

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/litecoins-project/litecoins/tags) are created
regularly to indicate new official, stable release versions of LitecoinS Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

The developer [mailing list](https://groups.google.com/forum/#!forum/litecoins-dev)
should be used to discuss complicated or controversial changes before working
on a patch set.

Developer IRC can be found on Freenode at #litecoins-dev.

Testing
=====================================

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

Automated Testing
=====================================

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/test), written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

Manual Quality Assurance (QA) Testing
=====================================

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
=====================================

We only accept translation fixes that are submitted through [Bitcoin Core's Transifex page](https://www.transifex.com/projects/p/bitcoin/).
Translations are converted to LitecoinS periodically.

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.


License
=====================================

LitecoinS Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.
