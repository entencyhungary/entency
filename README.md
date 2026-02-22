# ENTENCY

**A unified neural infrastructure for the next-generation internet.**

ENTENCY is building a new foundation layer for distributed applications - combining a browser runtime, a decentralized execution network, and a programmable protocol stack into a single coherent system.

This repository serves as the public-facing entry point to the ENTENCY ecosystem.

---

# Vision

The web evolved in layers.

Static pages.
Dynamic applications.
Cloud platforms.
Decentralized networks.

Yet fragmentation remains.

Different protocols.
Different runtimes.
Different trust models.
Different execution environments.

ENTENCY unifies them.

The goal is not to replace the internet.
The goal is to evolve it.

A programmable, protocol-agnostic, distributed execution layer - accessible through a unified workstation.

---

# What Problem Does ENTENCY Solve?

Modern digital infrastructure is fragmented:

- Web browsers operate in isolated sandboxes.
- Distributed systems require complex integration layers.
- Streaming, hosting, execution, and networking are separate stacks.
- Decentralized systems lack cohesive user-facing runtimes.

ENTENCY integrates:

- Protocol handling
- Execution environment
- Content distribution
- Secure session lifecycle management
- Distributed node orchestration

Into a single architecture.

---

# Why Is It Different?

Most systems focus on one layer:

- A browser.
- A node.
- A blockchain.
- A hosting platform.
- A streaming network.

ENTENCY integrates them into a unified protocol ecosystem.

It is not a wrapper around existing infrastructure.
It is an extensible runtime designed for protocol-level evolution.

Key differences:

- Native support for custom protocols (e.g. gns://)
- Integrated distributed node system (GNS)
- Session-driven architecture
- Multi-platform runtime (Windows / Linux x64 / Linux ARM64)
- CI-based reproducible builds
- Cross-platform packaging pipeline
- Deterministic release infrastructure

ENTENCY is not a website.
It is a platform layer.

---

# Why Now?

Three forces are converging:

1. Hardware decentralization (ARM boards, edge devices)
2. Distributed computing becoming mainstream
3. The need for protocol-level innovation beyond HTTP

The infrastructure of the next decade cannot rely purely on centralized stacks.

ENTENCY is designed for distributed-native environments.

---

# Why ENTENCY?

Because the system is built holistically.

ENTENCY UP (Unified Protocol Browser and Workstation Runtime)
+
ENTENCY GNS (Global Neural System)
==================================

Unified distributed execution environment.

This is not an incremental extension of the web.

It is an architectural rethink.

---

# Architecture Overview

High-level system structure:

```
+---------------------------------------------------------+
|                    ENTENCY UP                           |
|    (Unified Protocol Browser & Workstation Runtime)     |
|                                                         |
|  +-------------------+     +------------------------+   |
|  | Session FSM       | --> | Protocol Router        |   |
|  +-------------------+     +------------------------+   |
|            |                         |                  |
|            v                         v                  |
|     Local Runtime Layer       gns:// Handler            |
|            |                         |                  |
+------------+-------------------------+------------------+
             |
             v
+---------------------------------------------------------+
|                ENTENCY GNS (Node Layer)                 |
|                                                         |
|  +----------------+   +------------------------------+  |
|  | Node Runtime   |<->| Distributed Chunk Network    |  |
|  +----------------+   +------------------------------+  |
|           |                     |                       |
|           v                     v                       |
|     Storage Layer        Execution Layer                |
+---------------------------------------------------------+
```

Core components:

**ENTENCY UP**

- Unified browser runtime
- Protocol execution layer
- Integrated GNS communication
- Multi-tab session architecture (planned expansion)
- Local and distributed content resolution

**ENTENCY GNS**

- Distributed node network
- Chunked content distribution
- Streaming and hosting support
- Deterministic rebuild of distributed assets
- Cross-node orchestration

---

# Key Capabilities

- Custom protocol resolution (gns://)
- Distributed streaming playback
- Web hosting via distributed node layer
- Local node deployment
- ARM64 board compatibility
- Electron-based cross-platform runtime
- Deterministic CI release builds
- Multi-architecture packaging

---

# Screenshots

### ENTENCY UP Interface

![ENTENCY UP UI](./assets/screenshots/up-interface.png)

### GNS Node Runtime

![GNS Runtime](./assets/screenshots/gns-runtime.png)

### Streaming Playback via gns://

![Streaming Playback](./assets/screenshots/streaming.png)

---

# Roadmap

### Phase 1 — Core Architecture & Interface Foundation

- Core runtime architecture design
- Unified workstation engine (ENTENCY UP)
- Foundational GNS node integration layer
- Protocol routing framework
- Session lifecycle engine (FSM-based)
- UI system architecture and design language
- Cross-platform rendering layer
- Brand identity and interaction model

### Phase 2 - Core Stability (Current)

- Local node integration
- Windows x64 packaging
- Linux x64 and Linux ARM64 packaging
- Deterministic CI builds
- Unified release pipeline

### Phase 3 - Distributed Chunk Network

- Cross-node chunk orchestration
- Content fragmentation and reassembly
- Distributed streaming layer
- Fault tolerance mechanisms

### Phase 4 - Protocol Expansion

- Extended gns:// capabilities
- Secure node identity model
- Tokenized network fuel layer (ENT)

### Phase 5 - Ecosystem Layer

- Public SDK
- Developer integration tools
- Visualization dashboards
- Monitoring and analytics layer

---

# Release Downloads

Latest releases:

Windows Installer
-> [https://github.com/entencyhungary/entency/releases/latest](https://github.com/entencyhungary/entency/releases/latest)

Linux x64 (.deb)
-> [https://github.com/entencyhungary/entency/releases/latest](https://github.com/entencyhungary/entency/releases/latest)

Linux ARM64 (.deb)
-> [https://github.com/entencyhungary/entency/releases/latest](https://github.com/entencyhungary/entency/releases/latest)

(Links are NOT available yet)

---

# Technical Principles

- Deterministic builds
- Platform-native packaging
- Separation of runtime and distribution layer
- Protocol-level extensibility
- Architecture-first engineering
- Closed-core during foundational development

---

# Philosophy

Technology is not just code.

It is infrastructure.
It is narrative.
It is architecture.

ENTENCY is building infrastructure for systems that do not yet exist.

---

Core engine is currently closed during active development.
