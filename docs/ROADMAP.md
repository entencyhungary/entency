# ENTENCY Public Roadmap

This roadmap describes development direction, not promises of release dates.

ENTENCY uses an evidence-first development model: a planned capability becomes a demonstrated capability only when implementation and reproducible validation support the claim.

## Current foundation

The current technical foundation is built around:

- **ENTENCY UP** — Browser, Workstation, session control and protocol execution surface;
- **ENTENCY GNS** — distributed node, data/object and service infrastructure.

Implemented foundations already span deterministic data handling, GNS service primitives, multi-node development operation, trust/control mechanisms, UP integration and cross-platform packaging.

## Development path

```text
Architecture Foundation
        |
        v
Deterministic Data / Object Layer
        |
        v
Service Foundations
        |
        v
Multi-Node Development Operation
        |
        v
Network Hardening
        |
        v
NAT / Independent-Network Operation
        |
        v
Multi-Machine and Internet Validation
        |
        v
Public Devnet
        |
        v
Public Network
```

The diagram represents progression, not a claim that every item above an active stage is uniformly production complete.

## Near-term network priorities

Important development areas on the road toward broader network operation include:

- NAT traversal;
- nodes operating across independent physical networks;
- internet-scale peer discovery;
- reconnect and recovery behavior;
- replication hardening;
- multi-source retrieval hardening;
- distributed failure recovery;
- network partition handling;
- observability and diagnostics;
- long-running stability testing.

## Security and resilience

Before public-network operation, the architecture requires continued work on:

- abuse resistance;
- adversarial devnet testing;
- capability/policy enforcement validation;
- malformed/hostile input handling;
- resource exhaustion behavior;
- failure isolation;
- reproducible security evidence.

## Service evolution

Existing GNS service foundations will continue to mature across:

- Storage;
- Communication;
- Streaming;
- Compute;
- Zero-Config Webhosting.

Future service domains may reuse the same common GNS primitives rather than creating unrelated network stacks.

One planned exploration area is a distributed **Game Backend** service layer.

## Ecosystem layers

### ENT

ENT is planned as the GNS network resource and participation layer, associated with resource metering and participation accounting.

### ENTENCY Wallet

ENTENCY Wallet is planned as a user-facing identity and network-asset layer.

### ENTENCY AXI

ENTENCY AXI is the planned intelligence layer. Potential directions include network observation, anomaly detection, security intelligence, routing assistance, resource optimization and user-facing AI functionality.

These ecosystem layers are not represented as completed production capabilities merely by appearing on this roadmap.

## Public devnet gate

A public devnet should follow demonstrated progress in the properties required for meaningful distributed testing, including independent-network connectivity, recovery, replication/retrieval behavior, observability and security controls.

## Public network gate

A production public network requires stronger evidence than a working development network.

Relevant properties include:

- reproducible distributed behavior;
- resilience under node/network failure;
- secure authority boundaries;
- abuse/resource controls;
- long-running stability;
- operational diagnostics;
- validated release and compatibility behavior.

## No artificial deadlines

ENTENCY does not need to claim a public-network date before the engineering evidence supports one.

The roadmap is therefore capability-driven rather than calendar-driven.

## Related documentation

- [Capabilities](CAPABILITIES.md)
- [Architecture](ARCHITECTURE.md)
- [ENTENCY GNS](ENTENCY_GNS.md)
- [ENTENCY UP](ENTENCY_UP.md)
