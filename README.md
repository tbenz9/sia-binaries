# arm64 Binaries for Sia projects

This repository contains binaries related to the Sia project for the Raspberry
Pi and other arm64 based systems.  Simply download the binaries you're
interested in and run them directly on any 64bit ARM v8 or newer CPU.

These binaries work on Raspberry Pi 3 and 4 boards with a 64bit OS.

# Instructions
Download the binary of your choice
```
$> wget -O /tmp/siad https://github.com/tbenz9/sia-binaries/blob/master/linux_arm64/siad-1.4.1.1
```
Set the binary to executable
```
$> chmod +x /tmp/siad
```
Start running Sia!
```
$> /tmp/siad
Sia Daemon v1.4.1.1
Git Revision ✗-fa3a788c4
Loading...
(1/7) Loading siad...
(2/7) Loading gateway...
(3/7) Loading consensus...
(4/7) Loading transaction pool...
(5/7) Loading wallet...
(6/7) Loading host...
(7/7) Loading renter...
Finished loading in 1.373552476 seconds
```

## Limitations
Sia is only compatible with 64bit operating systems.

# Contributing
If there are other architectures or projects you'd like to see added to this
repository please open a GitHub issue and I'll try to add them.  If you maintain
a Sia project please feel free to open a PR that adds your binaries to this
repo.

# Troubleshooting
Remember that Sia requires a 64bit OS.  If you're using a 32bit OS you might
see the following message when you try to start Sia.
```
$> /tmp/siad
-bash: /tmp/siad: cannot execute binary file: Exec format error
```
