<p align="center">
  <img src="./profile-console.svg" alt="Mihir Swarnkar distributed systems profile console" width="100%">
</p>

<p align="center">
  <a href="https://yumekaz.vercel.app/">portfolio</a> ·
  <a href="https://yumekaz.vercel.app/projects/">projects</a> ·
  <a href="https://yumekaz.vercel.app/notes/">engineering notes</a> ·
  <a href="https://yumekaz.vercel.app/resume.pdf">resume</a>
</p>

## `identity :: distributed_backend_engineer`

I am a final-year B.Tech CSE student focused on the algorithmic core of
distributed backend systems: replication, consistency, coordination, and
recovery under failure. I build inspectable systems that turn those questions
into executable behavior, failure tests, and evidence reports.

My lane is the logic that keeps services correct and available when nodes
disagree, leaders become stale, writes are acknowledged too early, or a process
dies halfway through a state transition. Cloud provisioning, CI/CD automation,
and hardware-level systems engineering are outside this profile's center of
gravity.

<table>
  <tr>
    <td><strong>PRIMARY SYSTEMS</strong><br>replication · quorum · gossip · leases</td>
    <td><strong>FAILURE MODEL</strong><br>partitions · crashes · stale state · disk faults</td>
    <td><strong>TOOLS</strong><br>Python · Rust · Go · Linux · gRPC</td>
  </tr>
</table>

## `/start-here`

The three repositories below are the clearest proof of how I think and build.

### `01 / Coordination-service`

[Repository](https://github.com/Yumekaz/Coordination-service)

A replicated coordination service for state, sessions, leases, watches, and
control-plane history. It explores leader/follower behavior, quorum-gated
operations, causal incident tracing, and recovery under cluster failure.

`evidence:` **306 documented tests** · cluster-failure coverage · checked-in
seed-42 certification note

### `02 / Mini-Redis-Cassandra`

[Repository](https://github.com/Yumekaz/Mini-Redis-Cassandra)

A distributed key-value store built to study sharding, replication, gossip
membership, persistence, and tunable consistency. The important result was a
real consistency failure: the system exposed read-after-write violations,
which were traced to protocol decisions and then fixed.

`evidence:` **23 initial violations → 0** · five consecutive zero-error
seed-42 reruns after the fixes

### `03 / FailForge`

[Repository](https://github.com/Yumekaz/FAILFORGE)

A deterministic fault-injection framework for making distributed failures
repeatable instead of anecdotal. Seeded schedules, partitions, crashes, disk
faults, invariant checkers, timeline reports, and delta-debugging turn a
failure into a reviewable artifact.

`evidence:` **15 documented fault types** · reproducible schedules · invariant
driven reports

## `/evidence-board`

| signal | what is recorded |
|---|---|
| `replication` | leader/follower behavior, quorum-gated operations, causal history |
| `consistency` | read-after-write violations, root-cause analysis, fixed reruns |
| `reliability` | seeded fault schedules, invariant checks, minimized failures |
| `correctness` | 281 oracle comparisons and 241 metamorphic variants in Qydrel |

These are deliberately inspectable systems prototypes. Their value is not a
production-readiness claim; the design decisions, failure behavior, fixes, and
evidence boundaries are public and reviewable.

## `/adjacent-systems`

- [Qydrel](https://github.com/Yumekaz/Qydrel) — Rust compiler/runtime
  correctness lab with AST-oracle execution, backend equivalence checks,
  fuzzing, and shrinking.
- [Mini-Docker](https://github.com/Yumekaz/Mini-Docker) — Linux container
  runtime study covering namespaces, cgroups, OverlayFS, networking, seccomp,
  capabilities, and lifecycle control.
- [DRT](https://github.com/Yumekaz/DRT) — deterministic record/replay runtime
  for selected Python concurrency failures.
- [Cairn](https://github.com/Yumekaz/Cairn) +
  [DuraFlow](https://github.com/Yumekaz/DURAFLOW) — interrupted deployment
  recovery, lease reclaim, and durable workflow state transitions.
- [TinyTantrum](https://github.com/Yumekaz/TinyTantrum) — from-scratch GPT
  laboratory with reproducible evaluation and checkpoint recovery.
- [BitNet Triton](https://github.com/Yumekaz/bitnet-1.58b-gemm-triton) —
  GPU-kernel prototype that measures packed-weight performance against
  optimized FP16 GEMM.
- [Orbits](https://github.com/Yumekaz/Orbits) — static and runtime codebase
  mapping for evidence-backed architecture decisions.

## `/build-protocol`

```text
problem → invariant → failure model → implementation → evidence → boundary
```

- Start with the guarantee and the failure model, not the framework.
- Treat failures, recovery paths, and observability as design inputs.
- Prefer a small executable proof over a large architectural claim.
- Preserve the decision, the failed attempt, the fix, and the remaining limit.

## `/connect`

- [Portfolio and engineering notes](https://yumekaz.vercel.app/)
- [Resume PDF](https://yumekaz.vercel.app/resume.pdf)
- [LinkedIn](https://www.linkedin.com/in/mihirswarnkar/)
- [GitHub](https://github.com/Yumekaz)
- [Email](mailto:mihir.swarnkar722@gmail.com)
