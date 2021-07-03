# TorExitRelayExclude
Python script to exclude Tor exit relays with no contact info set.  Adapted from POC by nusenu for use with Tor Daemon on Debian.

Requires the following in /etc/tor/torrc

ControlSocket /var/run/tor/control GroupWritable RelaxDirModeCheck
UseMicrodescriptors 0

Must run after service is fully bootstrapped.
