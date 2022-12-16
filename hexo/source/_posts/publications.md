---
title: Publications
---
## 2023

### [Chasing Shadows: A security analysis of the ShadowTLS proxy](https://gaukas.wang/paper/chasing_shadows-foci23.pdf)

#### Author(s)

Gaukas Wang, Anonymous, Jackson Sippe, Hai Chi, Eric Wustrow

#### Abstract

ShadowTLS is a new type of circumvention tool where the relay forwards traffic to a legitimate (unblocked) TLS server until the end of the handshake, and then connects the client to a hidden proxy server (e.g. Shadowsocks). In contrast to previous probe-resistant proxies, this design can evade SNI sniffing, since to the censor it appears as a legitimate TLS connection to an unblocked domain.

In this paper, we describe several attacks against ShadowTLS which would allow a censor to identify if a suspected IP is hosting a ShadowTLS relay or not (and block it accordingly), distinguishing it from the legitimate TLS servers they mimic. Our attacks require only a few TCP connections to the suspected IP, a capability that censors including China have already demonstrated in order to block previous proxies.

We evaluate these vulnerabilities by performing Internet-wide scans to discover potential ShadowTLS proxies, and find over 15K of them. We also describe mitigations against this attack that ShadowTLS (and proxies like it) can implement, and work with the ShadowTLS developers to deploy these fixes.

## 2022

### [Acuerdo: Fast Atomic Broadcast over RDMA](https://gaukas.wang/paper/acuerdo-icpp22.pdf)

#### Author(s)

Joseph Izraelevitz, Gaukas Wang, Rhett Hanscom, Kayli Silvers, Tamara Silbergleit Lehman, Gregory Chockler, Alexey Gotsman

#### Abstract 

Atomic broadcast protocols ensure that messages are delivered to a group of machines in some total order, even when some of these machines can fail. These protocols are key to making distributed services fault-tolerant, as their total order guarantee allows keeping multiple service replicas in sync. But, unfortunately, atomic broadcast protocols are also notoriously expensive. 

We present a new protocol, called Acuerdo, that improves atomic broadcast performance by using remote direct memory addressing (RDMA). Acuerdo is built from the ground up to perform communication using one-side RDMA writes, which do not use the CPU of the remote machine, and is explicitly designed to minimize waiting on the critical path. Our experimental results demonstrate that Acuerdo provides raw throughput comparable to or exceeding other RDMA atomic broadcast protocols, while improving latency by almost 2𝑥.

In Proceedings of: **ICPP 2022**