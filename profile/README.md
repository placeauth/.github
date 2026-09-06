<p align="center">
  <img src="https://github.com/placeauth/.github/blob/main/profile/assets/placeauth-logo-github-readme.png" alt="PlaceAuth" width="500">
</p>

<p align="center">
  <strong>Open infrastructure for interoperability between autonomous systems and physical environments.</strong>
</p>

<p align="center">
  <a href="https://placeauth.org/"><img src="https://img.shields.io/badge/Website-PlaceAuth.org-1f3b4d" alt="Website"></a>
  <a href="https://github.com/placeauth/spatial-policy-protocol/blob/main/docs/whitepaper.md"><img src="https://img.shields.io/badge/Whitepaper-From%20Permission%20to%20Admission-4b5563" alt="Whitepaper"></a>
  <a href="https://github.com/placeauth/spatial-policy-protocol/releases/tag/v0.2.0-experimental-preview"><img src="https://img.shields.io/badge/SPP-v0.2.0%20Experimental%20Preview-6b7280" alt="SPP v0.2.0 Experimental Preview"></a>
  <a href="https://github.com/placeauth/spatial-policy-protocol/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Apache%202.0-0f766e" alt="Apache 2.0"></a>
</p>

---

## Spatial Policy Protocol

PlaceAuth develops the **Spatial Policy Protocol (SPP)**: an experimental, vendor-neutral interoperability layer for place-defined operating requirements, autonomous-system conformance, and evidence-backed operating profiles.

> **The place defines the requirements.**  
> **The machine demonstrates conformance.**  
> **SPP establishes the operating profile.**

```text
PLACE REQUIREMENTS
        →
CONFORMANCE PLAN
        →
EVIDENCE
        →
ADMISSION PROFILE
        →
PHYSICAL OPERATION
```

## Current release

**[SPP v0.2.0 Experimental Preview](https://github.com/placeauth/spatial-policy-protocol/releases/tag/v0.2.0-experimental-preview)** is the current public reference implementation release.

- Reference implementation: **0.2.0**
- Normative protocol specification: **SPP 0.1**
- Dependency-free reference suite: **186 passed, 4 skipped**

SPP remains experimental and pre-standardization. It is not an industry standard or a production safety platform.

## What it includes

- place-defined operating requirements
- evidence-based admission, sufficiency assessment, and admission-time revalidation
- signed evidence with local trusted-issuer verification
- selective requalification across spatial transitions
- embodiment-specific conformance mapping
- deterministic decision traces with `spp-explain`
- ROS 2/Nav2 enforcement integration
- Open-RMF task-eligibility adapter

## Concrete validation

**Nav2 runtime behavior.** SPP demonstrated an evidence-backed operating profile changing navigation speed behavior of a running Nav2 robot from **1.0 m/s → 0.5 m/s** under one active `FollowPath` goal. The bounded validation exercised ROS 2 Humble, Nav2 `ControllerServer`, and stock Regulated Pure Pursuit. It is not a physical safety validation claim.

**Open-RMF adapter boundary.** Task eligibility is gated at `FleetUpdateHandle.consider_delivery_requests`. The adapter boundary was validated; no live Open-RMF runtime validation is claimed.

## Explore

| Resource | Link |
|---|---|
| Spatial Policy Protocol | [github.com/placeauth/spatial-policy-protocol](https://github.com/placeauth/spatial-policy-protocol) |
| SPP v0.2 release | [SPP v0.2.0 Experimental Preview](https://github.com/placeauth/spatial-policy-protocol/releases/tag/v0.2.0-experimental-preview) |
| Whitepaper | [From Permission to Admission](https://github.com/placeauth/spatial-policy-protocol/blob/main/docs/whitepaper.md) |
| Technical Review | [Read the technical review](https://github.com/placeauth/spatial-policy-protocol/blob/main/docs/technical-review.md) |
| Website | [placeauth.org](https://placeauth.org/) |

## Technical feedback

Critical technical feedback on protocol design, deployment assumptions, trust boundaries, interoperability, and overlapping systems is welcome through the [Technical Review](https://github.com/placeauth/spatial-policy-protocol/blob/main/docs/technical-review.md).

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
