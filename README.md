# Hi, I’m Mihir Swarnkar

I build systems from first principles, focusing on correctness, failure modes,
and recovery. My work is hands-on and exploratory, centered on understanding how
distributed and OS-level systems behave under real constraints.

I prefer one deep system over many shallow projects and document trade-offs,
failures, and limits explicitly.

---

## Core Systems Work

### Mini-Redis-Cassandra — Distributed Key-Value Store
**Python · TCP · Raft-inspired consensus · Consistent Hashing**

A distributed key-value database built to explore CAP trade-offs, replication,
and failure handling.

- Implemented configurable consistency levels (ANY, QUORUM, STRONG) to study
  availability vs consistency behavior under partitions
- Built a Raft-inspired leader election and replication mechanism, observing
  stable leader failover during simulated network partitions
- Designed sharding via consistent hashing with virtual nodes for balanced key
  distribution and minimal rebalancing
- Implemented a custom TCP-based protocol with JSON framing, sustaining
  thousands of operations per second in local multi-node tests
- Wrote a fault-injection framework to simulate packet drops and network delays,
  validating recovery paths and replica convergence

This system is intentionally simplified and incomplete, but it forced explicit
reasoning about safety, liveness, and failure boundaries.

---

### Mini-Docker — Container Runtime Implementation
**Python · Linux kernel APIs · cgroups v2**

A container runtime built from scratch to understand process isolation and
resource control in Linux.

- Implemented multiple Linux namespaces (PID, NET, IPC, UTS, MNT, USER) to achieve
  process and filesystem isolation
- Designed a defense-in-depth security model using seccomp-BPF filtering,
  capability dropping, and `NO_NEW_PRIVS`
- Integrated cgroups v2 controllers to enforce CPU and memory limits and protect
  the host from resource exhaustion
- Built basic container networking using veth pairs, Linux bridges, and NAT
- Measured lightweight overhead (~12 MB memory) and fast startup latency in local
  benchmarks

This project exposed the complexity behind container semantics and the importance
of correct init and signal-handling behavior.

---

## Current Focus

- Extending distributed system work with deeper emphasis on:
  - durability semantics
  - replication safety
  - crash recovery
  - explicit guarantees vs non-guarantees
- Treating failures, invariants, and limits as first-class artifacts

I am early-stage and not claiming expertise.
I am building toward it deliberately.

---

## How I Work

- Depth over breadth
- Written invariants over clever code
- Explicit trade-offs and non-goals
- Public code with documented failures
- Minimal abstractions for core system logic

---

## Links

- Portfolio / Engineering Notes: [[Mihir]](https://yumekaz.github.io/Portfolio/)
- GitHub: https://github.com/Yumekaz
- Email: mihir.swarnkar722@gmail.com
