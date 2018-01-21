[→ switch to github.io version](https://pothos.github.io/papers/)

Some works done during computer science studies at FU Berlin, TU Berlin and KAIST.

2015-2018 Kai Lüke

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

PDF: [Design of a Python-subset Compiler in Rust targeting ZPAQL, Kai Lüke](http://pothos.blogsport.eu/files/2016/12/kailueke_bsc_thesis_zpaql_compiler.pdf)
HTML (pdf2htmlEX): [Design of a Python-subset Compiler in Rust targeting ZPAQL, Kai Lüke](https://pothos.github.io/papers/bsc_thesis_zpaql_compiler.pdf2htmlEX.html)

# Seminar Work
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

PDF: [Interaction Between the User and Kernel Space in Linux, Kai Lüke](http://pothos.blogsport.eu/files/2018/01/linux_userspace_kernel_interaction.pdf)
HTML (pdf2htmlEX): [Interaction Between the User and Kernel Space in Linux, Kai Lüke](https://pothos.github.io/papers/linux_userspace_kernel_interaction.pdf2htmlEX.html)

## Web Connectivity in Ghana: A Survey

**Abstract**

Starting from the research “Dissecting web latency in Ghana”
of *Zaki et al.* the field of Internet connectivity in Ghana is
explored and the different aspects like latency, DNS resolution times,
complexity of web sites, caching and prefetching, TLS/SSL, TCP and cellular network performance,
role of ISPs, Internet Exchange Points, are brought in relation.
Measurement approaches and tailored solutions for areas
with bad connectivity are listed. Possible ways of improvement are discussed.

PDF: [Web Connectivity in Ghana: A Survey, Kai Lüke](http://pothos.blogsport.eu/files/2015/07/web-connectivity-in-ghana-a-survey.pdf)
HTML (pdf2htmlEX): [Web Connectivity in Ghana: A Survey, Kai Lüke](https://pothos.github.io/papers/web-connectivity-in-ghana-a-survey.pdf2htmlEX.html)
