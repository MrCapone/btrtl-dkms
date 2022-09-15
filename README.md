# btrtl-dkms
bluetooth driver module for linux kernel older than 4.18

# Build and install with DKMS

DKMS is a system which will automatically recompile and install a kernel module when a new kernel gets installed or updated. To make use of DKMS, install the dkms package, which on Debian (based) systems is done like this:

```
sudo apt-get install dkms
sudo mkdir /usr/src/btrtl-0.2
git archive master | sudo tar -x -C /usr/src/btrtl-0.2
sudo dkms install btrtl/0.2
```
