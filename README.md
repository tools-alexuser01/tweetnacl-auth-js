HMAC-SHA-512-256 for TweetNacl.js
=================================

Implementation of <http://nacl.cr.yp.to/auth.html>
(requires [TweetNaCl.js](https://github.com/dchest/tweetnacl-js)).

Written in 2014 by Dmitry Chestnykh. Public domain.

[![Build Status](https://travis-ci.org/dchest/tweetnacl-auth-js.svg?branch=master)
](https://travis-ci.org/dchest/tweetnacl-auth-js)

Usage
-----


### nacl.auth(message, key)

Authenticates the given message with the secret key.
(In other words, returns HMAC-SHA-512-256 of the message under the key.)


### nacl.auth.full(message, key)

Returns HMAC-SHA-512 (without truncation) of the message under the key
