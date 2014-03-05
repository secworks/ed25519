ed25519
=======
This is a hardware implementation of the ed25519 public key signature
system. The core is implemented in Verilog (2001).


## Introduction ##
The ed25519 public key signature system is used in Tor. As part of the
Cryptech project we want to support the ed25519 signing in the HSM.

The references used for this implementation are:
- [The DJB implementation and paper.](http://ed25519.cr.yp.to/index.html)
- [The NaCl on 8-bit AVR MCU project and paper.](http://cryptojedi.org/crypto/)

Daniel Cegielka Suggested using the OpenBSD signify tool as reference:

http://www.openbsd.org/cgi-bin/cvsweb/src/usr.bin/signify/
SRCS= signify.c
SRCS+= fe25519.c sc25519.c smult_curve25519_ref.c
SRCS+= mod_ed25519.c mod_ge25519.c
SRCS+= crypto_api.c
http://www.openbsd.org/cgi-bin/cvsweb/src/usr.bin/ssh/



## Status ##
***(2014-03-05)***

Implementation is almost started. Info collection and functional model
is being looked at.

