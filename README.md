TCPKTQ
==========

> work in progress!

My own implementation of TCP!

## Rationale

Inspired by @jonhoo's [live streaming](https://youtu.be/bzja9fQWzdA) of [Rust TCP implementation](https://www.github.com/jonhoo/rust-tcp). 

It is not an exhaustive implementation, but one that is enough to communicate with common-level TCP sockets.


## How it's implemented

### Low-Level API : linux TUN/TAP interface

There are many ways to access the network interface from the application process. We could use `pcap` API, or `pnet` crate that gives access to the raw sockets. However, we will use TUN/TAP interface for our use.


