# ENTENCY

### Distributed Infrastructure. Unified Execution.

> A deterministic distributed computing ecosystem built around  
> **ENTENCY UP** and the **ENTENCY GNS — Global Neural System**.

---

## What is ENTENCY?

ENTENCY is an experimental distributed computing ecosystem designed to bring **execution, storage, communication, streaming, compute and application delivery** into a unified architecture.

At its foundation are two core systems:

**ENTENCY UP** — the user-facing browser, workstation and execution environment.

**ENTENCY GNS** — the distributed node infrastructure that provides network-native services beneath it.

Together, they form an environment where applications and services can operate across both the conventional web and the GNS network.

ENTENCY is not simply a browser.

It is not simply a peer-to-peer network.

It is not simply a hosting platform.

**It is an attempt to build a unified execution environment for distributed-native systems.**

---

# Why ENTENCY?

Modern internet infrastructure is composed of many independent layers:

- browsers provide access,
- cloud platforms provide compute,
- storage systems hold data,
- CDNs distribute content,
- communication platforms move messages,
- streaming infrastructure transports media,
- identity systems establish trust.

Each layer solves a different problem.

But each layer also introduces another dependency.

ENTENCY explores a different model:

> **What if execution, protocol, storage, communication and distribution were designed as parts of the same system?**

The goal is not to replace the Web.

The goal is to extend what an internet-native execution environment can be.

---

# Core Architecture

ENTENCY currently revolves around two tightly integrated systems.

```text
+-------------------------------------------------------------+
|                         ENTENCY UP                          |
|                                                             |
|        Browser • Workstation • Execution Environment        |
|                                                             |
|   +----------------+     +-------------------------------+  |
|   |  Session FSM   | --> |      Protocol Router          |  |
|   +----------------+     +-------------------------------+  |
|           |                         |                       |
|           v                         v                       |
|   Runtime Isolation            gns:// Resolution            |
|           |                         |                       |
|           +------------+------------+                       |
|                        |                                    |
+------------------------|------------------------------------+
                         |
                         v
+-------------------------------------------------------------+
|                    ENTENCY GNS                              |
|                 Global Neural System                        |
|                                                             |
|  Identity • Transport • Objects • Services • Trust          |
|                                                             |
|   +----------------+      +------------------------------+  |
|   |  Node Runtime  | <--> |   Distributed Node Network   |  |
|   +----------------+      +------------------------------+  |
|           |                          |                      |
|           v                          v                      |
|   Chunk / Object Layer        Service Infrastructure        |
|                                      |                      |
|                  +-------------------+------------------+   |
|                  |        |          |        |         |   |
|               Storage   Comms    Streaming  Compute  Hosting |
|                                                             |
+-------------------------------------------------------------+
```

### Design principle

**Deterministic control at the execution surface.  
Distributed operation underneath.**

---

# ENTENCY UP

### Unified Protocol Browser & Workstation

ENTENCY UP is the primary user-facing environment of the ENTENCY ecosystem.

It combines browser functionality, workstation capabilities, protocol routing and GNS-native execution into a single application.

UP can interact with conventional web resources while also providing a native interface to services operating through the GNS network.

### Core responsibilities

- deterministic session lifecycle management
- FSM-based session control
- protocol routing
- `gns://` resolution
- GNS-native navigation
- runtime isolation boundaries
- local application execution
- GNS node communication
- network state integration
- service interaction
- integrated execution surfaces

The Session FSM controls session state independently from the visual tab lifecycle, allowing protocol events, reconnects, redirects and termination to be handled deterministically.

UP is therefore more than the graphical interface to GNS.

**It is the execution and control surface of ENTENCY.**

---

# ENTENCY GNS

### Global Neural System

ENTENCY GNS is the distributed infrastructure beneath ENTENCY.

It is built around deterministic content addressing, chunked data, independently operating nodes and protocol-defined services.

Instead of treating storage, communication, streaming, compute and hosting as completely separate infrastructures, GNS provides foundations for operating them through the same distributed network architecture.

### Core responsibilities

- deterministic chunk processing
- canonical object and manifest identities
- content verification
- distributed node communication
- peer discovery and connectivity
- node identity
- distributed storage
- cross-node data retrieval
- streaming
- communication
- compute execution
- service publication and resolution
- capability-based authorization
- reputation
- audit and event state
- network inspection

GNS is designed so that network state and content can be reconstructed and verified deterministically rather than relying exclusively on a single central service.

---

# GNS Service Layer

The GNS architecture is being developed as a common infrastructure for multiple distributed service classes.

## Storage

Content can be fragmented into deterministic chunks, addressed through canonical objects and reconstructed from network resources.

## Communication

The Communication Fabric provides foundations for GNS-native message exchange and distributed communication services.

## Streaming

GNS supports chunk-oriented streaming primitives designed for progressive reconstruction and distributed delivery.

## Compute

The compute layer provides deterministic job submission, execution and finalization primitives across participating nodes.

## Zero-Config Webhosting

Applications and websites can be published as GNS services and resolved through GNS-native addressing.

A published service can be opened from ENTENCY UP through the `gns://` protocol without requiring a conventional web-hosting stack for the GNS resource itself.

---

# What Works Today

ENTENCY is still under active development, but the project has moved beyond a single-node architectural prototype.

Current implemented foundations include:

### Network

- local GNS node runtime
- multi-node connectivity
- peer discovery and peer state
- persistent node identity
- network topology inspection
- transport telemetry
- protocol and chain compatibility checks

### Data

- deterministic chunk generation
- chunk hashing and verification
- canonical object manifests
- object reconstruction
- distributed storage foundations
- cross-node retrieval foundations

### Services

- Storage foundations
- Communication Fabric foundations
- Streaming foundations
- Compute foundations
- Zero-Config Webhosting
- GNS service publication and resolution

### Trust & Control

- node identity
- reputation state
- delegated capabilities
- capability grant and revocation
- protected service operations
- signed compute voting
- deterministic compute finalization
- audit/event state

### ENTENCY UP Integration

- deterministic Session FSM
- protocol router
- `gns://` navigation
- integrated GNS node connectivity
- GNS resource resolution
- File Storage integration
- Zero-Config Webhosting deployment
- GNS-hosted site navigation
- node and peer monitoring
- network topology visibility
- installable local application support

### Tooling & Infrastructure

- GNS daemon
- GNS CLI
- explorer/indexer foundations
- rebuildable network read model
- deterministic build pipeline
- runtime ↔ node compatibility enforcement
- Windows x64 packaging
- Linux x64 packaging
- Linux ARM64 packaging

---

# Current Development Stage

The current focus is no longer proving that the basic architecture can exist.

The focus is turning the existing foundations into a resilient distributed network.

```text
Architecture Foundation          COMPLETE
        │
        ▼
Deterministic Data Layer         COMPLETE
        │
        ▼
Service Foundations              COMPLETE
        │
        ▼
Multi-Node Operation             ACTIVE
        │
        ▼
Network Hardening                ACTIVE
        │
        ▼
NAT Traversal                    PLANNED / IN DEVELOPMENT
        │
        ▼
Multi-Machine / Internet Tests   NEXT
        │
        ▼
Public Devnet                    FUTURE
        │
        ▼
Public Network                   FUTURE
```

Individual subsystems may remain experimental even when their architectural foundation is complete.

---

# Road to the Public Network

The next stage of ENTENCY GNS development focuses on removing assumptions that are acceptable in local development but not acceptable on a public distributed network.

Key areas include:

- NAT traversal
- nodes operating across independent physical networks
- internet-scale peer discovery
- connection recovery
- replication hardening
- multi-source retrieval hardening
- distributed failure recovery
- network partition handling
- resource accounting
- abuse resistance
- security hardening
- adversarial devnet testing
- long-running network stability testing
- observability and diagnostics
- public devnet deployment

The public network will only follow once these properties can be demonstrated through reproducible tests and evidence.

---

# Beyond the Core

ENTENCY UP and ENTENCY GNS form the current technical foundation.

Additional layers are planned around them.

## ENT

**ENT** is planned as the network resource and participation layer of GNS.

Its role is intended to include deterministic resource metering, network participation accounting and mechanisms associated with the consumption and provision of distributed resources.

ENT is **not part of the current production-ready core**.

---

## ENTENCY Wallet

ENTENCY Wallet is planned as the user-facing identity and network asset layer of the ecosystem.

Its exact production architecture will evolve alongside the GNS identity, capability and resource-accounting systems.

---

## ENTENCY AXI

**ENTENCY AXI** is the planned intelligence layer of the ENTENCY ecosystem.

AXI is intended to operate with GNS-native infrastructure rather than existing only as an external AI service.

Potential areas include:

- network intelligence
- distributed system observation
- anomaly detection
- routing assistance
- security intelligence
- resource optimization
- user-facing AI capabilities

AXI remains a future subsystem and is not represented as a completed capability.

---

# Future Service Domains

The common GNS service architecture is intended to support additional distributed workloads over time.

One planned area is a **Game Backend** service layer.

The objective is not to build infrastructure for one specific game, but to explore whether multiplayer and persistent game services can use the same GNS network primitives used by other distributed applications.

Other service domains may be added as the protocol evolves.

---

# Architecture Principles

ENTENCY development follows several core principles.

### Determinism

Equivalent inputs should produce equivalent identities and verifiable results wherever the protocol requires deterministic behavior.

### Protocol Before Convenience

Network behavior should be defined by explicit contracts rather than accidental implementation behavior.

### Reproducibility

Builds, tests and network behavior should be reproducible whenever technically possible.

### Capability-Based Authority

Sensitive operations should require explicit authority rather than implicit trust.

### Separation of Control and Execution

ENTENCY UP controls user-facing execution and session state.

ENTENCY GNS provides distributed network infrastructure.

### Evidence Before Claims

A milestone is not considered complete simply because code exists.

Implementation, tests and reproducible evidence are expected to agree.

---

# Development Philosophy

Infrastructure defines what becomes possible above it.

Browsers transformed access to information.

Cloud platforms transformed access to computation.

Distributed systems changed how ownership, availability and trust can be modeled.

ENTENCY explores the next question:

> **What happens when browsing, execution, storage, communication, compute and distribution become parts of one interoperable architecture?**

That question is what ENTENCY UP and ENTENCY GNS are being built to answer.

---

# Project Status

ENTENCY is under active foundational development.

The project currently operates primarily as a development network and experimental execution environment.

Some architectural components are implemented and tested, while public-network operation, production hardening and several ecosystem layers remain under development.

The project intentionally distinguishes between:

**Implemented** — functionality exists in the codebase.

**Validated** — functionality has reproducible tests or runtime evidence.

**Experimental** — functionality exists but requires further distributed testing or hardening.

**Planned** — architectural direction only; not presented as an existing capability.

---

# Repository

This repository is the public entry point to the ENTENCY ecosystem.

Detailed implementation, protocol specifications, milestone evidence and component documentation are maintained alongside the active development repositories and specifications.

The core engine remains closed during active foundational development.

---

<p align="center">
  <strong>ENTENCY</strong><br>
  <sub>Built with intent.</sub>
</p>
