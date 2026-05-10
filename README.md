# Hi, I’m Mihir Swarnkar

I build systems from first principles: container runtimes, distributed storage,
coordination services, deterministic debugging tools, compiler correctness labs,
and codebase intelligence systems.

My work focuses on correctness, failure modes, replayability, recovery paths,
and making system behavior observable instead of hidden behind abstractions.

I prefer a few deep systems over many shallow projects.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Distributed Systems](https://img.shields.io/badge/Distributed%20Systems-1f2937?style=flat-square)
![Correctness](https://img.shields.io/badge/Correctness-111827?style=flat-square)
![WebAssembly](https://img.shields.io/badge/WebAssembly-654FF0?style=flat-square&logo=webassembly&logoColor=white)

---

## Selected Work

| Project | Focus | What it demonstrates |
|--------|-------|----------------------|
| [Mini-Docker](https://github.com/Yumekaz/Mini-Docker) | Container runtime from scratch | Linux namespaces, cgroups v2, OverlayFS, veth networking, seccomp/capability hardening, lifecycle control |
| [Mini-Redis-Cassandra](https://github.com/Yumekaz/Mini-Redis-Cassandra) | Distributed key-value store | Consistent hashing, replication, gossip membership, tunable consistency, persistence, failure handling |
| [Coordination-service](https://github.com/Yumekaz/Coordination-service) | Crash-aware control plane | Leader/follower replication, quorum-gated writes, causal incident tracing, control-plane visibility |
| [DRT](https://github.com/Yumekaz/DRT) | Deterministic record/replay runtime | Controlled scheduling, replayable concurrency failures, failure bundles, trace reports, schedule exploration |
| [Qydrel](https://github.com/Yumekaz/Qydrel) | Compiler/runtime correctness lab | Bytecode verification, AST oracle execution, VM/GC/JIT equivalence checks, trace replay, fuzzing, shrinking |
| [Orbits](https://github.com/Yumekaz/Orbits) | Codebase map and cleanup tool | Static dependency graphs, runtime overlays, architecture diffs, cleanup plans, language coverage, visual exploration |
| [WasmForge](https://github.com/Yumekaz/WasmForge) | Local-first browser IDE | WebAssembly workers, browser-side execution, offline-first storage, Python/JS/SQL experimentation in the browser |
| [Autoforge](https://github.com/Yumekaz/Autoforge) | Governed AI code generation | YAML-to-code generation, validation gates, adversarial review, traceability, architect/auditor-style pipeline |

---

## Recently Shipping

- Improving **Mini-Docker** as a runtime layer for lightweight self-hosted infrastructure
- Expanding **DRT** around failure bundles, replay reports, and schedule minimization
- Hardening **Qydrel** as a compiler/runtime correctness lab with executable evidence
- Turning **Orbits** into a practical codebase-mapping and cleanup CLI
- Connecting my systems work toward stateful deployment, recovery, and failure visibility

---

## Project Notes

### Mini-Docker

A from-scratch container runtime in Python built directly on Linux primitives.

It implements process isolation, resource limits, virtual networking, filesystem
layering, container lifecycle handling, and a Unix-socket API surface for higher
level orchestration experiments.

This is not meant to replace Docker. It exists to understand what Docker,
Podman, and platform runtimes abstract away.

### DRT

A deterministic concurrency testing and record/replay runtime for Python code
that opts into DRT-managed threads, synchronization primitives, and controlled
nondeterministic APIs.

The goal is to turn flaky concurrency bugs into repeatable, inspectable
executions.

### Qydrel

A Rust compiler/runtime correctness lab for a deliberately small language.

The interesting part is not language size. The interesting part is the audit
loop: AST oracle execution, bytecode verification, backend equivalence, trace
replay, fuzzing, shrinking, and evidence reports.

### Orbits

A codebase map for understanding unfamiliar repositories.

It analyzes project structure, entrypoints, dependency edges, runtime traces,
dead-code confidence, architecture diffs, and cleanup paths so refactoring can
be based on evidence instead of guesswork.

---

## Current Direction

I am building toward deeper infrastructure around:

- runtime isolation
- stateful deployment
- deterministic failure testing
- durable workflow execution
- replicated control planes
- crash recovery
- codebase intelligence
- compiler/runtime correctness

The long-term direction is to connect these ideas into a serious infrastructure
stack: run workloads, coordinate state, recover from failures, replay bugs, and
explain system behavior with evidence.

---

## How I Work

- Depth over breadth
- Correctness before cleverness
- Failure cases as first-class design inputs
- Written invariants and explicit non-goals
- Small systems that expose real engineering trade-offs
- Public code, honest limitations, and reproducible behavior

---

## Links

- Portfolio / Engineering Notes: [Mihir](https://yumekaz.github.io/Portfolio/)
- GitHub: [Yumekaz](https://github.com/Yumekaz)
- Email: mihir.swarnkar722@gmail.com
