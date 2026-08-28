# ENTENCY UP

## Browser and Workstation for the ENTENCY ecosystem

**ENTENCY UP** is the user-facing Browser, Workstation and execution environment of ENTENCY.

It is designed to provide a unified surface for conventional web resources, local applications and services operating through the **ENTENCY GNS (Global Neural System)**.

UP is not the GNS node network itself. Its primary responsibility is user-facing execution, session control, protocol routing and interaction with network services.

## Core model

ENTENCY UP combines several responsibilities that are normally separated across different applications:

- browser functionality;
- workstation functionality;
- deterministic session lifecycle control;
- protocol routing;
- `gns://` resource navigation;
- runtime isolation;
- local application execution;
- GNS node connectivity;
- GNS service interaction;
- network and service inspection.

## Deterministic session lifecycle

UP uses a formal Session FSM to keep protocol and execution state independent from purely visual tab state.

The normative lifecycle states are:

```text
IDLE
ROUTING
ACQUIRING
ACTIVE
BACKGROUND
GC_PENDING
TERMINATING
TERMINATED
```

This separation allows redirects, reconnects, backgrounding, protocol failures and termination to be handled through explicit transitions rather than accidental UI behavior.

Important invariants include:

- `TERMINATED` has no outgoing transition;
- UI events do not directly terminate a session;
- a terminal protocol event always enters `TERMINATING` before `TERMINATED`.

## Protocol routing

UP is designed as a multi-protocol environment rather than a browser tied to one resource type.

For GNS-native resources, UP provides `gns://` navigation and resolution. Conventional web access remains a separate supported resource path; GNS is intended to extend the execution environment rather than require the conventional Web to disappear.

## Browser and Workstation

The Browser and Workstation are complementary execution surfaces.

The Browser provides navigation-oriented interaction with resources and services. The Workstation provides a broader environment for applications, tools, local execution and network-aware workflows.

Together they form the primary user-facing layer of ENTENCY.

## Relationship to GNS

```text
ENTENCY UP
Browser + Workstation
        |
        | protocol/service interaction
        v
ENTENCY GNS
Distributed node infrastructure
```

UP controls user-facing execution and session state. GNS provides distributed network infrastructure beneath it.

## Current public status

The current development foundations include deterministic session control, protocol routing, GNS navigation, GNS node connectivity, resource resolution, file-storage integration, GNS-hosted site navigation, node/peer monitoring, network topology visibility and installable local application support.

Individual features remain subject to development, distributed testing and hardening. The existence of an architectural interface does not by itself mean that every planned protocol or ecosystem feature is production ready.

## What ENTENCY UP is not

ENTENCY UP should not be described as:

- the GNS network itself;
- merely a skin or dashboard for a node;
- a distributed neural-processing engine;
- a production-ready replacement for every existing browser or operating system;
- a generic distributed task substrate.

The most useful short description is:

> **ENTENCY UP is the Browser and Workstation that provides the user-facing execution and control surface of the ENTENCY ecosystem.**

## Related documentation

- [What is ENTENCY?](WHAT_IS_ENTENCY.md)
- [ENTENCY GNS](ENTENCY_GNS.md)
- [Architecture](ARCHITECTURE.md)
- [Capabilities](CAPABILITIES.md)
- [GNS Protocol](GNS_PROTOCOL.md)
- [Terminology](TERMINOLOGY.md)
