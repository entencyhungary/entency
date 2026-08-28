# ENTENCY Architecture

ENTENCY is organized around a deliberate separation between **user-facing execution and control** and **distributed network infrastructure**.

The two current core systems are **ENTENCY UP** and **ENTENCY GNS**.

## System overview

```text
+------------------------------------------------------+
|                     ENTENCY UP                       |
|                                                      |
|              Browser + Workstation                   |
|                                                      |
| Session Control | Protocol Routing | Local Apps      |
| Runtime Isolation | GNS Navigation | Service Access  |
+---------------------------+--------------------------+
                            |
                            | gns:// / service interaction
                            v
+------------------------------------------------------+
|                    ENTENCY GNS                       |
|                 Global Neural System                 |
|                                                      |
| Identity | Transport | Objects | Services | Trust    |
|                                                      |
| Storage | Communication | Streaming | Compute        |
| Zero-Config Webhosting                               |
+------------------------------------------------------+
```

## ENTENCY UP: execution and control surface

UP owns the user-facing execution environment. Its responsibilities include Browser and Workstation interaction, deterministic session lifecycle management, protocol routing, runtime isolation and access to GNS-native services.

A formal Session FSM separates execution state from visual tab state. This is intended to make redirects, reconnects, backgrounding, failures and termination deterministic at the control layer.

## ENTENCY GNS: distributed infrastructure

GNS owns distributed network responsibilities. Its foundations include node identity and transport, deterministic chunks and objects, service infrastructure, trust/control mechanisms and distributed service classes.

GNS is not an artificial neural network. The term Global Neural System refers to the network architecture.

## Data path

A simplified GNS-native resource flow can be represented as:

```text
User action
   |
   v
ENTENCY UP
   |
Protocol routing / gns:// resolution
   |
   v
GNS service identity
   |
   v
Object / manifest identity
   |
   v
Chunk acquisition / verification
   |
   v
Runtime reconstruction / presentation
```

Exact behavior depends on the service and implementation stage, but the architectural principle is that protocol-defined identities and verifiable content sit between user-facing execution and distributed resources.

## Service architecture

GNS is being developed as common infrastructure for multiple service classes rather than as a separate network for each workload.

Current service domains include foundations for:

- Storage
- Communication
- Streaming
- Compute
- Zero-Config Webhosting

Additional service domains may be introduced as the protocol evolves.

## Trust and authority

ENTENCY favors explicit authority and reproducible state.

Relevant GNS foundations include:

- node identity;
- reputation state;
- delegated capabilities;
- capability grant and revocation;
- protected operations;
- signed compute voting;
- deterministic compute finalization;
- auditable event/read-model foundations.

These mechanisms do not imply that all public-network security problems are solved. Public operation still requires hardening, abuse resistance and adversarial testing.

## Architectural principles

### Determinism

Equivalent inputs should produce equivalent identities and verifiable results wherever the protocol requires deterministic behavior.

### Protocol before convenience

Network behavior should be defined through explicit contracts rather than accidental implementation behavior.

### Separation of control and infrastructure

UP controls user-facing execution and session state. GNS provides distributed infrastructure.

### Capability-based authority

Sensitive operations should require explicit authority rather than implicit trust.

### Reproducibility

Builds, tests and network behavior should be reproducible wherever technically possible.

### Evidence before claims

Architecture, implementation and validation are different things. Public documentation should state which one supports a capability.

## Ecosystem extensions

The current technical foundation is UP + GNS. Additional planned layers include:

- **ENT** — planned network resource and participation layer;
- **ENTENCY Wallet** — planned identity/network-asset layer;
- **ENTENCY AXI** — planned intelligence layer.

These planned components must not be treated as completed capabilities of the current core.

## Related documentation

- [What is ENTENCY?](WHAT_IS_ENTENCY.md)
- [ENTENCY UP](ENTENCY_UP.md)
- [ENTENCY GNS](ENTENCY_GNS.md)
- [Capabilities](CAPABILITIES.md)
- [GNS Protocol](GNS_PROTOCOL.md)
- [Terminology](TERMINOLOGY.md)
