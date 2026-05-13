# Board Executive Summary Deck — AI Cyber Defence Programme
## "Defending Against Mythos: India's AI Threat and Our Response"

**Classification:** Board Confidential  
**Audience:** Board of Directors, Risk Committee, Audit Committee  
**Presenter:** CISO + CTO  
**Duration:** 20 minutes presentation + 10 minutes Q&A  
**Date:** May 2026

> **Deck Design Notes:** Each slide has a headline that is itself the message (not a topic). Use the "so what" framing throughout. Every number on every slide must be citable. Max 5 bullets per slide. No jargon without a one-line definition. All risk ratings expressed in financial impact terms, not colour codes alone.

---

## SLIDE 1 — TITLE SLIDE

**Headline:** Defending the Bank Against India's Most Serious AI Cyber Threat

**Subtext:**
- A government-declared emergency. A proven attack on 300 Indian banks. A 12-month programme to close the gaps.
- Presented by: CISO + CTO
- Reviewed by: Risk Committee | Audit Committee

**Visual:** Single powerful image — India's financial network topology. No bullet points.

---

## SLIDE 2 — THE SITUATION IN THREE FACTS

**Headline:** Three Facts That Define Why This Is a Board Matter Today

**Content:**
1. **April 23, 2026**: Finance Minister Sitharaman called an emergency meeting with all bank heads, RBI, NPCI, and CERT-In — specifically naming Mythos as the threat requiring "something new, something far more versatile."
2. **August 2024**: A single misconfigured Jenkins server (C-Edge Technologies) disrupted 300+ Indian banks, took down ATMs and UPI for 1,500 cooperative banks, and forced NPCI to isolate an entire payment segment. The entry vector is **identical** to vectors in our current infrastructure.
3. **2025 data**: Cyber fraud in Indian banking increased **40%** in the first half of 2025 alone. Prompt injection attacks cost the global financial sector **$1.1 billion**. India is projected to lose **₹70,000 crore** to AI-powered deepfake fraud this year.

**Speaker Note:** The board must understand this is not a future risk. The C-Edge attack already happened to an institution with our stack. The government has already declared an emergency. We are responding to a known, active, government-validated threat.

---

## SLIDE 3 — WHAT IS MYTHOS

**Headline:** Mythos Is Not a Conventional Cyberattack — It Is an AI That Hacks at Machine Speed

**Content:**
| Traditional Attack | Mythos-Class AI Attack |
|---|---|
| Human hacker takes days to find vulnerabilities | Mythos identifies thousands of vulnerabilities before institutions can patch them |
| Attacks one system at a time | Simultaneously targets CI/CD, containers, cloud, and human operators |
| Detected by pattern-matching | Designed to evade SAST tools; exploits the >40% false-positive rate that drowns triage |
| Alert: CERT-In, patch, recover | Alert-to-exploit gap may be hours, not weeks |

**Key Statistic:** UK AI Security Institute testing: Mythos achieves **73% performance on expert-level hacking tasks** — outperforming most human penetration testers in specific domains.

**Bottom Line:** This is an AI fighting our human-speed security team. We need AI on our side.

**Visual:** Side-by-side comparison graphic — human attacker timeline vs. Mythos timeline on the same kill chain.

---

## SLIDE 4 — OUR CURRENT EXPOSURE

**Headline:** Our Infrastructure Has Five Structural Gaps That Mythos Will Exploit First

**Content (each with a one-line plain-English explanation):**

1. **No cross-cloud security monitoring** — We operate on both GCP and AWS. An attack that starts in one cloud and moves to the other is currently invisible to us. This is how sophisticated attackers avoid detection.

2. **CI/CD pipeline is an unguarded entry point** — Jenkins, our build system, is how all software reaches production. The C-Edge attack entered through exactly this channel. Our Jenkins has no AI-powered anomaly detection.

3. **Security alert triage is overwhelmed** — More than 40% of our security scanner alerts are false alarms. Attackers exploit this: hide real attacks inside manufactured noise. Our teams are triaging by hand.

4. **Kubernetes workloads not fully hardened** — Our container platform has acknowledged deviations from the security baseline. These misconfigurations are a documented escalation path for attackers who gain initial access.

5. **AI defence is 3–6 months from deployment** — We have a plan (the AI in DevSecOps POV). The plan is sound. But the threat is here now. We need to accelerate.

**Risk Rating Table:**

| Gap | If Exploited | Financial Exposure |
|---|---|---|
| Cross-cloud monitoring gap | Undetected lateral movement | Comparable to C-Edge: payment system disruption, ₹X crore operational loss + regulatory penalty |
| Jenkins pipeline compromise | Supply chain backdoor in production | Production data exfiltration; regulatory action; reputational loss |
| Alert fatigue | Malicious code ships undetected | Application-layer fraud; SAST bypass resulting in vulnerable production deployment |
| Kubernetes misconfiguration | Container escape → cluster takeover | Full workload compromise; potential data breach across all GKE/EKS namespaces |

**Speaker Note:** We are not presenting a hypothetical risk model. Each of these gaps has a real-world precedent from Indian banking in the last 18 months.

---

## SLIDE 5 — WHAT PEERS ARE DOING

**Headline:** The Gap Between Us and the Best Indian Bank Is 12–24 Months — Here Is How We Close It

**Content:**

| Capability | HDFC Bank (Indian Leader) | JPMorgan (Global Leader) | Our Bank Today | Our Target (12 months) |
|---|---|---|---|---|
| AI-powered SOC | Securonix agentic AI live; 35% false positive reduction | 450+ AI use cases; $18B tech budget | Phase 1 planned | AI SIEM live; cross-cloud coverage |
| Supply chain security | Advanced (not public) | Enterprise-grade | Prisma scanning only | Full lineage tracking + admission control |
| Cross-cloud SIEM | Likely advanced | Unified, cross-cloud | Not deployed | Live by Month 3 |
| Threat intelligence sharing | IBA coordination | FS-ISAC active member | IBA engagement | IBA threat intel platform |
| Post-quantum readiness | Not disclosed | Actively investing | Not started | Crypto inventory complete; PQC roadmap approved |

**Key Benchmark:** Bain & Company, advising Indian banks post-Mythos: banks may need to **double their current cybersecurity spending** from typical 10% annual increases.

**Visual:** Maturity radar chart — Our Bank vs. HDFC vs. JPMorgan across 6 dimensions.

---

## SLIDE 6 — THE REGULATORY IMPERATIVE

**Headline:** Three Regulators Now Require What We Are Proposing — Non-Compliance Carries Financial and Operational Penalties

**Content:**

| Regulator | Requirement | Our Current Status | Deadline |
|---|---|---|---|
| **RBI** — Cyber Resilience Master Direction (July 2024) | Zero Trust, micro-segmentation, AI-powered continuous monitoring, business continuity drills | Partially compliant | Large PSOs: April 2025 (past) |
| **SEBI** — CSCRF (August 2024) | Red teaming exercises, post-quantum risk assessment, SOC requirements | Assessment pending | January 2025 (past) |
| **CERT-In** | 6-hour mandatory incident reporting; BFSI-specific threat intelligence sharing | Compliant on reporting; sharing informal | In force |
| **RBI FREE-AI** (August 2025) | AI governance, AI Innovation Sandbox participation, responsible AI deployment | Framework adopted; governance in progress | Guidance (enforcement signals 2026) |

**Penalty Signal:** RBI imposed **₹54.78 crore** in cybersecurity-related penalties on Indian banks in FY2024-25.

**Bottom Line:** The programme we are proposing is not just risk management — it is regulatory compliance for mandates that are already in force.

---

## SLIDE 7 — OUR RESPONSE PROGRAMME

**Headline:** A Three-Tier, 12-Month Programme: Immediate Hardening → AI Defence → Strategic Posture

**Content:**

```
TIER 1 — IMMEDIATE (Months 1–3)                    Investment: ₹X crore
"Close the structural gaps before any AI attack can exploit them"
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
• Cross-cloud SIEM: GCP + AWS logs unified; cross-cloud attack detection live
• Jenkins hardening: Audit logging, plugin CVE gating, plugin whitelist
• Kubernetes admission control: OPA/Kyverno; blocks misconfigured pods
• Kubernetes runtime security: Falco; real-time threat detection in containers
• Jenkins credential rotation: All static keys → Vault dynamic secrets

TIER 2 — AI DEFENCE (Months 3–6)                  Investment: ₹X crore
"AI to fight AI: deploy the capabilities that match Mythos's speed"
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
• AI Gateway (LiteLLM Phase 1): Single hardened AI inference point
• AI-powered SIEM (Palo Alto XSIAM or Microsoft Sentinel)
• AI-assisted SAST triage: Checkmarx false-positive rate target: <15%
• Gemini security agents on CI/CD: AI code review on every PR
• Prompt injection hardening: Structural gateway protection

TIER 3 — STRATEGIC POSTURE (Months 6–12)          Investment: ₹X crore
"Future-proof the bank's defences against next-generation threats"
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
• AI Incident Copilot: AI-assisted P1/P2 response; human-in-the-loop
• Post-quantum cryptography: Crypto inventory + HSM procurement roadmap
• White-box cryptography: Pilot for payment processing workloads
• TIBER-IN engagement: Lobby IBA/RBI for India's red-team framework
• Palo Alto AI SOC: Production deployment; SOC automation live
```

**Total Programme Investment: ₹[X] crore over 12 months**
**Compared to:** C-Edge incident cost equivalent (operational disruption + regulatory + reputational) + ₹54.78 crore in peer bank penalties + ₹70,000 crore sector deepfake loss projections

---

## SLIDE 8 — THE AI GATEWAY: THE MOST CRITICAL DECISION

**Headline:** The AI Gateway Is the Linchpin — It Is Also the Highest-Value Attack Target

**Content:**

**What it is:** A single hardened AI inference point (LiteLLM + Gemini) that every security tool routes through — instead of each tool calling AI directly.

**Why it is critical:**
- Without it: tools make uncontrolled AI calls; data leaks; no audit trail; no redaction
- With it: every AI interaction is logged, redacted, rate-limited, and auditable by regulators

**Why it is also a risk:**
- LiteLLM was itself the target of a supply chain attack in 2025 (97 million monthly downloads compromised)
- Prompt injection attacks cost global financial services **$1.1 billion** in 2025

**Board decision required:** Approve the gateway architecture with the following non-negotiable controls:
1. All prompts pass through PII redaction (Microsoft Presidio + bank-specific patterns) before any AI sees data
2. Every AI interaction produces an audit record to SIEM — regulatorily defensible
3. Human approval required for any AI-initiated action that modifies production (not just read/summarise)
4. Quarterly adversarial red-team exercise against the gateway itself

**Speaker Note:** The board is not approving "AI for AI's sake." It is approving a specific, controlled, auditable architecture that is the foundation for every other AI defence capability in this programme.

---

## SLIDE 9 — THREAT INTELLIGENCE AND THE IBA DIMENSION

**Headline:** No Bank Can Defend Alone — We Need India's FS-ISAC

**Content:**

**The global model:** Financial Services Information Sharing and Analysis Center (FS-ISAC) — banks share attack indicators, breach patterns, and threat intelligence in real time. JPMorgan, HSBC, Goldman Sachs are all active members.

**India's gap:** No equivalent exists. The IBA coordination post-Mythos is a start — but it needs a technical execution layer.

**What we are proposing:**
- Lead or co-lead the IBA initiative to establish a **formal BFSI threat intelligence platform** (STIX/TAXII standard; real-time IOC sharing)
- Engage CERT-In/CSIRT-Fin as the government anchor for the platform
- Outcome: When Mythos attacks one Indian bank, all banks see the indicators within minutes

**The regulatory unlock we need:** Lobby RBI/IBA to establish **TIBER-IN** — India's equivalent of the EU's formal AI-assisted red-team framework. Without it, authorised Mythos-class offensive testing exists in regulatory grey territory.

**Board ask:** Authorise the CISO to formally represent the bank in IBA cybersecurity coordination discussions and to co-author the TIBER-IN proposal.

---

## SLIDE 10 — RISK QUANTIFICATION

**Headline:** The Cost of Not Acting Is Larger Than the Cost of the Programme

**Content:**

| Risk Scenario | Probability (12 months) | Estimated Financial Impact |
|---|---|---|
| Jenkins / CI-CD compromise (C-Edge precedent) | HIGH — identical vector already exploited in sector | Operational disruption + regulatory penalty: ₹50–200 crore |
| Undetected cross-cloud lateral movement → data breach | MEDIUM-HIGH — no SIEM currently | RBI penalty + customer notification + remediation: ₹100–500 crore |
| AI chatbot prompt injection → transaction fraud | HIGH once AI gateway live without protection | $47M precedent (hedge fund, 2025); retail bank equivalent: ₹100–400 crore |
| Deepfake-enabled executive wire fraud | MEDIUM — 47% of Indian adults already exposed | Single incident range: ₹5–50 crore |
| Regulatory non-compliance penalty | HIGH — mandates already past deadline | ₹54.78 crore peer benchmark; potential operating restrictions |

**Programme Investment:** ₹[X] crore  
**Expected Risk Reduction:** Closes 5 of 8 critical attack vectors within 6 months; all 8 within 12 months  
**Regulatory Compliance Value:** Addresses RBI Cyber Resilience Master Direction, SEBI CSCRF, and FREE-AI framework simultaneously

**Return on Security Investment (ROSI):** At even a 10% reduction in the median risk scenario, the programme pays for itself in Year 1.

---

## SLIDE 11 — GOVERNANCE MODEL

**Headline:** AI-Assisted Security Requires a New Governance Model — Human Authority Is Preserved

**Content:**

The board must be confident that AI in our security operations does not mean AI makes autonomous decisions without human accountability.

**Our governance principle:** AI advises, ranks, and explains. Humans approve, act, and are accountable.

| Action Type | AI Role | Human Step Required |
|---|---|---|
| Security alert triage | Classifies and prioritises | AppSec engineer reviews and approves suppression |
| Vulnerability finding | Proposes fix with rationale | Developer reviews; AppSec approves before merge |
| Incident response | Surfaces context and hypotheses | On-call engineer commands all actions |
| Deployment decision | Provides risk score | Deployment approver retains authority |
| Production system change | Cannot act — surface only | GitOps + human approver merges |

**AI Governance Council (proposed):** Risk, Compliance, AppSec, Platform Engineering, and a business representative. Owns: model promotion, prompt repository, use-case approval. Reports to: Risk Committee quarterly.

**Audit trail:** Every AI-assisted decision produces an immutable audit record (request ID, model, redacted input hash, output, downstream action). Regulatorily defensible under RBI IT Governance Master Direction.

---

## SLIDE 12 — WHAT WE ARE ASKING THE BOARD TO APPROVE

**Headline:** Three Approvals Required — Programme, Governance, and Regulatory Engagement

**Content:**

### Resolution 1 — Programme Investment Approval
Approve ₹[X] crore over 12 months for the three-tier AI Cyber Defence Programme as outlined in Slide 7, subject to phase-gate review after each tier.

### Resolution 2 — AI Governance Council
Establish the AI Governance Council with cross-functional membership (Risk, Compliance, AppSec, Platform Engineering, Business). Mandate: quarterly reporting to Risk Committee; owns AI model governance and the AI Use Standard.

### Resolution 3 — Regulatory Engagement Mandate
Authorise the CISO and Head of Legal to:
a) Formally represent the bank in IBA cybersecurity coordination (Mythos response)
b) Co-author the TIBER-IN proposal for RBI/IBA
c) Engage RBI for an interim AI offensive tool exemption (bounded scope, committed localisation architecture) to enable authorised red-team testing under TIBER-IN

**Timeline:** Tier 1 implementation begins within 30 days of board approval. Phase-gate presentations to Risk Committee at Month 3 and Month 6.

---

## SLIDE 13 — APPENDIX A: GLOSSARY

| Term | Plain-English Definition |
|---|---|
| Mythos | An AI-powered offensive security platform that can identify and exploit vulnerabilities at machine speed, significantly faster than human-operated attack tools |
| LiteLLM | Open-source software that acts as a single, controlled gateway between our security tools and AI models — like a controlled API router |
| SAST | Static Application Security Testing — automated code scanning that finds vulnerabilities before software is deployed |
| OPA/Kyverno | Policy enforcement tools that automatically block Kubernetes workloads that don't meet our security baseline |
| Falco | Open-source runtime security tool that watches what's happening inside running containers and alerts on suspicious behaviour |
| XSIAM | Palo Alto's AI-powered Security Operations platform — unified SIEM, threat detection, and automated response |
| TIBER-IN | Proposed India equivalent of the EU's Threat Intelligence-Based Ethical Red Teaming framework — a regulatory sandbox for authorised AI-powered offensive security testing |
| Prompt Injection | An attack where malicious instructions are hidden in data that an AI system reads, causing it to take unintended actions |
| STIX/TAXII | Industry-standard formats for sharing cybersecurity threat intelligence between organisations |
| PQC | Post-Quantum Cryptography — encryption algorithms designed to resist attacks from quantum computers, required by NIST by 2030–2035 |
| Zero Trust | A security model where no user, device, or system is trusted by default — every access request is verified |

---

## SLIDE 14 — APPENDIX B: KEY REGULATORY CITATIONS

| Regulation | Key Requirement Referenced | Source |
|---|---|---|
| RBI Cyber Resilience Master Direction (July 2024) | Zero Trust, micro-segmentation, AI-powered monitoring, vendor resilience standards | KPMG India Analysis |
| RBI FREE-AI Framework (August 2025) | Seven Sutras for responsible AI; AI Innovation Sandbox | RBI Official Publication |
| SEBI CSCRF (August 2024) | Red teaming mandate, post-quantum assessment, SOC requirements | SEBI Circular |
| CERT-In Mandate | 6-hour incident reporting; BFSI threat intelligence sharing | PIB / CERT-In |
| IRDAI ICS 2025 | Continuous monitoring, AI governance, third-party cloud security | IRDAI Guidelines |
| US Treasury FS AI RMF (February 2026) | 230 AI control objectives across governance, model risk, third-party risk | US Treasury |

---

## SLIDE 15 — APPENDIX C: PROGRAMME SUCCESS METRICS

| Metric | Baseline (Today) | Target (Month 6) | Target (Month 12) |
|---|---|---|---|
| Cross-cloud attack detection time | Not detectable | <4 hours | <30 minutes |
| Jenkins unauthorised change detection | Hours (manual) | <15 minutes | <5 minutes |
| Checkmarx false positive rate | >40% | <20% | <15% |
| Mean time to detect (MTTD) — production anomalies | Hours–days | 30% reduction | 50% reduction |
| Kubernetes policy compliance | Partial | 90% namespaces | 100% namespaces |
| AI-assisted triage coverage (% of security findings) | 0% | 60% | 90% |
| Regulatory compliance score (RBI/SEBI frameworks) | Partial | Substantially compliant | Fully compliant |
| Prompt injection detection rate | 0% (gateway not live) | 80% | 95% |

---

*Deck prepared by: CISO Office + AI Architecture Team*  
*Companion documents: mythos-bank-attack-analysis.md | global-bank-ai-defence-benchmark.md*  
*Classification: Board Confidential*
