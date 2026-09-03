---
layout: home
title: Prasenjit Das
subtitle: Systems Engineer | PhD Candidate | Principal at Teknally Consulting Group
---

### High-Performance Systems & Research Lab

I build deterministic, low-latency infrastructure in asynchronous **Rust** and conduct doctoral research on zero-overhead edge-to-cloud networking protocols. 

Through **Teknally Consulting Group**, I assist engineering teams with low-level systems refactoring, $p99.9$ tail-latency optimization, and fractional infrastructure leadership.

---

### Active Focus Areas

* **ZeroGate (Primary Portfolio Artifact):** High-throughput, zero-copy protocol translation gateway (`CoAP/CBOR` to `gRPC/Protobuf`) engineered with Tokio and Tonic.
* **Doctoral Research:** Eliminating dynamic heap allocations and CPU overhead during edge-to-cloud payload transcoding under strict memory constraints ($<16\text{MB}$).
* **B2B Technical Advisory:** Low-latency network design, custom protocol runtimes, and specialized Rust infrastructure consulting.

---

### Core Target Metrics (ZeroGate Engine)

| Constraint / Metric | Target Value | Implementation Strategy |
| :--- | :--- | :--- |
| **Hot-Path Allocations** | **0 Heap Allocations** | Unsafe-free `BytesMut` buffer slicing |
| **Parsing Latency** | **Sub-microsecond** | Zero-copy header extraction & state machine |
| **Memory Footprint** | **$< 16\text{MB}$ RSS** | Static compilation & minimal async runtime overhead |
| **Protocol Path** | **UDP / CoAP $\rightarrow$ gRPC** | Asynchronous lock-free ring channel dispatch |

---

### Navigation & Resources

* Explore doctoral research questions and problem formulations on the **[Research](/research)** page.
* View architecture diagrams, `Criterion.rs` benchmarks, and `DESIGN.md` specs on the **[Projects](/projects)** page.
* Read technical deep dives on Rust memory safety, lock-free queues, and low-level I/O on the **[Blog](/blog)**.
* Retain **[Teknally Consulting Group](/consulting)** for fractional technical advisory and infrastructure refactoring.