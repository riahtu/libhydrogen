[![Build Status](https://travis-ci.org/jedisct1/libhydrogen.svg?branch=master)](https://travis-ci.org/jedisct1/libhydrogen?branch=master)
[![Coverity Scan Build Status](https://scan.coverity.com/projects/13315/badge.svg)](https://scan.coverity.com/projects/13315)

![libhydrogen](https://raw.github.com/jedisct1/libhydrogen/master/logo.png)
==============

The Hydrogen library is a small, easy-to-use, hard-to-misuse cryptographic library for constrained environments.

Features:
- Consistent high-level API, inspired by libsodium. Instead of low-level primitives, it exposes simple functions to solve common problems that cryptography can solve.
- 100% built using just two cryptographic building blocks: the [Curve25519](https://cr.yp.to/ecdh.html) elliptic curve, and the [Gimli](https://gimli.cr.yp.to/) permutation.
- Small and easy to audit. Implemented as one tiny file for every set of operation, and adding a single `.c` file to your project is all it takes to use libhydrogen in your project.
- The whole code is released under a single, very liberal license (ISC).
- Zero dynamic memory allocations and low stack requirements. This makes it usable in constrained environments such as microcontrollers.
- Portable: written in standard C99. Supports Linux, *BSD, MacOS, Windows, and the Arduino IDE out of the box.
- Can generate cryptographically-secure random numbers, even on Arduino boards.
- Attempts to mitigate the implications of accidental misuse, even on systems with an unreliable PRG and/or no clock.

Non-goals:
- Having multiple primitives serving the same purpose, even to provide compatibility with other libraries.
- Networking -- but a simple key exchange API based on the Noise protocol is available.
- Replacing libsodium. Libhydrogen focuses on being small and is for environments where libsodium cannot be used.

# [Libhydrogen documentation](https://github.com/jedisct1/libhydrogen/wiki)

The documentation is maintained in the [libhydrogen wiki](https://github.com/jedisct1/libhydrogen/wiki).

# Warning
This is a work in progress.
