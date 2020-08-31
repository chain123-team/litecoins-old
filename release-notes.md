LiTeCoinS Core version 1.1.0.0
==========================

Release is now available from:

  <https://www.litecoins.tech/>

This is a new major version release, including various bug fixes and performance improvements, as well as updated translations.

Please report bugs using the issue tracker at github:

  <https://https://github.com/chain123-team/litecoins/issues>
 


Mandatory Update
=========================

How to Upgrade
--------------

If you are running an older version, shut it down. Wait until it has completely
shut down (which might take a few minutes for older versions), copy over litecoinsd on Linux.
If you upgrade after version 1.1.0.0 activation and you were
using version < 1.1.0.0 you will have to reindex (start with -reindex -chainstate
or -reindex) to make sure your wallet has all the new data synced. Upgrading from
version 1.1.0.0 should not require any additional actions.

Compatibility
-----------------

LiTeCoinS Core is tested on Ubuntu 16.04 Lts.

LiTeCoinS Core should also work on most other Unix-like systems but is not frequently tested on them.


Notable changes
===============

Performance improvements
------------------------
Slow startup times were observed in older versions. This was due to sub-optimal handling of old
deterministic masternode lists which caused the loading of too many lists into memory. This should be
fixed now.

Fixed excessive memory use
--------------------------
Multiple issues were found which caused excessive use of memory in some situations, especially when
a full reindex was performed, causing the node to crash even when enough RAM was available. This should
be fixed now.


Older releases
==============

LiTeCoinS tree 1.1.0.0 was a fork of Litecoin 0.15.1, original name was LiteCoin Coin
which was first released on Jan/13/2015.

LiTeCoinS tree 1.1.0.0 was the open source implementation of masternodes based on
the 0.15.1 tree and was first released on Oct/02/2020.
