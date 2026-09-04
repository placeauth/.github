<p align="center">
  <img src="https://placeauth.org/assets/png/horizontal/placeauth-horizontal-light-transparent-1200x300.png" alt="PlaceAuth" width="500">
</p>


<p align="center">
  <strong>A common language for machines and places.</strong>
</p>

<p align="center">
  Open interoperability infrastructure for autonomous systems operating in physical environments.
</p>

<p align="center">
  <a href="https://placeauth.org/">
    <img src="https://img.shields.io/badge/Website-PlaceAuth.org-1f3b4d" alt="Website">
  </a>
  <a href="https://github.com/placeauth/spatial-policy-protocol/blob/main/docs/whitepaper.md">
    <img src="https://img.shields.io/badge/White%20Paper-From%20Permission%20to%20Admission-4b5563" alt="White Paper">
  </a>
  <a href="https://github.com/placeauth/spatial-policy-protocol/releases/tag/v0.1.0-experimental-preview">
    <img src="https://img.shields.io/badge/SPP-0.1.0%20Experimental-6b7280" alt="SPP 0.1.0 Experimental Preview">
  </a>
  <a href="https://github.com/placeauth/spatial-policy-protocol/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-Apache%202.0-0f766e" alt="Apache 2.0">
  </a>
</p>

---

## Spatial Policy Protocol

PlaceAuth develops the **Spatial Policy Protocol (SPP)**, an experimental interoperability layer that allows physical environments to express operating requirements, autonomous systems to demonstrate conformance, and both sides to establish evidence-backed operating profiles.

> **The place defines the requirements.**  
> **The machine demonstrates conformance.**  
> **SPP establishes the operating profile.**

```text
PHYSICAL ENVIRONMENT
"What must be true here?"
        │
        ▼
PLACE REQUIREMENTS
        │
        ▼
CONFORMANCE
        │
        ▼
EVIDENCE
        │
        ▼
ADMISSION PROFILE
        │
        ▼
AUTONOMOUS OPERATION
```

## Protocol Model

| Layer | Purpose |
|---|---|
| **SPP Core** | Place requirements, policy semantics, hierarchy, and operating constraints |
| **SPP Conformance** | Requirement-to-test mapping, evidence generation, and assurance |
| **SPP Admission** | Admission decisions, degraded operation, spatial transitions, and selective requalification |

## What SPP Explores

### Place-defined requirements

Physical environments can describe machine-readable conditions governing autonomous operation, such as:

- maximum speed
- human separation
- sensing restrictions
- recording and retention
- manipulation constraints
- infrastructure interaction
- space-specific operating conditions

### Conformance

An autonomous system can demonstrate whether it satisfies applicable requirements using conformance plans and executable tests.

### Evidence

SPP can associate demonstrated guarantees with evidence tied to relevant system, policy, configuration, and environmental state.

### Admission profiles

A resulting operating profile may be:

| Result | Meaning |
|---|---|
| **ADMITTED** | Applicable requirements are satisfied |
| **DEGRADED** | Operation is allowed under additional restrictions |
| **DENIED** | Required guarantees could not be established |

### Spatial transitions

Different spaces may impose different requirements.

SPP explores **selective requalification**, where evidence that remains sufficient can be reused and only new, stricter, unresolved, or invalidated requirements need additional conformance.

```text
CURRENT EVIDENCE
      +
DESTINATION REQUIREMENTS
      │
      ▼
REQUIREMENT DELTA
      │
      ├── Reuse still-sufficient evidence
      └── Requalify changed requirements
      │
      ▼
UPDATED OPERATING PROFILE
```

## Current Status

> **SPP 0.1.0 Experimental Preview**
>
> PlaceAuth is currently in an experimental, pre-standardization phase. The project is intended for technical evaluation, interoperability research, and early implementation work.

The current reference implementation includes:

- reference policy evaluation
- evidence-based admission
- deterministic conformance scenarios
- evidence binding and replay checks
- FastAPI reference services
- OPA/Rego integration
- ROS 2 enforcement integration stub
- JSON schemas and example policies

SPP should not currently be treated as a production safety or security system.

## Open by Design

PlaceAuth is intended to complement existing robotics and infrastructure systems rather than replace them.

SPP may sit alongside technologies such as:

- ROS 2
- Nav2
- Open-RMF
- building automation systems
- fleet managers
- identity systems
- policy engines
- localization systems
- attestation technologies

The protocol and reference implementation are available under the **Apache License 2.0**.

## Explore

| Resource | Link |
|---|---|
| 🌐 **PlaceAuth.org** | [placeauth.org](https://placeauth.org/) |
| 📖 **White Paper** | [From Permission to Admission](https://github.com/placeauth/spatial-policy-protocol/blob/main/docs/whitepaper.md) |
| ⚙️ **Spatial Policy Protocol** | [github.com/placeauth/spatial-policy-protocol](https://github.com/placeauth/spatial-policy-protocol) |
| 🧪 **Experimental Release** | [SPP 0.1.0 Experimental Preview](https://github.com/placeauth/spatial-policy-protocol/releases/tag/v0.1.0-experimental-preview) |

## Technical Feedback

PlaceAuth welcomes review from people working in:

- robotics
- autonomous systems
- ROS 2 and fleet management
- smart buildings
- physical infrastructure
- security and attestation
- interoperability
- standards development

Useful feedback includes:

- protocol design concerns
- interoperability gaps
- implementation proposals
- threat-model observations
- deployment assumptions
- integration ideas
- overlapping prior systems or standards

<details>
<summary><strong>What kind of review is most useful?</strong></summary>

We are especially interested in where the model:

- overlaps existing infrastructure
- introduces unnecessary complexity
- makes unrealistic deployment assumptions
- lacks important trust or enforcement mechanisms
- could integrate cleanly with real robotics and facility systems

Critical technical feedback is welcome.

</details>

## Contact

**General inquiries**  
hello@placeauth.org

**Standards & interoperability**  
standards@placeauth.org

**Security**  
security@placeauth.org

---

<p align="center">
  <sub>Certain technologies described by PlaceAuth are patent pending.</sub>
</p>
