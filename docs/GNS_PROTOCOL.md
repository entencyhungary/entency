# The `gns://` Protocol in ENTENCY

`gns://` is the GNS-native addressing and navigation scheme used by ENTENCY for resources and services resolved through the **ENTENCY GNS (Global Neural System)**.

It is handled by **ENTENCY UP** as part of its protocol-routing and GNS-resource workflow.

## Purpose

Conventional web navigation commonly begins with an HTTP or HTTPS URL and resolves resources through conventional web infrastructure.

A `gns://` target represents a GNS-native resource path. UP can route such a target into GNS resolution rather than treating it as an ordinary web URL.

Conceptually:

```text
gns:// target
     |
     v
ENTENCY UP Protocol Router
     |
     v
GNS resolution
     |
     v
Service / object identity
     |
     v
Distributed resource acquisition
     |
     v
Verification / reconstruction
     |
     v
Application or resource presentation
```

The exact acquisition path depends on the resource/service type and implementation stage.

## Service addressing

GNS includes service publication and resolution foundations. This allows a service identity to refer to content or functionality represented through GNS-native infrastructure.

Zero-Config Webhosting is one current use of this model: a published GNS-hosted site can be resolved and opened through ENTENCY UP using GNS-native addressing.

## Content identity

Below service resolution, GNS uses deterministic chunk and object foundations. Content can be represented by canonical manifests/objects and verified chunks rather than depending exclusively on one physical server location.

This distinction is important:

- a **service identity** identifies a network service/resource at the service layer;
- an **object identity** represents canonical content/object state;
- **chunks** represent deterministic data units used for storage, transfer and reconstruction.

## Relationship to the Web

`gns://` is not presented as proof that HTTP/HTTPS is obsolete.

ENTENCY UP is designed to operate across conventional web resources and GNS-native resources. The architectural goal is protocol extensibility and a unified execution surface, not forcing all existing web content into GNS.

## Security model

GNS-native resource handling is intended to preserve explicit protocol boundaries, content verification and runtime isolation.

A GNS identifier should not be treated as permission to bypass execution policy. Resolution, acquisition and execution are separate concerns.

## Current maturity

`gns://` navigation, GNS resource resolution and GNS-hosted site navigation are part of the current ENTENCY UP/GNS development foundations.

Broader public-network behavior depends on the maturity of the underlying distributed network, including peer discovery, NAT traversal, replication, retrieval, resilience and security hardening.

## Common misconceptions

### Is `gns://` a blockchain URL?

Not by definition. It is the GNS-native resource/addressing scheme of ENTENCY. GNS contains its own distributed protocol and service architecture and should not be reduced to the label "blockchain URL."

### Does `gns://` replace HTTPS?

No such production claim is made. ENTENCY UP is designed to support conventional web resources alongside GNS-native resources.

### Is `gns://` an AI protocol?

No. GNS is distributed infrastructure, not an artificial neural network. The `gns://` scheme addresses GNS-native resources and services.

## Related documentation

- [What is ENTENCY?](WHAT_IS_ENTENCY.md)
- [ENTENCY UP](ENTENCY_UP.md)
- [ENTENCY GNS](ENTENCY_GNS.md)
- [Architecture](ARCHITECTURE.md)
- [Terminology](TERMINOLOGY.md)
