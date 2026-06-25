# 🏗️ OFFSITE — Drone-Based Construction Visibility Platform

> A project management case study applying PMI's five-phase lifecycle to an offsite drone-based construction monitoring system — complete with full documentation, a feasibility report template, and a presentation deck.

---

## 📁 Project Resources

This repository is accompanied by two ready-to-use project management resources:

| Resource | Description |
|---|---|
| 📄 [Project Report](./ProjectManagement_ConstructionVisibilityDroneBased_Report.docx) | Full final project report — covers all PM phases, WBS, RACI Matrix, risk register, financial plan, stakeholder analysis, and technical architecture |
| 📊 [Presentation Deck](./ProjectManagement_ConstructionVisibilityDroneBased_Presentation.pptx) | Slide deck summarizing the platform, problem statement, roadmap, tech stack, and financial plan |
| 📋 [Feasibility Report Template](./ProjectManagement_ConstructionFeasibility_Template.pdf) | Reusable template for conducting feasibility studies on similar construction technology projects |

---

## Overview

**OFFSITE** is an integrated offsite construction management platform proposed and managed using engineering project management principles taught at Northeastern University (EMGT 5220). The project addresses persistent construction industry failures — 98% of megaprojects face cost or schedule overruns, 53% finish late, and 66% go over budget — by combining drone and LiDAR data acquisition, cloud processing, and an interactive 3D dashboard into a single visibility platform.

The project is documented end-to-end as a PM deliverable: from initiation and stakeholder mapping through execution planning, risk management, budgeting, and closure.

---

## 📋 Project Management Framework

This project follows **PMI's five-phase project lifecycle**, applied rigorously across all work streams.

### Phase 1 — Initiation
- Technical and operational feasibility study (scalability, integration, data security)
- Stakeholder identification across primary, secondary, and tertiary groups
- Scope and success criteria definition
- FAA drone regulation compliance review
- Initial site mapping and requirement baselining

### Phase 2 — Planning
- Detailed Work Breakdown Structure (WBS) — see [Appendix A of the report]
- System architecture design (Flutter, React, Node.js, Flask, AWS)
- RACI Matrix defining Responsible / Accountable / Consulted / Informed for every task
- Phase-by-phase resource allocation chart across all 9 roles
- Risk assessment and mitigation planning
- Full financial budget with labor, hardware, software, and contingency breakdowns

### Phase 3 — Execution
- LiDAR drone missions (DJI Matrice 350 RTK + Zenmuse L2) via DJI Pilot 2
- Backend API and cloud pipeline development (Node.js, Python, AWS EC2/S3/RDS)
- Frontend dashboard development (React, CesiumJS, Three.js, Potree)
- Flutter mobile app build
- LiDAR processing pipeline integration (Pix4D, PDAL, GDAL)

### Phase 4 — Monitoring & Control
- CI/CD pipelines via GitHub Actions and Jenkins
- Unit, integration, and performance testing
- Field testing with drone pilots; security validation
- User Acceptance Testing (UAT) with site engineers
- Real-time tracking via Jira, CI/CD dashboards, and cloud logs

### Phase 5 — Closure
- Production rollout and field team training
- Final project review — successes, challenges, lessons learned
- Full documentation archive
- Post-deployment support and maintenance plan

---

## 📊 Work Breakdown Structure (WBS)

A detailed WBS was developed following PMI conventions, decomposing the project into manageable tasks by phase. Full WBS is in **Appendix A** of the project report. Top-level structure:

```
OFFSITE Platform
├── 1.0 Initiation
│   ├── 1.1 Stakeholder Identification
│   ├── 1.2 Feasibility Study
│   ├── 1.3 FAA/Regulatory Compliance
│   └── 1.4 Initial Site Mapping
├── 2.0 Planning
│   ├── 2.1 Requirements Gathering
│   ├── 2.2 Architecture Design
│   ├── 2.3 WBS Development
│   ├── 2.4 Risk Assessment
│   └── 2.5 Resource & Schedule Planning
├── 3.0 Execution
│   ├── 3.1 Drone Operations Setup
│   ├── 3.2 Backend Development
│   ├── 3.3 Frontend Dashboard
│   ├── 3.4 Mobile App (Flutter)
│   └── 3.5 LiDAR Processing Pipeline
├── 4.0 Monitoring
│   ├── 4.1 CI/CD Pipeline Setup
│   ├── 4.2 Testing (Unit / Integration / UAT)
│   ├── 4.3 Security Validation
│   └── 4.4 Performance Monitoring
└── 5.0 Closure
    ├── 5.1 Production Deployment
    ├── 5.2 Training & Handover
    ├── 5.3 Documentation Archive
    └── 5.4 Post-Deployment Support Plan
```

---

## 👥 Stakeholder Analysis

**Primary Stakeholders**
- **Project Manager** — Oversees planning, execution, and cross-team coordination
- **Construction Company Client** — Primary user; provides requirements and validates performance
- **Software Development Team** — Designs, builds, and maintains the platform
- **Site Engineers / Field Supervisors** — Operate drones and use the dashboard for progress validation
- **End Users (Clients & Subcontractors)** — View progress reports and communicate updates

**Secondary Stakeholders**
- **Data Analytics & GIS Specialists** — Process LiDAR data into 3D models and dashboards
- **Drone Vendors / Operators** — Supply hardware, ensure FAA regulatory compliance

**Tertiary Stakeholders**
- IT Security, Legal/Compliance, Cloud Infrastructure Vendors

---

## 🗂️ RACI Matrix

A full RACI Matrix (Appendix C of the report) maps every project activity to roles:

| Role | Initiation | Planning | Drone Ops | Development | Testing | Handover |
|---|---|---|---|---|---|---|
| Project Manager | A | A | I | A | A | A |
| Backend Developers | I | C | I | R | C | I |
| Frontend Developers | I | C | I | R | C | I |
| UI/UX Designer | I | C | I | R | I | I |
| Data Engineer | I | C | R | R | C | I |
| QA Team | I | I | I | C | R | I |
| DevOps | I | C | I | R | R | C |
| Security Architect | C | C | I | C | R | I |
| Scrum Master | C | R | I | C | C | I |

---

## 💰 Financial Plan

Total estimated project cost: **$3,940,393**

| Resource | Cost | Share |
|---|---|---|
| Labor | $2,974,400 | 75.5% |
| Contingency | $624,023 | 15.8% |
| Hardware | $251,698 | 6.4% |
| Software Tools | $90,272 | 2.3% |
| **Total** | **$3,940,393** | |

**Labor** covers the full multidisciplinary team: backend, frontend, DevOps, data engineering, security, drone operations, QA, and project management.

**Hardware** includes DJI Matrice 350 RTK drones, Zenmuse L2 LiDAR sensors, RTK equipment, and field computers.

**Software** covers AWS infrastructure, Pix4D licenses, GitHub Enterprise, Figma, Jira, and monitoring tooling.

**Contingency (15.8%)** buffers against regulatory approvals, hardware failure, scope changes, and unforeseen technical issues.

---

## ⚠️ Risk Management

Six risk categories were identified and tracked in a formal Risk Register (Section 6.0 of the report):

| Category | Key Risk | Priority | Mitigation |
|---|---|---|---|
| Regulatory | FAA drone compliance failure | High | Early permit applications; dedicated compliance track |
| Hardware | Drone malfunction mid-mission | High | Redundant hardware; pre-flight checklists; field spares |
| Security | Unauthorized data access | High | TLS + AES encryption; OAuth 2.0 + RBAC; full audit logging |
| Technical | Integration delays between modules | High | CI/CD pipelines; modular architecture; schedule buffers |
| Financial | Budget overrun | Medium | 15.8% contingency; weekly financial reviews |
| Workforce | Key personnel unavailability | Medium | Cross-training; documented handover procedures |

---

## 👷 Team & Resource Allocation

Resources were phased according to project intensity — heavy development during Execution, concentrated QA during Monitoring, and cross-functional collaboration throughout:

| Role | P1 | P2 | P3 | P4 | P5 |
|---|---|---|---|---|---|
| Project Manager | ●●● | ●●● | ●●● | ●●● | ●●● |
| Developers | ●●● | ●●●● | ●●●●● | ●●●● | ●●● |
| UI/UX Designer | ● | ●●●● | ●●●●● | ●● | ● |
| Data Engineer | ●● | ●●● | ●●● | ●● | ●● |
| QA Team | ● | ●● | ●●●●● | ●●● | ●● |
| DevOps | ● | ●● | ●●●●● | ●●● | ●● |
| Security Architect | ● | ●● | ●●● | ●●● | ●● |

*● Low involvement · ●●● Medium · ●●●●● Very High*

---

## 🔧 Platform Technical Summary

The drone-powered platform built and managed under this project:

- **Data Capture** — DJI Matrice 350 RTK + Zenmuse L2 LiDAR; ±2 cm accuracy; up to 1,200,000 pts/sec; 2.5 km² per flight
- **Cloud Pipeline** — AWS S3 ingestion → EC2 processing (Pix4D, PDAL, GDAL) → PostgreSQL/PostGIS
- **3D Dashboard** — React + CesiumJS / Three.js / Potree; real-time digital twin with cut/fill volume calculations
- **Mobile** — Flutter app for field access
- **Security** — TLS in transit, AES at rest, OAuth 2.0 + JWT, RBAC, full audit logging
- **CI/CD** — GitHub Actions + Docker + Jenkins

---

## 📚 Documentation Index

| Document | Location |
|---|---|
| Full Project Report (26 pages) | `ProjectManagement_ConstructionVisibilityDroneBased_Report.docx` |
| Presentation Deck | `ProjectManagement_ConstructionVisibilityDroneBased_Presentation.pptx` |
| Feasibility Template | `ProjectManagement_ConstructionFeasibility_Template.pdf` |
| WBS (full breakdown) | Report — Appendix A |
| Project Schedule | Report — Appendix B |
| RACI Matrix | Report — Appendix C |
| Resource Allocation Charts | Report — Appendix D |

---

## 🎓 Academic Context

This project was submitted as a final deliverable for **EMGT 5220: Engineering Project Management** at **Northeastern University, College of Engineering** (December 2025), under Prof. Sharad Bajracharya.

---

*Built by the OFFSITE team — Northeastern University, 2025*
