
# Bachelor Thesis
## Design of a Python-subset Compiler in Rust targeting ZPAQL

**Abstract**

The compressed data container format ZPAQ embeds decompression algorithms as ZPAQL bytecode in the
archive. This work contributes a Python-subset compiler written in Rust for the assembly language ZPAQL,
discusses design decisions and improvements. On the way it explains ZPAQ and some theoretical and prac-
tical properties of context mixing compression by the example of compressing digits of π. As use cases for
the compiler it shows a lossless compression algorithm for PNM image data, a LZ77 variant ported to Python
from ZPAQL to measure compiler overhead and as most complex case a implementation of the Brotli algo-
rithm. It aims to make the development of algorithms for ZPAQ more accessible and leverage the discussion
whether the current specification limits the suitability of ZPAQ as an universal standard for compressed
archives.

# Seminar Work
## Web Connectivity in Ghana: A Survey

**Abstract**

Starting from the research “Dissecting web latency in Ghana”
of *Zaki et al.* the field of Internet connectivity in Ghana is
explored and the different aspects like latency, DNS resolution times,
complexity of web sites, caching and prefetching, TLS/SSL, TCP and cellular network performance,
role of ISPs, Internet Exchange Points, are brought in relation.
Measurement approaches and tailored solutions for areas
with bad connectivity are listed. Possible ways of improvement are discussed.
