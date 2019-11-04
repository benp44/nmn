## Network Monitor and Notifier (nmn)

[![Build Status](https://travis-ci.com/benp44/nmn.svg?branch=master)](https://travis-ci.com/benp44/nmn)

A very simple utility that monitors for devices joining and leaving any/all networks connected to the host, and optionally shows desktop notifications for these events.

### How it works

nmn is basically a glorified method of running nmap repeatedly. nmn monitors which network interfaces are up, and for each available network, uses nmap to track when an IPv4 address on that network comes up or down.

nmn should handle networks going offline and online, stopping monitoring them if unreachable, and then restarting monitoring when connectivity is restored.

### Installation and usage

Can be run from the terminal for typical usage, however can also be run in the background by adding to autostart etc.

```
git clone https://github.com/benp44/nmn.git
cd nmn
./nmn
```

To run with notifications disabled, use the `--disable-notifications` flag.
