# Awesome-Data-Security-Posture-Management-DSPM

# Awesome-Data-Security-Posture-Management-DSPM

**Top Data Security Posture Management DSPM (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Sensitive Data Discovery, Access Intelligence, Data Store Risk Scoring & Self-Hosted DSPM Scanners*

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Data Security Posture Management (DSPM)**. These tools enable organizations to discover where sensitive data lives, who can access it, how it flows, and where the risk concentrates—from fully managed enterprise platforms with agentless multi-cloud scanning to open-source scanners that give teams control over their discovery pipeline.



**Examples** include Cyera, Normalyze, Sentra, BigID, Securiti, Varonis, Symmetry Systems, Prisma Cloud DSPM (Dig Security), and CrowdStrike Falcon Data Security for SaaS (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted sensitive data discovery, cloud scanning, and open DSPM infrastructure. **Critical note**: The open-source DSPM landscape is nascent—**Poirot DSPM** is the most actively developed purpose-built open-source scanner with TheHive integration and multi-source support , while **Mantissa Stance** offers agentless multi-cloud discovery but with limited public validation . No open-source project matches Cyera's data volume tiering or BigID's 1,000+ classifiers out of the box.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global Data Security Posture Management (DSPM) market is estimated at **$1.1B–$2.2B in 2025** and projected to reach **$4.0B–$7.2B by 2030**, growing at a **CAGR of ~20%–25%**. The sector is currently **moderately fragmented**—pioneered by specialized pure-play innovators (such as Cyera, BigID, and Sentra) but undergoing rapid consolidation as cybersecurity and CNAPP heavyweights (Palo Alto Networks, CrowdStrike, Proofpoint, Veeam, Zscaler) acquire startups or embed native DSPM capabilities into unified cloud security suites.

## SaaS/Hosted Platforms

| Company & Platform | Company Size (Valuation / Revenue) | Starting Tier Pricing | Free Tier / Trial Limit | Key Focus & Deployment |
| :--- | :--- | :--- | :--- | :--- |
| **[Palo Alto Networks (Prisma Cloud DSPM)](https://www.paloaltonetworks.com/prisma/cloud)** | **~$105B+ Market Cap** ($9.2B FY25 Revenue) | **$18,000/year baseline commitment** (Credit model: 1 credit/IaaS-PaaS asset, 1 credit/TB DBaaS, 0.1 credit/SaaS user) | **30-day guided free trial** (scoped to evaluation cloud accounts & data volumes; contact sales) | Full CNAPP + DSPM multi-cloud data discovery & risk posture |
| **[CrowdStrike (Falcon Data Security)](https://www.crowdstrike.com/)** | **~$80B–$100B+ Market Cap** ($3.95B FY25 Revenue) | **$59.99/device/year** (Falcon Go entry tier; enterprise SaaS DSPM contracts typically start at **$20,000–$50,000/year**) | **15-day free trial** (Falcon platform modules, up to 100 endpoints) | SaaS ecosystem data security integrated into Falcon XDR platform |
| **[Cyera](https://cyera.io/)** | **$12B Valuation** (Series G 2026; $100M+ ARR) | **$50,000/year** (AWS Marketplace Standard tier up to 25 TB; Business: $100k/100 TB; Enterprise: $250k/250 TB) | **No perpetual free plan; Proof-of-concept (POC)** & Free Data Risk Assessment (1–2 weeks scoped assessment) | AI-native DSPM with agentless multi-cloud discovery & classification |
| **[Varonis](https://www.varonis.com/)** | **~$4.5B–$5.5B Market Cap** ($623.5M FY25 Revenue) | **$50–$95/user/year** (list benchmark for core DSP SaaS; custom volume tiers with enterprise minimums) | **30-day free trial** / Data Risk Assessment (limited to evaluation tenant & data footprint) | Data-centric security, automated remediation, and insider risk |
| **[Securiti (Securiti.ai)](https://securiti.ai/)** | **$1.725B Valuation** (Acquired by Veeam in Oct 2025) | **$50,000/year platform fee** (Modular subscription based on data sources and connected environments) | **No perpetual free plan; Guided trial / interactive demo** (scoped evaluation by request) | AI-driven Data Command Center bundling DSPM, privacy, and compliance |
| **[BigID](https://bigid.com/)** | **$1.25B Valuation** (~$100M ARR) | **$175,000/year** (AWS Marketplace Discovery Foundation tier; quoted per data sources & volume) | **No perpetual free plan; Scoped Data Risk Assessment** (limited-scope POC by request) | Broad data intelligence across DSPM, DLP, privacy, and AI governance |
| **[Normalyze](https://normalyze.ai/)** | **~$100M–$250M Valuation** (Acquired by Proofpoint in Oct 2024) | **$0 (Free Tier) / Enterprise custom quote** (Scales by cloud accounts, storage accounts, and data volume) | **Free Forever Tier**: 1 connected cloud account (AWS, Azure, GCP, or Snowflake) with up to 30-day history | Agentless DSPM with continuous sensitive data asset & access graph mapping |
| **[Sentra](https://sentra.io/)** | **~$200M+ Valuation** ($103M total funding) | **$50,000/year** (AWS Marketplace Standard tier; Essential: $100k; Advanced: $250k; Enterprise: $500k) | **No perpetual free plan; Tailored enterprise POC** (scoped evaluation by request) | Cloud-native DSPM priced by volume of data at-rest across IaaS/PaaS/SaaS |
| **[Symmetry Systems DataGuard](https://www.symmetry-systems.com/)** | **~$50M+ Valuation** (Acquired by Zscaler in May 2026; $20M+ funding) | **$5,000/month ($60,000/year)** (AWS Marketplace DataGuard Express tier up to 25 TB; Essentials up to 100 TB) | **No perpetual free plan; Scoped assessment** (live data risk assessment session by request) | Hybrid & on-premise/in-VPC DSPM with fine-grained access governance |

## Open-Source GitHub Projects



- **[Poirot DSPM](https://github.com/safernandez666/poirot-public)**

  **Open-source Data Security Posture Management scanner** (license per repo) — **the most actively developed purpose-built open-source DSPM** found in this research . **Features**: **Multi-source scanning**—MySQL, S3, Apache Kafka, Google Drive, OneDrive; detects credit cards, credentials, and PII; **severity classification** (CRITICAL/HIGH/MEDIUM/LOW) with deduplication; **TheHive 5 integration**—automatically creates cases and syncs findings; **multi-channel notifications** (Slack, Email, Teams, Webhooks); **scheduled scans**; **Cyberpunk dashboard** with real-time KPIs; **professional reports** (PDF/Excel/JSON) with AI-powered analysis via Ollama . **Tech stack**: Python, Docker Compose. **Deploy**: `git clone` and `docker compose up -d`; dashboard at localhost:8080 . **Trade-off**: **Early-stage project**—no enterprise support or SLAs; source connectors limited to specific data stores; no agentless cloud scanning like commercial DSPM . **Best for**: security teams wanting a self-hosted DSPM scanner with TheHive case management and multi-source discovery—especially those already using TheHive for incident response.



- **[Mantissa Stance](https://www.producthunt.com/products/mantissa-stance)**

  **Open-source CSPM, DSPM, CIEM, and vulnerability management** (license per Product Hunt listing) — **the most comprehensive open-source cloud security platform with DSPM capabilities** . **Features**: **Agentless** cloud security visibility across **AWS, GCP, and Azure**; combines **CSPM** (misconfiguration detection), **DSPM** (sensitive data discovery), **CIEM** (identity and entitlement management), and **vulnerability management** in a single tool . **Tech stack**: Per repository. **Deploy**: Self-hosted. **Trade-off**: **Limited public validation**—Product Hunt listing is the primary source; no GitHub repository or documentation surfaced in search results. **Best for**: teams wanting an all-in-one open-source cloud security tool with DSPM included—**verify maturity and activity before production adoption**.



### Additional Strong Open-Source Options



- **Lacework Terraform AWS DSPM Module** — Infrastructure-as-code module for deploying DSPM scanning in AWS (Terraform). Creates ECS Fargate scanner tasks, S3 bucket for results, EventBridge scheduling, and IAM roles for Lacework/FortiCNAPP integration . **Note**: **Deployment module, not a DSPM platform**—it deploys a commercial scanner (Lacework/FortiCNAPP). **Best for**: existing Lacework/FortiCNAPP customers wanting Terraform-managed DSPM deployment.

- **enterprise-siem-platform DSPM module** — Open-source SIEM platform with a DSPM module (GitHub commit). Pattern-based detection (SSNs, credit cards), context analysis, risk assessment, compliance mapping (PCI-DSS, GDPR, HIPAA), scheduled scanning . **Note**: **Component within a larger SIEM project**, not a standalone DSPM product; commit-based documentation only. **Best for**: developers building custom SIEM with DSPM capabilities.



**Frameworks for building custom systems**: **Poirot DSPM** is the most functional open-source starting point, combining multi-source scanning with TheHive integration. **Mantissa Stance** aims for broader cloud-native DSPM but needs validation. **No open-source project matches Cyera's data volume tiering or BigID's classifier library.**



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- DSPM platforms handling sensitive data must comply with data protection regulations (GDPR, CCPA, HIPAA, etc.) and implement appropriate access controls for discovered data and findings.

- **The "agentless cloud DSPM" vs. "source-connector scanner" vs. "deployment module" distinction is critical.** **Cyera, Normalyze, Sentra, BigID, Securiti, Varonis, Symmetry, Prisma Cloud DSPM, and CrowdStrike** are **commercial DSPM platforms**—they provide agentless discovery across cloud data stores with classification and access analysis . **Poirot DSPM** is a **source-connector scanner**—it connects to specific data sources (MySQL, S3, Kafka) and scans them; no agentless cloud discovery . **Mantissa Stance** aims for **agentless cloud DSPM** but has limited public validation . **Lacework Terraform module** is a **deployment tool** for a commercial scanner. **Choose based on whether you need agentless cloud coverage, specific source scanning, or deployment automation.**

- **Cyera's pricing is volume-tiered and six-figure minimum.** AWS Marketplace Standard is **$50,000/year for 25 TB**; Business is **$100,000/year for 100 TB**; Enterprise is **$250,000/year for 250 TB** . **Direct pricing is custom quoted and can exceed marketplace rates** . **Do not evaluate without enterprise budget approval.**

- **Prisma Cloud DSPM credit metering is asset-type-dependent.** IaaS/PaaS assets cost **1 credit each**; DBaaS assets cost **1 credit per TB**; SaaS assets cost **0.1 credit per user** . **Model your asset mix before comparing costs—a database-heavy environment pays differently than a SaaS-heavy one.**

- **Sentra's pricing is data-volume-based, not user-based.** It charges for **data at-rest** across all environments, not seats or infrastructure . **For organizations with large data stores but small teams, this can be advantageous; for data-light organizations, it may be less so.**

- **BigID's licensing is complex**—quoted per data sources, volume, environment count, and licensed pillars. **Do not expect a simple per-TB or per-user rate.** The **1,000+ pre-trained classifiers across 100+ languages** are a genuine differentiator .

- **Poirot DSPM is the most functional open-source DSPM** with TheHive integration and multi-source scanning, but it is **early-stage with no enterprise support** . **For security teams wanting a self-hosted scanner with case management, it is the starting point.**

- **Mantissa Stance lacks public validation.** The Product Hunt listing claims agentless multi-cloud DSPM, but no GitHub repository or documentation surfaced . **Verify maturity before production adoption.**

- **Pricing opacity is universal** across Normalyze, Sentra, BigID, Securiti, Varonis, Symmetry, Prisma Cloud DSPM, and CrowdStrike. All require sales contact or quote requests. **Cyera publishes marketplace tiers.** **Validate with direct vendor conversations against your data volume and cloud footprint.**

- Self-hosted open-source solutions require proper infrastructure (Docker for Poirot, Python for enterprise-siem DSPM module), security hardening, and ongoing maintenance. **DSPM tools scan sensitive data stores**—ensure your deployment meets your organization's privacy and compliance requirements before connecting production data sources.



---



**Made for data security engineers, cloud security teams, and organizations building transparent DSPM solutions.**

Let's make Data Security Posture Management more open, data-driven, and discovery-aware.
