- [OS Architecture](#os-architecture)
	- [Drivers](#drivers)
	- [Kernels](#kernels)
- [Notes about popular OS's](#notes-about-popular-oss)

# OS Architecture

Without going into detail, almost all ops have a similar architecture.

All programs run in [user space](https://en.wikipedia.org/wiki/User_space_and_kernel_space) and connect to the [kernel space](https://en.wikipedia.org/wiki/User_space_and_kernel_space) using the api methods.

There are manages in the kernel space managing all running programmes ([processes](https://en.wikipedia.org/wiki/Process_(computing)) & [threads](https://en.wikipedia.org/wiki/Thread_(computing))).
The [kernel](https://en.wikipedia.org/wiki/Kernel_(operating_system)) has the [resource management](https://en.wikipedia.org/wiki/Resource_management_(computing)) like:
- [processes](https://en.wikipedia.org/wiki/Process_management_(computing))
- [memory](https://en.wikipedia.org/wiki/Memory_management) 
- storages 
- ...

All of them are using [drivers](https://en.wikipedia.org/wiki/Device_driver) which manage the devices via interfaces


![](./basic_os_arch.jpg)



## Drivers

In computing, a device driver is a computer program that operates or controls a particular type of device that is attached to a computer or automaton.[1] A driver provides a software interface to hardware devices, enabling operating systems and other computer programs to access hardware functions without needing to know precise details about the hardware being used. [Read more...](https://en.wikipedia.org/wiki/Device_driver)

## Kernels

[Kernel](https://en.wikipedia.org/wiki/Kernel_(operating_system)) types:
 - [Monolithic](https://en.wikipedia.org/wiki/Monolithic_kernel)
 - [Micro](https://en.wikipedia.org/wiki/Microkernel)
 - [Hybrid](https://en.wikipedia.org/wiki/Hybrid_kernel)

![](./kernels_types.svg.png)


<!-- ### monolithic kernel structure:
- device tree
- drivers
- managers:
	- Memory
	- Process
	- virtual fs
	- IPC
	- IO
	- Network
- system call interface -->

# Notes about popular OS's
 - [UNIX-LIKE](https://en.wikipedia.org/wiki/Unix-like)
   - [Linux notes](./docs/oss/unix-like/linux/README.md)
   - [FreeBSD notes](./docs/oss/unix-like/bsd/README.md)
   - [MacOS notes](./docs/oss/unix-like/mac/README.md)
 - [Windows](./docs/oss/win/README.md)