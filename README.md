[→ switch to github.io version](https://pothos.github.io/papers/)

Some works done during computer science studies at FU Berlin (BSc), TU Berlin, and KAIST (Dual-Degree MSc).

2015-2019 Kai Lüke

# Master Thesis
## Memory-safe Network Services Through A Userspace Networking Switch

**Abstract**

A network service needs to be resilient against malicious input from the Internet.
Specially programs written in C are prone to memory corruption bugs which are the basis for remote code execution attacks.
Memory-safe languages solve this problem for application code running in userspace.
The TCP/IP network stack however runs in the operating system kernel, which is written in C and vulnerable to memory corruption.
Therefore, this work explored moving the TCP/IP stack into the memory-safe userspace process while providing a compatible API. The process should share an IP address with the kernel and integrate with the kernel's loopback interface. This solution keeps the benefits of a full-featured OS and does not impose different IPs per process or changes in the application logic.
I analyzed the requirements for deploying memory-safe TCP/IP services along with the kernel network stack.
The existing switching solutions for userspace network stacks do not meet these requirements because they do not handle untrusted packets in a memory-safe language and expose the kernel network stack to untrusted packets.
I present a memory-safe L4 software switch that connects multiple userspace network stacks and the host kernel network stack.
The switch allows the kernel and userspace network stacks to share an IP address. It also firewalls the host kernel network stack while supporting outgoing connections for updates.
To make memory-safe userspace networking easily usable I developed a socket library for Rust. Its in-app TCP/IP stack provides the same socket API types as the standard library and is based on smoltcp.
The combination of a memory-safe userspace switch and userspace TCP/IP stack expands the memory-safety of existing Rust web services to the TCP/IP layer with low porting efforts.

PDF: [Memory-safe Network Services Through A Userspace Networking Switch; Kai Lüke](http://pothos.blogsport.eu/files/2019/01/msc_thesis_memory-safe_network_services_userspace_switch.pdf)

HTML (pdf2htmlEX): [Memory-safe Network Services Through A Userspace Networking Switch; Kai Lüke](https://pothos.github.io/papers/msc_thesis_memory-safe_network_services_userspace_switch.pdf2htmlEX.html)

Slides as PDF: [Slides](msc_thesis_memory-safe_network_services_userspace_switch_slides.pdf)

Slides as HTML (pdf2htmlEX): [Slides](msc_thesis_memory-safe_network_services_userspace_switch_slides.pdf2htmlEX.html)

Code: [usnetd on GitHub](https://github.com/ANLAB-KAIST/usnetd), [usnet_sockets on GitHub](https://github.com/ANLAB-KAIST/usnet_sockets)

# Bachelor Thesis
## Design of a Python-subset Compiler in Rust targeting ZPAQL

**Abstract**

The compressed data container format ZPAQ embeds decompression algorithms as ZPAQL bytecode in the
archive. This work contributes a Python-subset compiler written in Rust for the assembly language ZPAQL,
discusses design decisions and improvements. On the way it explains ZPAQ and some theoretical and
practical properties of context mixing compression by the example of compressing digits of π. As use cases for
the compiler it shows a lossless compression algorithm for PNM image data, a LZ77 variant ported to Python
from ZPAQL to measure compiler overhead and as most complex case a implementation of the Brotli algorithm.
It aims to make the development of algorithms for ZPAQ more accessible and leverage the discussion
whether the current specification limits the suitability of ZPAQ as an universal standard for compressed
archives.

PDF: [Design of a Python-subset Compiler in Rust targeting ZPAQL; Kai Lüke](http://pothos.blogsport.eu/files/2016/12/kailueke_bsc_thesis_zpaql_compiler.pdf)

HTML (pdf2htmlEX): [Design of a Python-subset Compiler in Rust targeting ZPAQL; Kai Lüke](https://pothos.github.io/papers/bsc_thesis_zpaql_compiler.pdf2htmlEX.html)

Code: [zpaqlpy on GitHub](https://github.com/pothos/zpaqlpy)

# Seminar Work

## Backward-edge Protection: Improvements on SafeStack and RETGUARD
*Leak-resistant cryptographic return address integrity*

**Abstract**

The integrity of return addresses pushed to the stack is
the oldest target of control flow attacks. No mainline
compiler offers defenses for attacks that find the position of the return address and replace its content with a
malicious target address. We study proposed solutions
of the last years and try to overcome their security and
compatibility problems. We present an accessible Clang
compiler wrapper which offers shadow stacks or cryptographic return address integrity. Future x86 or ARM
processors will enable the kernel to provide hardware
shadow stacks (Intel) or fast pointer authentification
(Qualcomm). But until then sensible applications with‐
out highest performance requirements can make use of
our software solution.

PDF: [Backward-edge Protection: Improvements on SafeStack and RETGUARD; Alexis Gacel, Ndeye Khady Ngom, Kai Lüke](https://pothos.github.io/papers/backward-edge_protection.pdf)

HTML (pdf2htmlEX): [Backward-edge Protection: Improvements on SafeStack and RETGUARD; Alexis Gacel, Ndeye Khady Ngom, Kai Lüke](https://pothos.github.io/papers/backward-edge_protection.pdf2htmlEX.html)

## Interaction Between the User and Kernel Space in Linux
**Abstract**

System calls based on context switches from user to kernel
space are the established concept for interaction in operating systems.
On top of them the Linux kernel offers various paradigms for communication and management of resources and tasks. The principles and
basic workings of system calls, interrupts, virtual system calls, special
purpose virtual filesystems, process signals, shared memory, pipes,
Unix or IP sockets and other IPC methods like the POSIX or System V
message queue and Netlink are are explained and related to each other
in their differences. Because Linux is not a puristic project but home for
many different concepts, only a mere overview is presented here with
focus on system calls.

PDF: [Interaction Between the User and Kernel Space in Linux; Kai Lüke](http://pothos.blogsport.eu/files/2018/01/linux_userspace_kernel_interaction.pdf)

HTML (pdf2htmlEX): [Interaction Between the User and Kernel Space in Linux; Kai Lüke](https://pothos.github.io/papers/linux_userspace_kernel_interaction.pdf2htmlEX.html)

## Web Connectivity in Ghana: A Survey

**Abstract**

Starting from the research “Dissecting web latency in Ghana”
of *Zaki et al.* the field of Internet connectivity in Ghana is
explored and the different aspects like latency, DNS resolution times,
complexity of web sites, caching and prefetching, TLS/SSL, TCP and cellular network performance,
role of ISPs, Internet Exchange Points, are brought in relation.
Measurement approaches and tailored solutions for areas
with bad connectivity are listed. Possible ways of improvement are discussed.

PDF: [Web Connectivity in Ghana: A Survey; Kai Lüke](http://pothos.blogsport.eu/files/2015/07/web-connectivity-in-ghana-a-survey.pdf)

HTML (pdf2htmlEX): [Web Connectivity in Ghana: A Survey; Kai Lüke](https://pothos.github.io/papers/web-connectivity-in-ghana-a-survey.pdf2htmlEX.html)
