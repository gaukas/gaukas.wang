---
title: Publications
---
## 2022

### [Acuerdo: Fast Atomic Broadcast over RDMA](https://gaukas.wang/paper/acuerdo-icpp22.pdf)

#### Author(s): 

Joseph Izraelevitz, Gaukas Wang, Rhett Hanscom, Kayli Silvers, Tamara Silbergleit Lehman, Gregory Chockler, Alexey Gotsman

#### Abstract: 

Atomic broadcast protocols ensure that messages are delivered to a group of machines in some total order, even when some of these machines can fail. These protocols are key to making distributed services fault-tolerant, as their total order guarantee allows keeping multiple service replicas in sync. But, unfortunately, atomic broadcast protocols are also notoriously expensive. 

We present a new protocol, called Acuerdo, that improves atomic broadcast performance by using remote direct memory addressing (RDMA). Acuerdo is built from the ground up to perform communication using one-side RDMA writes, which do not use the CPU of the remote machine, and is explicitly designed to minimize waiting on the critical path. Our experimental results demonstrate that Acuerdo provides raw throughput comparable to or exceeding other RDMA atomic broadcast protocols, while improving latency by almost 2𝑥.

In Proceedings of: **ICPP 2022**