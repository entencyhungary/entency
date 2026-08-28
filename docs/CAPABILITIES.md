# ENTENCY Capabilities

This document provides a public, evidence-aware view of ENTENCY capabilities.

ENTENCY intentionally distinguishes between architecture, implementation and validation. A feature appearing in a specification or roadmap does not automatically mean that it is available as a production capability.

## Status vocabulary

| Status | Meaning |
|---|---|
| **Implemented** | Functionality exists in the active codebase. |
| **Validated** | Functionality has reproducible tests and/or runtime evidence. |
| **Experimental** | Functionality exists but still requires broader distributed testing or hardening. |
| **Planned** | Architectural direction only; not presented as an existing capability. |

A subsystem may reasonably be both implemented and experimental. These labels describe different dimensions rather than a single marketing maturity level.

## ENTENCY GNS foundations

### Data and identity

The current project publicly identifies implemented foundations for:

- deterministic chunk generation;
- chunk hashing and verification;
- canonical object/manifest identities;
- object reconstruction;
- persistent node identity;
- distributed-storage foundations;
- cross-node retrieval foundations.

### Network

Current foundations include:

- local GNS node runtime;
- multi-node connectivity;
- peer discovery and peer state;
- network topology inspection;
- transport telemetry;
- protocol/chain compatibility checks.

Local multi-node operation has been demonstrated, while broader independent-network and internet-scale operation remains an active development area.

### Services

Implemented foundations exist for:

- Storage;
- Communication Fabric;
- Streaming;
- Compute;
- Zero-Config Webhosting;
- GNS service publication and resolution.

The maturity of individual service paths varies. The existence of a service foundation must not be interpreted as a claim of internet-scale production readiness.

### Trust and control

Current foundations include:

- reputation state;
- delegated capabilities;
- capability grant and revocation;
- protected service operations;
- signed compute voting;
- deterministic compute finalization;
- audit/event state and rebuildable read-model foundations.

## ENTENCY UP foundations

Current public project documentation identifies foundations for:

- deterministic Session FSM;
- protocol routing;
- `gns://` navigation;
- GNS node connectivity;
- GNS resource resolution;
- File Storage integration;
- Zero-Config Webhosting deployment;
- GNS-hosted site navigation;
- node and peer monitoring;
- network topology visibility;
- installable local application support.

## Tooling and release infrastructure

Current foundations include:

- GNS daemon;
- GNS CLI;
- explorer/indexer foundations;
- rebuildable network read model;
- deterministic build pipeline;
- runtime/node compatibility enforcement;
- Windows x64 packaging;
- Linux x64 packaging;
- Linux ARM64 packaging.

## Experimental / hardening areas

The following areas require further distributed validation and/or hardening before a public-network production claim would be appropriate:

- operation across independent physical networks;
- internet-scale peer discovery;
- NAT traversal;
- long-running connection recovery;
- replication hardening;
- multi-source retrieval hardening;
- network partition handling;
- abuse resistance;
- adversarial devnet testing;
- long-running network stability;
- public devnet deployment.

## Planned ecosystem capabilities

The following should currently be treated as planned ecosystem direction rather than completed production capabilities:

### ENT

ENT is planned as the network resource and participation layer, associated with resource metering and participation accounting.

### ENTENCY Wallet

ENTENCY Wallet is planned as a user-facing identity and network-asset layer.

### ENTENCY AXI

ENTENCY AXI is the planned intelligence layer of the ecosystem. Potential directions include network observation, anomaly detection, security intelligence, routing assistance, resource optimization and user-facing AI functionality.

### Additional service domains

Additional distributed service domains, including a future Game Backend layer, may be explored on top of common GNS primitives.

## Production-readiness statement

**ENTENCY is not currently represented as a production-ready public network.**

The project is in active development and validation. Public-network operation follows only after the relevant distributed, security, resilience and operational properties can be demonstrated through reproducible evidence.

## Claim policy

A public capability claim should answer three questions:

1. **Is it implemented?**
2. **Has it been validated?**
3. **What limitations remain?**

If those questions cannot be answered, the capability should be described as experimental or planned rather than complete.

## Related documentation

- [What is ENTENCY?](WHAT_IS_ENTENCY.md)
- [Architecture](ARCHITECTURE.md)
- [ENTENCY UP](ENTENCY_UP.md)
- [ENTENCY GNS](ENTENCY_GNS.md)
- [Roadmap](ROADMAP.md)
