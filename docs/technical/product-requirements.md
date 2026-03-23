# Product Requirements Document (PRD)

> **Status**: Draft — to be completed after market study segment ranking

## 1. Overview

<!-- Product name, vision, target segment (TBD from market study) -->
<!-- MVP scope definition -->

## 2. Target Users

<!-- Primary persona (from value-propositions.md) -->
<!-- Secondary persona -->

## 3. User Stories

### Farmer / Primary User

<!-- As a dairy farmer, I want to... so that... -->
<!-- As a farmer, I want to set a virtual fence boundary so that my cattle stay in the designated pasture -->
<!-- As a farmer, I want to receive alerts when an animal leaves the boundary so that I can act quickly -->
<!-- As a farmer, I want to monitor herd health metrics so that I can detect illness early -->
<!-- As a farmer, I want to schedule grazing rotations so that pasture utilization improves -->

### System Administrator

<!-- As an admin, I want to manage multiple farms so that... -->

## 4. Functional Requirements

### MVP (v1.0)

<!-- FR-001: GPS tracking with position updates every X seconds -->
<!-- FR-002: Virtual fence boundary creation via mobile app -->
<!-- FR-003: Audio + vibration cues when animal approaches boundary -->
<!-- FR-004: Real-time alerts when animal breaches boundary -->
<!-- FR-005: Basic health metrics (activity level, rest patterns) -->
<!-- FR-006: Mobile app with map view (French + English) -->
<!-- FR-007: Collar battery status and solar charge monitoring -->

### Future (v2.0+)

<!-- FR-100: ML-based health anomaly detection -->
<!-- FR-101: Automated grazing rotation scheduling -->
<!-- FR-102: Herd analytics dashboard -->
<!-- FR-103: Integration with existing farm management software -->

## 5. Hardware Specifications

| Spec                         | Target                       | Minimum Acceptable |
| ---------------------------- | ---------------------------- | ------------------ |
| Weight                       | g                            | g                  |
| Battery life (summer)        | days                         | days               |
| Battery life (winter, –30°C) | days                         | days               |
| IP rating                    | IP67                         | IP65               |
| Operating temp range         | –40°C to +50°C               | –30°C to +45°C     |
| GPS accuracy                 | m                            | m                  |
| Solar recharge rate          | hrs full sun for full charge |                    |
| Collar attachment            |                              |                    |

## 6. Software Specifications

| Spec                    | Target                               |
| ----------------------- | ------------------------------------ |
| Position update latency | < X seconds                          |
| App platforms           | iOS + Android                        |
| Languages               | French, English                      |
| Offline support         | Yes — sync when connectivity returns |
| API                     | RESTful for third-party integrations |
| Data retention          | X months                             |

## 7. Non-Functional Requirements

<!-- NFR-001: System uptime ≥ 99.5% -->
<!-- NFR-002: Position data latency < X seconds -->
<!-- NFR-003: Support up to X collars per farm -->
<!-- NFR-004: Data encrypted in transit (TLS 1.3) and at rest (AES-256) -->
<!-- NFR-005: PIPEDA + Law 25 compliant data handling -->

## 8. Out of Scope for MVP

<!-- What we explicitly will NOT build in v1 -->

## 9. Success Metrics

<!-- Collar uptime % -->
<!-- Virtual fence breach reduction % -->
<!-- Farmer satisfaction (NPS) -->
<!-- Hardware failure rate -->
