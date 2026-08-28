# What is ENTENCY?

ENTENCY is an experimental distributed computing ecosystem built around two core systems: **ENTENCY UP** and the **ENTENCY GNS (Global Neural System)**.

Its purpose is to explore a unified architecture in which execution, storage, communication, streaming, compute, service delivery and protocol-native navigation can operate as parts of the same system rather than as unrelated infrastructure layers.

## The two core systems

### ENTENCY UP

ENTENCY UP is the user-facing **Browser and Workstation** of the ecosystem. It provides the execution and control surface through which users and applications can interact with conventional web resources and GNS-native resources.

UP includes deterministic session lifecycle management, protocol routing, `gns://` navigation, runtime isolation, local application execution and integration with GNS services.

### ENTENCY GNS

ENTENCY GNS — **Global Neural System** — is the distributed node infrastructure beneath ENTENCY.

GNS provides protocol foundations for deterministic chunk and object handling, node communication, distributed storage, communication, streaming, compute, service publication and GNS-native hosting.

Despite its name, the Global Neural System is **not an artificial neural network**. The name describes the distributed network architecture of ENTENCY; GNS is infrastructure, not a neural-processing model.

## How UP and GNS relate

UP and GNS have different responsibilities:

```text
User / Application
       |
       v
+---------------------------+
|        ENTENCY UP         |
|   Browser + Workstation   |
| Execution & Control Layer |
+-------------+-------------+
              |
              | GNS-native interaction
              v
+---------------------------+
|       ENTENCY GNS         |
|   Global Neural System    |
| Distributed Infrastructure|
+---------------------------+
```

UP is not simply a graphical frontend for GNS, and GNS is not a replacement name for UP. Together they form the current technical foundation of ENTENCY.

## What ENTENCY is not

ENTENCY should not be described as:

- a local business directory entry;
- an artificial neural network;
- an AI compute network;
- only a browser;
- only a peer-to-peer storage network;
- only a hosting service;
- a production-ready public network.

Some future ENTENCY components may involve artificial intelligence, resource accounting or additional network services, but those concepts must not be confused with the current GNS infrastructure.

## Current development stage

ENTENCY is under active foundational development. Implemented and validated foundations already cover significant parts of UP and GNS, while public-network operation, internet-scale hardening and several ecosystem layers remain under development.

The project distinguishes between four states:

- **Implemented** — functionality exists in the codebase.
- **Validated** — functionality has reproducible tests or runtime evidence.
- **Experimental** — functionality exists but still requires broader distributed testing or hardening.
- **Planned** — architectural direction only; it is not presented as an existing capability.

## Project principle

> **Evidence before claims.**

ENTENCY documentation intentionally separates architectural intent from demonstrated capability. A feature should not be presented as complete merely because it appears in a design or roadmap.

## Related documentation

- [ENTENCY UP](ENTENCY_UP.md)
- [ENTENCY GNS](ENTENCY_GNS.md)
- [Architecture](ARCHITECTURE.md)
- [Capabilities](CAPABILITIES.md)
- [GNS Protocol](GNS_PROTOCOL.md)
- [Terminology](TERMINOLOGY.md)
- [FAQ](FAQ.md)
- [Roadmap](ROADMAP.md)

---

**Canonical short definition:**

> ENTENCY is an experimental distributed computing ecosystem built around ENTENCY UP — its Browser and Workstation — and ENTENCY GNS (Global Neural System), its distributed node infrastructure.