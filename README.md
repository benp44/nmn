## Network Monitor and Notifier (nmn)

Very simple utility that monitors for devices joining and leaving the networks connected to the host, and optionally shows desktop notifications for these events.

### How it works

nmn is basically a glorified method of running nmap repeatedly. nmn monitors which network interfaces are up, and for each available network, uses nmap to track when an IPv4 address on that network comes up or down.

### Installation and operation

Can be run from the terminal for typical usage, however can also be run in the background by adding to autostart etc.

```
git clone https://github.com/benp44/nmn.git
cd nmn
./nmn
```
