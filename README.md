HUSH 1.0.8-1
=============

Zdash rebranded to HUSH on May 1st 2017

What is HUSH?
--------------

[HUSH] is a private implementation of the "Zerocash" protocol forked from [Zcash].
Based on Bitcoin's code, it intends to offer a far higher standard of privacy
through a sophisticated zero-knowledge proving scheme that preserves
confidentiality of transaction metadata. 

This software is the HUSH client. It downloads and stores the entire history
of HUSH transactions; depending on the speed of your computer and network
connection, the synchronization process could take a day or more once the
blockchain has reached a significant size.


**HUSH is unfinished and highly experimental.** Use at your own risk.

TEAM
----

Axel Karlsson: [@sparkit] Community manager, general communications.

Iolar Demartini Junior: [@demartini] Web Developer (Front End).

Joseph Stuhlman: [@joseph] Dev, general communications. 


* You can join our team and make contributions

Slack
-----
https://zdash-slack.herokuapp.com/ //invite


Building
--------

Build HUSH along with most dependencies from source by running
Get dependencies:
```{r, engine='bash'}

sudo apt-get install \
      build-essential pkg-config libc6-dev m4 g++-multilib \
      autoconf libtool ncurses-dev unzip git python \
      zlib1g-dev wget bsdmainutils automake
```

Install
```{r, engine='bash'}
#pull
git clone https://github.com/J-Stuhlman/zdash.git
cd zdash
# fetch key
./zcutil/fetch-params.sh
# Build
./zcutil/build.sh -j$(nproc)
# Run
./src/zcashd
```


Currently only Linux is officially supported.

Where do I begin?
-----------------
We have a guide for joining the main Zcash network:
https://github.com/zcash/zcash/wiki/1.0-User-Guide

### Need Help?

* See the documentation at the [Zcash Wiki](https://github.com/zcash/zcash/wiki)
  for help and more information.


License
-------

For license information see the file [COPYING](COPYING).
