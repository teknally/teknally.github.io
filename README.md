# Prasenjit Das | Systems Engineering & Research Lab

> **Systems & Infrastructure Engineer | PhD Scholar | Principal at Teknally Consulting Group**

Welcome to the central repository and research log for [teknally.github.io](https://teknally.github.io). This space serves as a technical portfolio, doctoral research clearinghouse, and engineering laboratory focused on high-performance systems, low-latency networking, and asynchronous Rust.

---

## Technical Focus & Pillars

### 1. Systems & Infrastructure Engineering
* **Core Stack:** Rust (Tokio, Bytes, Tonic, Serde), C/C++, Linux Systems Programming.
* **Specializations:** Zero-copy byte parsing, lock-free concurrency models, low-latency API gateways, memory-constrained execution environments.
* **Performance:** $p99.9$ tail-latency minimization, cache-aware data structures, non-blocking I/O.

### 2. Doctoral Research (Computer Science)
* **Domain:** Edge Computing, Industrial IoT (IIoT), and Protocol Translation.
* **Thesis Topic:** Zero-overhead edge-to-cloud translation gateways for resource-constrained environments.
* **Core Problem:** Eliminating heap allocation overhead during dynamic CoAP/CBOR to gRPC/Protobuf transcoding at the network edge.

### 3. Technical Advisory (Teknally Consulting Group)
Through **Teknally Consulting Group**, I provide B2B technical strategy and engineering advisory services:
* **System Architecture & Refactoring:** Migrating heavy legacy middleware to high-throughput, deterministic Rust microservices.
* **Performance Profiling:** Memory leak analysis, flamegraph diagnostics, and sub-millisecond benchmarking.
* **B2B Remote Contracting:** Available for specialized fractional CTO and principal systems infrastructure roles.

---

## Featured Portfolio Artifact: ZeroGate

**ZeroGate** is a high-performance, asynchronous protocol translation gateway engineered in Rust.

* **Architecture:** Ingests binary CoAP/CBOR frames over UDP/TCP, parses headers without dynamic heap allocation using `BytesMut` slices, and forwards decoded payloads to cloud targets via async gRPC (`Tonic`) over HTTP/2.
* **Benchmarks:** Designed for sub-microsecond parsing latency and low memory footprint ($<16\text{MB}$ operating threshold).
* **Key Components:**
  * `zerogate-core`: Zero-copy frame parsing and state machine.
  * `zerogate-transcode`: Zero-alloc CBOR-to-Protobuf translation pipeline.
  * `zerogate-net`: Non-blocking Tokio socket runtime with lock-free channel orchestration.

---

## Site Navigation & Structure

| Route | Focus Area |
| :--- | :--- |
| **[Home](https://teknally.github.io/)** | Executive summary, active benchmarks, and system status. |
| **[Research](https://teknally.github.io/research)** | PhD research statements, problem formulations, and preprints. |
| **[Projects](https://teknally.github.io/projects)** | Open-source systems artifacts, design specifications (`DESIGN.md`), and Criterion benchmarks. |
| **[Consulting](https://teknally.github.io/consulting)** | B2B advisory, Teknally service offerings, and retainer terms. |
| **[Blog](https://teknally.github.io/blog)** | Technical deep dives on Rust memory safety, lock-free queues, and eBPF profiling. |

---

## Research Publications & Writing

* *Zero-Copy Memory Allocation Strategies in Asynchronous Rust* (Technical Note)
* *Deterministic Tail-Latency Bounds in Constrained Edge Translation Gateways* (PhD Research Working Paper)

---

## Contact & Connect

* **Website:** [teknally.github.io](https://teknally.github.io)
* **Entity:** Teknally Consulting Group
* **Location:** Assam, India (Available for Global 100% Remote B2B Contracting)
* **GitHub:** [@teknally](https://github.com/teknally)

---
*© 2026 Prasenjit Das / Teknally Consulting Group. All rights reserved.*
