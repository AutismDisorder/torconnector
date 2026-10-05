*torconnector* is a simple script that routes all OS traffic through TOR. It works with runit.

# Installation
```bash
git clone https://github.com/AutismDisorder/torconnector /tmp/torconnector
sudo mv /tmp/torconnector/torconnector /usr/local/bin
```

Simple as that. If you intend to spoof you mac address, then install maccahnger.

```bash
sudo xbps-install -S macchanger # for Void Linux  
```

```bash

$ torctl
--==[ torconnector by AutismDisorder ]==--

Usage: torconnector COMMAND

A script to redirect all traffic through tor network

Commands:
  start      - start tor and redirect all traffic through tor
  stop       - stop tor and redirect all traffic through clearnet
  status     - get tor service status
  restart    - restart tor and traffic rules
  autowipe   - enable memory wipe at shutdown
  autostart  - start torctl at startup
  ip         - get remote ip address
  chngid     - change tor identity
  chngmac    - change mac addresses of all interfaces
  rvmac      - revert mac addresses of all interfaces
  version    - print version of torctl and exit
```

Original:
https://github.com/BlackArch/torctl
