# Hi, I’m Mihir Swarnkar

I build systems from first principles, with a focus on correctness, failure modes,
and recovery. My work is exploratory and early-stage, aimed at understanding how
real systems behave under stress rather than producing polished demos.

I prefer depth over breadth and document what breaks, why it breaks, and what the
constraints actually are.

---

## Current Focus

- Building a **replicated key-value store** from scratch
- Starting with **single-node correctness**, WAL, and crash recovery
- Explicitly stating **guarantees vs non-guarantees**
- Treating failures and limitations as first-class artifacts

This system is early-stage and evolving.

---

## Prior Exploratory System Work

- **Mini Redis-like KV Store**
  - In-memory state
  - Write-ahead logging
  - Crash recovery via log replay
  - Learned the real cost of durability and fsync semantics

- **Mini Container Runtime**
  - Process lifecycle exploration
  - Linux namespaces and cgroups
  - Signal handling across process boundaries
  - Discovered why PID 1 and init behavior matter

These were stepping stones, not production systems.

---

## How I Work

- One system over many projects
- Written invariants over clever code
- Public code and documented failures
- No framework abstractions for core logic
- Comfort with being explicit about limits

I am not claiming expertise.
I am building toward it deliberately.

---

## Links

- Portfolio / Engineering Notes: [your website link]
- GitHub: https://github.com/Yumekaz
- Email: your.email@example.com
