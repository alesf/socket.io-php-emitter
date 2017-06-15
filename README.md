[![Build Status](https://travis-ci.org/ashiina/socket.io-php-emitter.svg?branch=master)](https://travis-ci.org/ashiina/socket.io-php-emitter)

### *Fork of ashiina/socket.io-php-emitter*

This is a fork of [rase-/socket.io-php-emitter](https://github.com/ashiina/socket.io-php-emitter).
If you have any questions or issues, please submit them there as this fork is not actively developed.

socket.io-php-emitter
=====================

A PHP implementation of socket.io-emitter.

## Changelist

### Emitting to multiple channels at once

This fork makes it possible to specify multiple channels to emit to in one call.
```
$emitter = new SocketIO\Emitter($redis);
$emitter
    ->in(['channel1', 'channel2', 'channel3'])
    ->emit('event', 'payload str');
```
