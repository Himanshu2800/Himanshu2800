<div align="center">

# HIMANSHU JHA

### Cybersecurity Engineer · Detection Engineering · Cloud Security

**Building systems that detect, investigate & explain threats.**

<br>

[![GitHub](https://img.shields.io/badge/GitHub-Himanshu2800-181717?style=for-the-badge&logo=github)](https://github.com/Himanshu2800)
[![Email](https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jhahimanshu168@gmail.com)

</div>

---

<div align="center">

## `DETECT • INVESTIGATE • AUTOMATE`

</div>

I build security tooling around **cloud security, detection engineering, SIEM architecture and SOC automation** — with a focus on turning raw telemetry into actionable security intelligence.

---

## ☁️ Currently Building

### GCP Cloud SIEM

A cloud-native SIEM and threat-detection pipeline built around the complete detection lifecycle.

```text
 GCP TELEMETRY
      │
      ├── Cloud Audit Logs
      │
      └── VPC Flow Logs
              │
              ▼
       ┌──────────────┐
       │Cloud Logging │
       └──────┬───────┘
              ▼
       ┌──────────────┐
       │    Pub/Sub   │
       └──────┬───────┘
              ▼
       ┌──────────────┐
       │   Cloud Run  │
       │              │
       │ Detection    │
       │   Engine     │
       └──────┬───────┘
              │
       ┌──────┼───────────┐
       ▼      ▼           ▼
     Sigma  Enrichment  Correlation
       │      │           │
       └──────┼───────────┘
              ▼
       ┌──────────────┐
       │  OpenSearch  │
       └──────┬───────┘
              │
         ┌────┴────┐
         ▼         ▼
      Grafana    Slack
