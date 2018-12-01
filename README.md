# About this kernel module
This Linux Kernel Module send IPv6 multicast packet. Result of the working LKM (IPv6 packet) is presented on the next screenshot (produced by WireShark).

![alt text](https://github.com/dmytroshytyi/KERNEL-sk_buff-helloWorld/blob/master/sample.png "Screenshot 1")

# Description
In this repo you may find a small demo of the Linux Kernel Module (LKM) develloped for kernel 4.4.0-116-generic. It is sending udp packet with "Hello World" payload.

Use

```make``` 

and


```make clean```

to compile and clean the project in the cli of current directory.

To import/remove the module, type in the cli:

```insmod lkm.ko```

```rmmod lkm.ko```

When imported, the module will send 1 udp packet with helloworld payload multicasted on the link layer and using IPv6

LKM uses sk_buff in the Linux kernel

