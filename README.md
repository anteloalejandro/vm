# vm

Simple script to run a VirtualBox VM in headless mode and connect to it with SSH

## How to use

**Just change whatever you need, such as vm names, in the script itself.**

The scripts asumes you have the OpenBSD version of netcat installed (the default in Debian/Ubuntu).

By default, the script will add a rule to port-forward SSH conections to the port 2222 on the host if it's not set.
Then, it starts the vm in headless mode (if it isn't already), waits until the SSH server on the guest is running, and tries to log in.
