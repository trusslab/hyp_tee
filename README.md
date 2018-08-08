
Saeed Mirzamohammadi, Ardalan Amiri Sani, "The Case for a Virtualization-Based Trusted Execution Environment in Mobile Devices
" in Proc. ACM SIGOPS Asia-Pacific Workshop on Systems (APSys), August 2018.

Link to the paper: ([PDF](http://www.ics.uci.edu/~saeed/Mirzamohammadi_APSys18.pdf)).

# People

* [Saeed Mirzamohammadi](http://www.ics.uci.edu/~saeed)
* [Ardalan Amiri Sani](http://www.ics.uci.edu/~ardalan)

In these instructions, we show how to set up the basic configurations for performing the measurements discussed in the paper.

# 1. Setup (Xen + CentOS on HiKey development board)

## 1.1 Compilation

Follow the instructions in this link to set up Xen and CentOS: https://github.com/Jeeppler/xen-note/blob/master/arm64/hikey/hikey-xen-centos.md.
We use linux kernel version 4.1 on android-hikey-linaro-4.1 branch and Xen version 4.9.0.
Download the Xen code from this link instead: 

```sh
git clone https://github.com/trusslab/hyp_tee_xen
```

In this repo, I added all the necessary scripts and config files to boot Xen correctly on HiKey which should be replaced with the ones used in the instructions.
Checkout the "pXen" branch to test Xen with optimizations.


## 1.2 Benchmark

Download the LMbench benchmark:

```sh
git clone https://github.com/trusslab/hyp_tee_lmbench
```

## 1.3 Note

Further commits might be added to further improve the performance of Xen, specifically on interrupts.
If there is any question, email me at: saeed@uci.edu

## 1.4 Acknowledgments

The work was supported in part by NSF Award #1617513.

