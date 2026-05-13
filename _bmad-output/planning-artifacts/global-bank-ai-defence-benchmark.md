# Global & Indian Banking AI Cyber Defence — Benchmark Analysis
**Classification:** Internal — Confidential  
**Prepared for:** CISO, CTO, Head of Cloud, DevSecOps Leads  
**Date:** 2026-05-05  
**Version:** 1.0 (Draft for Review)  
**Sources:** Internet-wide research across RBI, CERT-In, BIS, FSB, SEBI, IRDAI, HDFC Bank, SBI, JPMorgan, HSBC, SWIFT, Palo Alto, Microsoft, Gartner (all citations inline)

---

## 1. The Mythos Trigger Event — India's Emergency Response

### 1.1 The April 23, 2026 Emergency Meeting

This is not a hypothetical threat. On **April 23, 2026**, Finance Minister Nirmala Sitharaman convened an emergency high-level meeting with:
- Heads of all scheduled commercial banks
- IT Minister Ashwini Vaishnaw
- Reserve Bank of India
- NPCI
- CERT-In

**FM Sitharaman's exact statement**: *"Now, because of the new challenge which coming in the name of Mythos, about which not much is known... We need something new, something far more versatile to counter the newer threats."*

**What the Government knows about Mythos**:
- UK AI Security Institute testing: **73% performance on expert-level hacking tasks**
- Already identified **thousands of high-severity vulnerabilities** across major operating systems and browsers before institutions could patch them
- Core threat: **acceleration of exploitation timelines** — industrialised vulnerability discovery faster than any human patching cadence can match

**Specific Directives issued to Indian banks:**
1. Implement all necessary measures to secure IT systems and protect customer data immediately
2. Establish **real-time threat intelligence sharing** between banks, CERT-In, and relevant agencies
3. Report suspicious activity within 6 hours (existing mandatory rule, now enforced strictly)
4. Hire top cybersecurity professionals and specialised agencies for enhanced monitoring
5. IBA to develop a coordinated institutional response — **SBI Chairman Challa Srinivasulu Setty is leading this**
6. MeitY actively engaging with technology companies and global authorities

**Bain & Company advised**: Banks may need to **double their current cybersecurity spending** from typical 10% annual increases.

> **Source**: [Outlook Business](https://www.outlookbusiness.com/deeptech/sitharaman-flags-mythos-ai-cyber-threat-directs-banks-to-boost-defences) | [Business Standard](https://www.business-standard.com/technology/tech-news/indian-banks-govt-anthropic-threat-claude-mythos-ai-cybersecurity-risks-126042700436_1.html) | [JNR Management Analysis](https://www.jnrmanagement.com/india-raises-unprecedented-ai-alarm-fm-sitharaman-convenes-emergency-meeting-with-banks-and-rbi-over-anthropics-claude-mythos-cyber-risk.html)

---

## 2. Indian Banking Threat Landscape — Verified Numbers

| Metric | Statistic | Source |
|---|---|---|
| Cyber fraud cases H1 2025 vs H1 2024 | **+40% increase** | RBI |
| CERT-In incidents handled 2025 | **29.44 lakh (2.944 million)** | PIB |
| Average data breach cost in India 2024 | **USD 2.18 million** | Digital Threat Report 2024 |
| Phishing attacks rise in BFSI 2024 | **+175%** | Digital Threat Report 2024 |
| AI-powered phishing success rate | **>40%** | Digital Threat Report 2024 |
| Pakistan-allied attacks post-Operation Sindoor | **1.5 million attempts; 150 breaches** | Maharashtra Cyber / CERT-In |
| Deepfake fraud losses projected 2025 | **₹70,000 crore** | HyperVerge |
| Indian adults exposed to AI voice/deepfake scams | **47%** (vs 25% global average) | McAfee / HyperVerge |
| Voice cloning fraud rise | **+680% YoY** | HyperVerge |
| RBI penalties for cybersecurity violations FY24-25 | **₹54.78 crore** | RBI enforcement |

### 2.1 The C-Edge Attack — Closest Real-World Precedent

The **C-Edge Technologies ransomware attack (August 2024)** is the bank's most relevant real-world precedent and directly validates Vector 2 (Jenkins Pipeline Compromise) in the Mythos attack analysis:

- **Entry point**: Misconfigured Jenkins server exploiting **CVE-2024-23897**
- **Attacker**: RansomEXX v2.0
- **Impact**: 300+ small banks disrupted; ~1,500 cooperative and regional rural banks' customers locked out of ATMs, UPI payments, RTGS
- **Response**: NPCI was forced to temporarily isolate C-Edge from all retail payment systems
- **Timeline**: Detection July 29, 2024 → public disruption August 1, 2024 (3-day gap)

> **This is not a hypothetical. It happened. The entry vector — a misconfigured Jenkins server — is identical to Vector 2 in the Mythos bank analysis.**

> **Source**: [Juniper Networks](https://blogs.juniper.net/en-us/threat-research/cve-2024-23897-enabled-ransomware-attack-on-indian-banks) | [CloudSEK](https://www.cloudsek.com/blog/major-payment-disruption-ransomware-strikes-indian-banking-infrastructure) | [CSO Online](https://www.csoonline.com/article/3480250/over-300-indian-banks-suffer-payment-disruption-from-ransomware-attack.html)

### 2.2 Operation Sindoor — Active APT Threat

Following India's military Operation Sindoor (May 7, 2025), **seven APT groups** coordinated attacks specifically against Indian BFSI:
- APT 36 (Pakistan-based)
- Pakistan Cyber Force
- Team Insane PK
- Mysterious Bangladesh
- Indo Hacks Sec
- Cyber Group HOAX 1337
- National Cyber Crew

Attack types included: ransomware, supply chain intrusions, DDoS, website defacement, and malware — all targeting BFSI systems.

> **Source**: [RUSI](https://www.rusi.org/explore-our-research/publications/commentary/operation-sindoor-and-india-pakistans-escalated-rivalry-cyberspace) | [CYFIRMA](https://www.cyfirma.com/research/firewalls-and-frontlines-the-india-pakistan-cyber-battlefield-crisis/)

---

## 3. Indian Regulatory Landscape — Current Requirements

### 3.1 RBI Master Directions (In Force)

**IT Framework & Outsourcing (April 2024)**: Governs IT governance, cloud adoption, and third-party outsourcing for all scheduled commercial banks. Key requirement: exit strategies and security obligations for all IT service providers.

**Cyber Resilience Master Direction for PSOs (July 2024)**:
- Board-approved IS policy reviewed annually
- **Zero Trust principles** (identity-first, biometrics, adaptive MFA)
- **Least privilege access** for employees and vendors
- **Micro-segmentation** to limit breach spread
- **Continuous monitoring using AI-powered analytics** (explicitly required)
- Business continuity drills simulating large-scale attacks
- Third-party vendors must meet the same resilience standards
- Implementation: Large PSOs by **April 1, 2025**; Medium PSOs by **April 1, 2026**

**RBI FREE-AI Framework (August 13, 2025)** — Seven "Sutras": Trust, People First, Innovation, Fairness, Accountability, Explainability, Resilience. Six pillars: Infrastructure, Policy, Capacity, Governance, Protection, Assurance. Proposes an **AI Innovation Sandbox** for pilot testing AI-driven solutions. Currently guidance, not binding regulation — but signals the direction of future mandates.

**Status**: Only **20.8% of surveyed Indian financial entities** currently deploy AI in cybersecurity — this is the maturity gap the regulator is trying to close.

> **Source**: [KPMG on RBI Cyber Resilience](https://kpmg.com/in/en/insights/2024/10/securing-non-bank-psos-rbis-guidelines-on-cyber-resilience-and-digital-payment-security-controls.html) | [RBI FREE-AI (PDF)](https://rbidocs.rbi.org.in/rdocs/PublicationReport/Pdfs/FREEAIR130820250A24FF2D4578453F824C72ED9F5D5851.PDF) | [KPMG FREE-AI Analysis](https://kpmg.com/in/en/insights/2025/08/rbi-free-ai-committee-report-on-framework-for-responsible-and-ethical-enablement-of-artificial-intelligence.html)

### 3.2 SEBI CSCRF (August 2024)

Mandatory for Market Infrastructure Institutions and Qualified Regulated Entities:
- Based on ISO 27000, CIS Controls v8, NIST SP 800-53
- Mandatory **red teaming exercises** simulating real-world adversarial attempts
- **Post-quantum risk assessments** required
- SOC requirements specified
- Compliance: Existing SEBI-regulated entities by **January 1, 2025**; others by **April 1, 2025**

> **Source**: [SEBI CSCRF Circular](https://www.sebi.gov.in/legal/circulars/aug-2024/cybersecurity-and-cyber-resilience-framework-cscrf-for-sebi-regulated-entities-res-_85964.html)

### 3.3 The Localisation Constraint

**RBI Data Localisation**: All customer and payment data must be stored on servers located in India. If processed abroad, it must be deleted from foreign servers and returned to India within 24 hours.

**IFS Cloud (Indian Financial Technology and Allied Services)**: RBI's wholly-owned subsidiary providing sovereign cloud infrastructure — **restricted to Indian-registered companies, explicitly excluding foreign players**.

This is the structural reason Mythos (a public cloud-based AI platform) cannot currently be used inside the bank's perimeter. The regulatory path is:
1. Engage RBI for interim exemption (bounded scope, specific use case, committed localisation timeline)
2. Design a localisation architecture (India-region processing, data residency guarantees)
3. Use the FREE-AI sandbox as a formal testing environment

---

## 4. How Indian Banks Are Responding — Benchmarks

### 4.1 HDFC Bank — The Gold Standard Among Indian Banks

HDFC is the most advanced Indian bank publicly demonstrating AI-powered cybersecurity. Key metrics and approach from CISO Sameer Ratolikar:

**AI SOC deployment (Securonix)**:
- Deployed Securonix with **AI agents to reduce noise, accelerate investigations through natural-language search, and prepare response actions** — while keeping analysts in control
- Implemented **Model Context Protocol (MCP)** enabling contextual conversations between AI agents
- At RSAC 2025: *"automation is no longer optional, it's inevitable" — "humans will act like security bots, and bots will be treated like humans"*

**Fraud Detection AI**:
- Databricks Data Intelligence Platform on Azure — unified data lake for fraud detection
- AI/ML analyzing **100+ parameters in real-time per transaction**
- **20% reduction in credit card fraud losses**
- **35% decrease in false positives** (most relevant benchmark for the Checkmarx FP problem)
- Streaming analytics scoring every card swipe, UPI payment, and net-banking login in **under 200 milliseconds**

> **Source**: [BankInfoSecurity](https://www.bankinfosecurity.com/ai-bots-take-over-cybersecurity-at-hdfc-bank-a-28241) | [Klover: HDFC AI Strategy](https://www.klover.ai/hdfc-bank-ai-strategy-analysis-of-dominating-banking-ai/)

### 4.2 SBI — Scale Player, Leading Coordination

- Annual ICT spending: **$1.3 billion (2024)** — AI, big data, cloud, cybersecurity are the focus areas
- AI-based tools identifying branches prone to fraud and suspicious chargeback complaints
- **Leading the IBA coordinated response** to Mythos (SBI Chairman Setty)
- "Hack-AI-Thon 2025" innovation initiative

### 4.3 ICICI Bank

- Enterprise Fraud Risk Management (EFRM) system using ML to analyse customer behaviour patterns
- AI chatbot 'iPal': **40% reduction in customer complaints related to fraud**
- AI-powered KYC processing

### 4.4 Axis Bank

- Annual ICT spending: **$290.8 million (2024)**
- CISO publicly endorsing AI-driven security tools for detecting sophisticated scams

---

## 5. Global Banking Benchmarks

### 5.1 JPMorgan Chase — The Apex Benchmark

| Metric | Value |
|---|---|
| Annual technology budget 2025 | **$18 billion** |
| Employees with AI tools | **200,000+** |
| Deployed AI use cases | **450+** |
| Annual business value from AI | **$1.5 billion** |
| AI investment in 2024 | **~$1.3 billion** |

JPMorgan has published guidance specifically on **security considerations for agentic AI systems** — a directly relevant reference for the bank's AI gateway design. Their public position: "AI vs. AI: The arms race for security."

> **Source**: [JPMorgan Agentic AI Security](https://www.jpmorganchase.com/about/technology/blog/securing-agentic-ai) | [Klover: JPMorgan AI Strategy](https://www.klover.ai/jpmorgan-ai-strategy-chasing-ai-dominance/)

### 5.2 HSBC

- AI deployed across **600+ applications** including detection and cybersecurity
- Established an **AI Academy** for responsible AI upskilling
- AI-powered coding assistants scaled across software development

### 5.3 SWIFT — Industry-Level AI Fraud Defence

- January 2025: **AI-powered fraud defence for cross-border payments** launched
- Built on pseudonymized data from billions of transactions annually
- September 2025: Experiments with **13 global financial institutions** using privacy-enhancing technologies for secure cross-border fraud data sharing
- Context: Fraud cost the financial industry **USD 485 billion in 2023 alone**

> **Source**: [SWIFT AI Launch](https://www.swift.com/news-events/press-releases/swift-launch-ai-powered-fraud-defence-enhance-cross-border-payments) | [SWIFT AI Pilots](https://www.swift.com/news-events/press-releases/swift-and-global-banks-launch-ai-pilots-tackle-cross-border-payments-fraud)

---

## 6. Technology Approaches — Evidence-Based

### 6.1 AI-Powered SIEM / SOC Platforms

**Palo Alto Cortex XSIAM**:
- Fastest-growing product in Palo Alto history — surpassed **$1 billion in cumulative bookings in 2025**
- Integrates SIEM, XDR, SOAR, and ASM into a single console
- **10,000+ detectors and 2,600+ ML models** without hand-built queries
- One documented customer: alert volume dropped **87% in 3 months**; mean time to respond reduced from days to **under 10 minutes**
- 2025 declared "The Year of the Autonomous SOC" by Palo Alto

**Microsoft Sentinel**:
- **Leader in 2025 Gartner Magic Quadrant for SIEM**
- Security Copilot-powered Threat Hunting Agent — end-to-end investigations via natural language
- Integration with Palo Alto Cortex XDR

**HDFC Bank (confirmed)**: Deployed **Securonix** with agentic AI mesh for SOC operations.

**Gartner**: Named "AI SOC Agents" as a formal category in **June 2025**.

**RSAC 2026**: CrowdStrike, Cisco, and Palo Alto all shipped agentic SOC tools — this is the confirmed market direction.

> **Source**: [Palo Alto XSIAM 2025](https://www.paloaltonetworks.com/blog/security-operations/2025-the-year-of-the-autonomous-soc-the-year-of-xsiam/) | [Microsoft Sentinel Ignite 2025](https://techcommunity.microsoft.com/blog/microsoft-security-blog/microsoft-ignite-2025-power-the-next-era-of-cybersecurity-with-microsoft-sentine/4469080)

### 6.2 Zero Trust and Micro-Segmentation

The **SecureBank framework** (arXiv:2512.23124, December 2024) formalises financially-aware Zero Trust architecture with four components:
1. Financial Zero Trust
2. Adaptive Identity Scoring
3. Contextual Micro-Segmentation
4. Impact-Driven Security Automation

**RBI explicitly mandates** Zero Trust principles and micro-segmentation in its July 2024 Cyber Resilience Master Direction — this is no longer optional for regulated entities.

Global Zero Trust Security market: **USD 36.5 billion (2024) → USD 78.7 billion by 2029** (CAGR 16.6%).

Leading banking deployers: Goldman Sachs, Capital One, JPMorgan Chase.

**CISA** published "Zero Trust Microsegmentation" guidance in 2025 specifically for critical infrastructure.

> **Source**: [SecureBank Framework](https://arxiv.org/html/2512.23124) | [CISA Microsegmentation](https://www.cisa.gov/sites/default/files/2025-07/ZT-Microsegmentation-Guidance-Part-One_508c.pdf)

### 6.3 Post-Quantum Cryptography (PQC) and HSM

The G7 Cyber Expert Group (January 2026) set a **2030–2032 migration target** for critical financial system PQC adoption.

**HSM PQC Certification Status (2024–2026)**:
| Vendor | Certification | Date | Notes |
|---|---|---|---|
| Thales Luna | FIPS 140-3 Level 3 + PQC firmware | April 2024 / mid-2025 | Native ML-KEM and ML-DSA |
| Entrust nShield 5 | FIPS 140-3 Level 3 + PQC | August 2024 | Hardware-accelerated via FPGA |
| Utimaco Atalla AT1000 | FIPS 140-3 | June 2025 | First payment HSM FIPS 140-3 cert |
| Futurex | **PCI HSM + PQC** | June 2025 | **Only PQC-ready PCI HSM** — critical for payment institutions |

**NIST deprecation timeline**:
- RSA and ECC at 112-bit: deprecated after **2030**
- All quantum-vulnerable asymmetric cryptography: disallowed after **2035**

**White-Box Cryptography (WBC)**: Actively used in software environments (mobile banking, payment terminals) where HSMs are impractical. WhibOx 2024/CHES 2024 contest with 47 implementations confirms active research. Specific bank deployments are not publicly disclosed (security by design) but Secure-IC, Irdeto, and Cryptomathic are the leading vendors.

> **Source**: [PQShield RSA 2025](https://pqshield.com/trust-starts-in-the-hardware-inside-the-hsm-strategy-for-post-quantum-security-rsa-2025/) | [Mastercard PQC Whitepaper](https://www.mastercard.com/content/dam/mccom/shared/news-and-trends/stories/2025/quantum-explainer-and-white-paper/Migration-to-post-quantum-cryptography-WhitePaper_2025.pdf)

### 6.4 Container and Supply Chain Security

**Scale of the problem**:
- Software supply chain attacks: **+742% between 2019 and 2023**
- **37% of organisations** reported container/Kubernetes security incidents in 2024
- Sonatype found **512,847 malicious packages** in a single year (+156% YoY)

**LiteLLM Supply Chain Attack (2025)**: Directly relevant to the bank's planned gateway — TeamPCP compromised LiteLLM's CI/CD pipeline (97 million monthly downloads), triggering investigations at OpenAI, Anthropic, and Meta. This confirms that the AI gateway itself is a supply chain target.

**NSA and CISA joint advisory**: CI/CD pipeline compromises are increasing as a primary attack vector.

The C-Edge attack is the definitive evidence that **Jenkins CI/CD security is not optional** in Indian banking.

> **Source**: [CloudSEK: DevSecOps Supply Chain](https://www.cloudsek.com/blog/the-scanner-was-the-weapon-36-months-of-precision-supply-chain-attacks-against-devsecops-infrastructure) | [ExtraHop: AI Supply Chain](https://www.extrahop.com/blog/amid-rising-genaI-hacking-hysteria-supply-chain-most-at-risk)

### 6.5 Prompt Injection in Financial Services

**The $1.1 billion problem**:
- Prompt injection is **OWASP Gen AI Top 10 LLM01:2025** — the #1 AI vulnerability
- Financial services bore **$1.1 billion of $2.3 billion** in total 2025 prompt injection losses
- A hedge fund lost **$47 million** in March 2025 through AI chatbot manipulation
- Retail banks lost **~$230 million** to AI chatbot fraud in 2025
- Current detection catches only **23% of sophisticated prompt injection attempts**

> **Source**: [Obsidian Security](https://www.obsidiansecurity.com/blog/prompt-injection)

---

## 7. International Regulatory Benchmarks

### 7.1 US Treasury FS AI RMF (February 2026)

The most comprehensive available framework for AI risk in financial services — **230 specific control objectives** across:
- Governance
- Data management
- Model development and validation
- Monitoring
- Third-party risk
- Consumer protection

**Critical gap**: US OCC SR 26-02 (April 2026) that replaced the 15-year SR 11-7 model risk framework **explicitly excludes GenAI and agentic AI** from scope. The FS AI RMF fills this gap.

**Recommendation**: Indian banks should self-impose the US Treasury FS AI RMF 230 control objectives as the most comprehensive available framework while RBI/SEBI develop binding regulation.

> **Source**: [Treasury FS AI RMF](https://home.treasury.gov/news/press-releases/sb0401) | [NIST AI RMF](https://www.nist.gov/itl/ai-risk-management-framework)

### 7.2 EBA / EU AI Act (November 2025)

EBA factsheet confirmed **no significant contradictions** between the EU AI Act and existing EU banking legislation — the AI Act is complementary. 2026–2027: EBA will promote common supervisory approach for AI Act implementation.

### 7.3 SEBI CSCRF vs RBI FREE-AI — The Gap

SEBI's CSCRF (binding, in force) mandates red teaming and post-quantum assessments. RBI's FREE-AI framework (August 2025) is guidance-only. For banks that are both RBI-regulated and SEBI-regulated, SEBI's harder requirements apply — and most large banks are both.

### 7.4 The TIBER Gap — India Has No Equivalent

EU banks operate under **TIBER-EU**: a threat intelligence-based red-teaming framework that enables Mythos-class offensive testing in a formally sanctioned regulatory environment. The UK has **CBEST**. The US has **iCAST**. **India has no equivalent.**

This is a material gap. Without a TIBER-IN framework, the bank cannot formally use Mythos for authorised red-teaming without regulatory ambiguity. Lobbying IBA/RBI to establish TIBER-IN would unblock this.

---

## 8. BIS / FSB Global Intelligence

### 8.1 BIS Papers No. 145 (May 2024)

Survey of central banks' GenAI posture:
- **71%** already using GenAI
- **26%** plan to adopt within 1–2 years
- Only **19%** have a concrete strategy for GenAI adoption — **23% have no strategy at all**
- GenAI assessed as offering **more benefits than risks** in cyber threat detection
- Primary challenge: **human capital** — people with both cybersecurity and AI expertise

### 8.2 FSB "Financial Stability Implications of AI" (November 2024)

Four primary AI-related vulnerabilities identified:
1. **Third-party dependency and AI provider concentration** — multiple institutions using identical AI providers creates systemic risk
2. **Market correlations** — AI-driven strategies potentially creating synchronised movements
3. **Cyber risks** — expanded attack surface from AI system integration
4. **Model risk, data quality and governance**

**FSB October 2025 Follow-Up**: Called for financial authorities to enhance monitoring, assess regulatory adequacy, and use AI-powered tools in their own supervisory work.

> **Source**: [FSB Nov 2024](https://www.fsb.org/2024/11/the-financial-stability-implications-of-artificial-intelligence/) | [BIS Papers 145](https://www.bis.org/publ/bppdf/bispap145.pdf)

---

## 9. Benchmark Gap Analysis — This Bank vs. Peers

| Dimension | HDFC Bank (best Indian) | JPMorgan (global best) | This Bank (estimated) | Gap |
|---|---|---|---|---|
| AI SOC deployment | Securonix agentic AI live | 450+ AI use cases, LLM Suite for 200K staff | Phase 1 planned | 12-24 months behind HDFC |
| Cross-cloud SIEM | Likely advanced (not public) | Unified; cross-cloud assumed | Not deployed | Critical gap |
| Prompt injection defence | Not publicly disclosed | Agentic AI security guidance published | Heuristic guard planned | Needs structural hardening |
| Container security | Not publicly disclosed | Assumed enterprise-grade | Prisma only; lineage Phase 3 | Medium gap |
| PQC readiness | Not publicly disclosed | Actively investing | Not mentioned | 2026-2030 window to act |
| Zero Trust / micro-segmentation | Likely partially deployed | Gold standard | Partially deployed | Moderate gap |
| Threat intelligence sharing | IBA coordinated response | FS-ISAC active member | Engagement via IBA | Needs formalisation |
| Red team programme | Not public | AI-assisted red team assumed | Quarterly adversarial exercise planned | On roadmap |

---

## 10. Priority Recommendations (Evidence-Based)

### Immediate (Board-Level)

1. **Double cybersecurity budget** — Bain & Company's direct advice to Indian banks post-Mythos announcement. Current 10% annual increase is insufficient against AI-speed threats.

2. **Engage IBA to establish TIBER-IN** — Without a formally sanctioned AI red-teaming framework, Mythos-class testing exists in regulatory grey territory. Push for India's equivalent of EU TIBER-EU.

3. **Adopt US Treasury FS AI RMF 230 control objectives** as the bank's AI governance standard while RBI develops binding AI regulation — proactive compliance positions the bank ahead of the regulatory curve.

### Technical (CISO-Level)

4. **Deploy Palo Alto XSIAM or Microsoft Sentinel** as the unified AI-powered SIEM — this solves the cross-cloud correlation gap (Vector 5) and the alert fatigue problem (Vector 1 enabler) in a single deployment.

5. **Jenkins hardening is non-negotiable** — The C-Edge attack (CVE-2024-23897, Jenkins misconfiguration, 300 banks disrupted) is the exact threat model. Jenkins plugin CVE gating, audit logging to SIEM, and plugin whitelist are minimum baselines.

6. **Implement OPA/Kyverno admission control now** — HDFC, JPMorgan, and Goldman all have Kubernetes policy enforcement. The bank's acknowledged manifest deviations from CIS hardening are a live attack surface.

7. **Treat prompt injection as a Tier-1 security control** — $1.1 billion in financial services losses in 2025 alone. OWASP LLM01:2025. Apply structural USER/SYSTEM separation; implement Lakera Guard or equivalent prompt firewall at the LiteLLM gateway.

8. **Start PQC inventory now** — The 2030 NIST deprecation deadline sounds distant; the cryptography audit, procurement planning, and architecture changes needed to hit that deadline require starting today. Require FIPS 140-3 + PQC firmware support for all new HSM procurements from 2026.

### Regulatory (CISO + Legal)

9. **Engage RBI for interim Mythos/AI offensive tool exemption** — Frame as a cyber resilience requirement, not a productivity ask. Reference the FM's own emergency meeting. Propose: bounded scope, India-region data processing, committed localisation architecture with a 24-month delivery timeline.

10. **Establish formal threat intelligence sharing via IBA** — FS-ISAC is the global model. The IBA-led coordination post-Mythos is the seed. It needs a technical execution layer: a shared STIX/TAXII threat intelligence platform where Indian banks share IOCs, attack patterns, and incident data in near-real-time.

---

## 11. Source Index

| Source | URL | Relevance |
|---|---|---|
| FM Sitharaman Mythos Emergency Meeting | https://www.outlookbusiness.com/deeptech/sitharaman-flags-mythos-ai-cyber-threat-directs-banks-to-boost-defences | Direct government response |
| Business Standard: Claude Mythos Threat | https://www.business-standard.com/technology/tech-news/indian-banks-govt-anthropic-threat-claude-mythos-ai-cybersecurity-risks-126042700436_1.html | Policy response details |
| Digital Threat Report 2024 (CERT-In/MeitY/SISA) | https://www.cert-in.org.in/PDF/Digital_Threat_Report_2024.pdf | India BFSI threat statistics |
| PIB: CERT-In 2025 Capabilities | https://www.pib.gov.in/PressReleasePage.aspx?PRID=2217537 | Incident volumes |
| RBI FREE-AI Framework (PDF) | https://rbidocs.rbi.org.in/rdocs/PublicationReport/Pdfs/FREEAIR130820250A24FF2D4578453F824C72ED9F5D5851.PDF | AI governance guidance |
| KPMG: RBI Cyber Resilience Master Direction | https://kpmg.com/in/en/insights/2024/10/securing-non-bank-psos-rbis-guidelines-on-cyber-resilience-and-digital-payment-security-controls.html | Regulatory requirements |
| SEBI CSCRF Circular Aug 2024 | https://www.sebi.gov.in/legal/circulars/aug-2024/cybersecurity-and-cyber-resilience-framework-cscrf-for-sebi-regulated-entities-res-_85964.html | Mandatory red team requirements |
| HDFC Bank AI SOC (BankInfoSecurity) | https://www.bankinfosecurity.com/ai-bots-take-over-cybersecurity-at-hdfc-bank-a-28241 | Indian banking gold standard |
| C-Edge Jenkins Attack (Juniper) | https://blogs.juniper.net/en-us/threat-research/cve-2024-23897-enabled-ransomware-attack-on-indian-banks | Real attack precedent |
| CSO Online: 300 Banks Disrupted | https://www.csoonline.com/article/3480250/over-300-indian-banks-suffer-payment-disruption-from-ransomware-attack.html | Attack impact |
| FSB: Financial Stability Implications of AI | https://www.fsb.org/2024/11/the-financial-stability-implications-of-artificial-intelligence/ | Global systemic risk |
| BIS Papers 145: GenAI and Cybersecurity | https://www.bis.org/publ/bppdf/bispap145.pdf | Central bank AI posture |
| SWIFT AI Fraud Defence | https://www.swift.com/news-events/press-releases/swift-launch-ai-powered-fraud-defence-enhance-cross-border-payments | Industry AI deployment |
| JPMorgan Agentic AI Security | https://www.jpmorganchase.com/about/technology/blog/securing-agentic-ai | Agentic AI security guidance |
| Palo Alto: Year of Autonomous SOC | https://www.paloaltonetworks.com/blog/security-operations/2025-the-year-of-the-autonomous-soc-the-year-of-xsiam/ | AI SOC market data |
| US Treasury FS AI RMF | https://home.treasury.gov/news/press-releases/sb0401 | 230 AI control objectives |
| CISA Zero Trust Microsegmentation | https://www.cisa.gov/sites/default/files/2025-07/ZT-Microsegmentation-Guidance-Part-One_508c.pdf | Critical infrastructure guidance |
| RUSI: Operation Sindoor Cyber | https://www.rusi.org/explore-our-research/publications/commentary/operation-sindoor-and-india-pakistans-escalated-rivalry-cyberspace | Active APT threat context |
| HyperVerge: Deepfake Banking Fraud | https://hyperverge.co/blog/deepfake-banking-fraud/ | ₹70,000 crore deepfake projection |
| CloudSEK: DevSecOps Supply Chain Attack | https://www.cloudsek.com/blog/the-scanner-was-the-weapon-36-months-of-precision-supply-chain-attacks-against-devsecops-infrastructure | CI/CD attack patterns |
| PQShield: HSM PQC Strategy | https://pqshield.com/trust-starts-in-the-hardware-inside-the-hsm-strategy-for-post-quantum-security-rsa-2025/ | PQC HSM landscape |
| SecureBank Zero Trust Framework | https://arxiv.org/html/2512.23124 | Banking ZT architecture |
| EBA: AI Act Implications for Banking | https://www.eba.europa.eu/sites/default/files/2025-11/d8b999ce-a1d9-4964-9606-971bbc2aaf89/AI%20Act%20implications%20for%20the%20EU%20banking%20sector.pdf | EU regulatory position |
| Obsidian Security: Prompt Injection | https://www.obsidiansecurity.com/blog/prompt-injection | $1.1B financial losses data |
| Mastercard PQC Whitepaper | https://www.mastercard.com/content/dam/mccom/shared/news-and-trends/stories/2025/quantum-explainer-and-white-paper/Migration-to-post-quantum-cryptography-WhitePaper_2025.pdf | PQC migration timeline |

---

*Document prepared by: Mythos Project — AI Architecture & Business Analysis*  
*Companion to: mythos-bank-attack-analysis.md*  
*Classification: Internal — Confidential*
