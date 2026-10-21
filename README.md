<p align="center">
  <img src="./profile-console.svg" alt="Yumekaz — Mihir Swarnkar's open workshop. Building systems. Following the failure." width="100%">
</p>

<p align="center">
  <a href="https://yumekaz.vercel.app/"><strong>Portfolio</strong></a>
  &nbsp; / &nbsp;
  <a href="#selected-systems"><strong>Selected systems</strong></a>
  &nbsp; / &nbsp;
  <a href="https://yumekaz.vercel.app/notes/"><strong>Field notes</strong></a>
  &nbsp; / &nbsp;
  <a href="mailto:mihir.swarnkar722@gmail.com"><strong>Say hello</strong></a>
</p>

<br>

## Curiosity, made executable.

I'm **Mihir Swarnkar**, also known as **Yumekaz**. I build software to answer questions I can't settle by reading alone.

Most of my work lives in **distributed systems, correctness tooling, and the machinery beneath an application**. I'm especially interested in the moment a node disappears, a read goes stale, or a process stops halfway through a promise.

My favourite question: **what must remain true when the system fails?**

<br>

## Selected systems

Four questions. Four ways to investigate them.

<table>
  <tr>
    <td width="50%" valign="top">
      <sub>01 / COORDINATION</sub>
      <h3><a href="https://github.com/Yumekaz/Coordination-service">Coordination-service ↗</a></h3>
      <p><strong>Who gets to lead when nodes disagree?</strong></p>
      <p>Replicated state, sessions, leases, watches, and recovery. A control-plane prototype that makes leadership and failure history inspectable.</p>
      <p><code>Python</code> <code>Replication</code> <code>Quorum</code></p>
    </td>
    <td width="50%" valign="top">
      <sub>02 / FAILURE TESTING</sub>
      <h3><a href="https://github.com/Yumekaz/FAILFORGE">FailForge ↗</a></h3>
      <p><strong>Can we make the failure happen again?</strong></p>
      <p>Seeded fault schedules, invariant checks, and failure minimization. A lab for turning distributed-system failures into reproducible evidence.</p>
      <p><code>Go</code> <code>Fault injection</code> <code>Replay</code></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <sub>03 / RECOVERY</sub>
      <h3><a href="https://github.com/Yumekaz/Cairn">Cairn ↗</a></h3>
      <p><strong>What survives an interrupted deploy?</strong></p>
      <p>A single-node Linux deployment platform exploring durable workflows, health gates, rollback, and reconciliation after interruption.</p>
      <p><code>Go</code> <code>Durability</code> <code>Linux</code></p>
    </td>
    <td width="50%" valign="top">
      <sub>04 / CORRECTNESS</sub>
      <h3><a href="https://github.com/Yumekaz/Qydrel">Qydrel ↗</a></h3>
      <p><strong>Do different runtimes mean the same thing?</strong></p>
      <p>A small Rust language and runtime lab with an independent oracle, backend comparisons, fuzzing, and a museum of minimized bugs.</p>
      <p><code>Rust</code> <code>Compilers</code> <code>Fuzzing</code></p>
    </td>
  </tr>
</table>

### A failure worth reading

In **[Mini-Redis-Cassandra](https://github.com/Yumekaz/Mini-Redis-Cassandra)**, acknowledged writes were followed by stale reads. Investigating that failure exposed a mismatch between write quorums and read guarantees, along with persistence and transport issues.

The repository follows the trail through the failure, the fixes, and the reruns.

<br>

## Elsewhere in the workshop

I also build tools and applications around reading, code exploration, and learning by implementation.

| Project | The idea |
| :--- | :--- |
| **[Yomikura](https://github.com/Yumekaz/Yomikura)** | A Suwayomi library and reader client for desktop, web, and PWA. |
| **[Orbits](https://github.com/Yumekaz/Orbits)** | Map a codebase's structure and runtime connections before changing it. |
| **[TinyTantrum](https://github.com/Yumekaz/TinyTantrum)** | Learn the machinery of a GPT through implementation, evaluation, and recovery. |

<details>
<summary><strong>Open the systems drawer</strong></summary>

<br>

| Project | Investigation |
| :--- | :--- |
| **[DRT](https://github.com/Yumekaz/DRT)** | Record and replay concurrency failures in Python programs using explicit scheduling points. |
| **[DuraFlow](https://github.com/Yumekaz/DURAFLOW)** | Checkpoint workflow steps and recover after interruption. |
| **[Mini-Docker](https://github.com/Yumekaz/Mini-Docker)** | Explore Linux isolation through namespaces, cgroups, OverlayFS, and lifecycle control. |
| **[BitNet Triton](https://github.com/Yumekaz/bitnet-1.58b-gemm-triton)** | Measure a packed ternary GEMM experiment against optimized FP16 baselines, including negative results. |

</details>

<br>

## How I work

1. **Name the guarantee.** Decide what must remain true and which failures the system must handle.
2. **Make the failure repeatable.** Keep the seed, trace, or smallest example that explains it.
3. **Leave a useful record.** Document the decision, the fix, and the limits that remain.

These repositories include focused prototypes and learning projects. Their design notes, tests, and documented boundaries are part of the work.

**Working materials** &nbsp; `Python` · `Go` · `Rust` · `TypeScript` · `Linux`

<br>

---

<p align="center">
  <strong>Have an interesting system, a stubborn bug, or a good question?</strong><br>
  I'd be glad to hear about it.
</p>

<p align="center">
  <a href="mailto:mihir.swarnkar722@gmail.com">Email</a>
  &nbsp; · &nbsp;
  <a href="https://www.linkedin.com/in/mihirswarnkar/">LinkedIn</a>
  &nbsp; · &nbsp;
  <a href="https://yumekaz.vercel.app/resume.pdf">Résumé</a>
  &nbsp; · &nbsp;
  <a href="https://github.com/Yumekaz?tab=repositories">All repositories ↗</a>
</p>
