# PROPRIETARY LICENSE STRATEGY & COMPLIANCE FRAMEWORK

**lifecycleResearch Organization**  
**Last Updated:** June 16, 2026

---

## EXECUTIVE SUMMARY

This document outlines the licensing and visibility strategy for 230+ proprietary applications across the lifecycleResearch portfolio. 

**Key Directives:**
1. All **original proprietary code** → **PRIVATE** visibility + **proprietary licenses**
2. All **open-source forks** → **PUBLIC** visibility + **respect original licenses**
3. All **products** → discoverable via **grea.site** landing page URLs (not GitHub source)
4. All **government data integrations** → compliance documentation required

---

## PART 1: REPOSITORY CLASSIFICATION

### A. PROTECTED OPEN-SOURCE FORKS (Must Remain Public)

These repositories are derivatives of open-source projects. **Making them private violates their licenses.**

| Repository | Original License | Current Status | Action | Notes |
|---|---|---|---|---|
| `twenty` | AGPL v3 + Commercial License | PUBLIC | **KEEP PUBLIC** | Dual-licensed. Can modify but must offer source code to users. |
| `lago` | AGPL v3 | PUBLIC | **KEEP PUBLIC** | Network service → server-side modifications must be disclosed. |
| `midday` | AGPL v3 | PUBLIC | **KEEP PUBLIC** | Freelancer tools. AGPL requires source sharing. |
| `open-codesign` | MIT | PUBLIC | **KEEP PUBLIC** | MIT permissive. Can make private only with attribution. Recommend public. |
| `PlanExe` | MIT | PUBLIC | **KEEP PUBLIC** | MIT permissive. Same as above. |
| `modelzoo` | Apache 2.0 | PUBLIC | **KEEP PUBLIC** | Apache 2.0 allows commercial use. Must include license. |
| `Legal` | AGPL v3 | PUBLIC | **KEEP PUBLIC** | AGPL requires disclosure of modifications. |

**Legal Implication:** Violating these licenses opens you to cease-and-desist orders and potential litigation.

---

### B. ORIGINAL PROPRIETARY PRODUCTS (Recommend Private)

All repositories **NOT** listed above are original code written by lifecycleResearch. These can and should be **made private** with **proprietary licenses**.

#### **Tier 1: Core SaaS Platforms (5 repos)**
- `meridian` — Client retention service (landing)
- `meridian-app` — Next.js 14 SaaS app
- `meridian-mobile` — PWA mobile variant
- `meridian-web` — Express backend
- `meridian-saas` — Multi-product portfolio
- `grea-leads` — Lead generation SaaS
- `grea-site` — GREA homepage
- `grea-chatbot` — Chatbot integration
- `apex-hq` — Business operations hub
- `client-retention-services` — AI lead gen SaaS

#### **Tier 2: Content Creation Suite (50+ repos)**
All video/audio/media generation platforms:
- `ai-video-generation-engine`
- `animation-pilot`
- `audiobook-builder`
- `audiobook-narration-pilot`
- `corporate-video-suite`
- `documentary-builder`
- `educational-video-content-hub`
- `explainer-video-suite`
- `food-video-content-suite`
- `gaming-video-content-forge`
- `interactive-fiction-pro`
- `interactive-video-content-forge`
- `jingle-studio`
- `kids-builder`
- `live-stream-engine`
- `lyric-video-flow`
- `meditation-studio`
- `multilingual-video-content-pro`
- `music-forge`
- `music-remixing-platform`
- `music-theory-flow`
- `music-video-studio`
- `pet-engine`
- `podcast-advertising-builder`
- `podcast-hub`
- `podcast-intro-pro`
- `real-estate-video-flow`
- `short-film-studio`
- `sports-video-content-pilot`
- `travel-video-content-platform`
- `video-builder`
- `video-color-grading-hub`
- `video-compilations-engine`
- `video-dubbing-pro`
- `video-editing-suite`
- `video-intro-forge`
- `video-marketing-content-platform`
- `video-response-campaigns-pro`
- `video-restoration-hub`
- `video-script-writing-platform`
- `video-seo-optimization-pilot`
- `video-sourcing-engine`
- `video-testimonials-suite`
- `video-transcription-flow`
- `virtual-event-hub`
- `voiceover-studio`
- `wedding-video-editing-pro`
- `zoom-platform`
- `asmr-audio-forge`
- `audio-cleaning-flow`
- ... and more

#### **Tier 3: AI & Intelligence Systems (5 repos)**
- `deer-flow` — Long-horizon agent framework (MIT licensed, recommend PRIVATE + Proprietary)
- `shadowbroker` — Geopolitical intelligence
- `Qwen-Image-Edit-2511-LoRAs-Fast-Lazy-Load` — Image editing
- `gigaGPT` — Large model training
- `codec` — Command layer (MIT licensed, recommend PRIVATE + Proprietary)

#### **Tier 4: Business/Utility Tools (20+ repos)**
- `microsaas-crm`
- `garage-sale-inventory`
- `vendor`
- `pima-taxlien-webapp`
- `solvent-recycling-tucson`
- `smokeshop-pro`
- `check-if-email-exists`
- `ringless-voip-app`
- `saas-product-generator`
- `digital_barista`
- `spec_md_files`
- `hermes-profile-templates`
- `horizons-export-ai-age-improved`
- `rick-industrybyrick`
- `openfans-audited`
- `openfans-dark`
- `Herb`
- `Enviro`
- `USB`
- `design` (Shadow Design System - Apache 2.0, recommend PRIVATE + Proprietary fork)

---

## PART 2: RECOMMENDED LICENSE STRATEGY BY PRODUCT TYPE

### **SaaS Platforms** (Private + Proprietary)

**Recommended License:** `COMMERCIAL - PROPRIETARY LICENSE v1.0`

```
Subject Matter: Enterprise SaaS, multi-tenant, API access
Restrictions: 
  - No redistribution without license agreement
  - No reverse engineering
  - No creating derivative works for commercial purposes
  - Single-tenant or multi-tenant deployment only per agreement
  - Audit rights reserved
Components to declare:
  - Next.js 14 (MIT) ✅
  - Supabase (Apache 2.0 / Postgres) ✅
  - Stripe SDK (proprietary) ✅
  - Resend email (proprietary) ✅
  - AWS SES (proprietary) ✅
Attribution: Required in documentation
```

**Examples:**
- `meridian-saas` 
- `client-retention-services`
- `grea-leads`
- `apex-hq`

---

### **Content Creation Tools** (Private + Proprietary)

**Recommended License:** `COMMERCIAL - CONTENT GENERATION LICENSE v1.0`

```
Subject Matter: AI-powered content generation, video/audio production
Restrictions:
  - API-only distribution (no source code exposure)
  - Per-seat or per-API-call pricing model
  - No commercial use of generated IP without additional license
  - White-label available under separate agreement
Components to declare:
  - OpenAI APIs (proprietary, ToS restricted)
  - Anthropic Claude (proprietary, ToS restricted)
  - Audio libraries (various)
  - Video encoding (FFmpeg - GPL? → Need to verify)
Attribution: Not typically exposed (API-only)
```

**Examples:**
- All 50+ video/audio generation repos
- `ai-video-generation-engine`
- `audiobook-builder`
- `corporate-video-suite`

---

### **AI Frameworks** (Private + SSPL or Modified Proprietary)

**Recommended License:** `SERVER SIDE PUBLIC LICENSE (SSPL) v1.0`

```
Subject Matter: Agent frameworks, LLM orchestration, inference systems
Restrictions:
  - If offered as a service, must provide source code to users
  - Can be used privately without disclosure
  - Commercial deployment allowed with SSPL compliance
Components to declare:
  - LLM libraries (Ollama, etc. - open source)
  - Inference engines
  - Vector databases
Attribution: Required if based on OSS
```

**Examples:**
- `deer-flow` (currently MIT, change to SSPL + Proprietary)
- `codec` (currently MIT, change to SSPL + Proprietary)

---

### **Intelligence/Data Systems** (Private + Data Rights License)

**Recommended License:** `COMMERCIAL - DATA LICENSE v1.0`

```
Subject Matter: Geopolitical data aggregation, satellite/aviation tracking
Restrictions:
  - Government/regulatory compliance required
  - Data attribution mandatory (satellite providers, aviation databases)
  - No redistribution of underlying data without separate license
  - Audit rights for regulatory compliance
  - Re-export controls (EAR/ITAR) may apply
Components to declare:
  - Public satellite data (various government sources)
  - Aviation tracking APIs
  - Seismic data (USGS, etc.)
Attribution: REQUIRED - government data sources must be cited
```

**Examples:**
- `shadowbroker` — **COMPLIANCE CRITICAL**

---

## PART 3: GOVERNMENT DATA COMPLIANCE

### **SHADOWBROKER — CRITICAL REVIEW REQUIRED**

Repository: `shadowbroker` — "Open-source geopolitical intelligence platform"

**Current Concerns:**

1. **Data Sources:**
   - Corporate jet tracking → ADS-B Exchange (open data)
   - Satellite monitoring → Likely public ephemeris data (TLE - Two-Line Elements)
   - Seismic events → USGS (public API)

2. **Regulatory Implications:**
   - **Export Controls:** If tracking foreign military/government assets, may be **ITAR-controlled** (International Traffic in Arms Regulations)
   - **Re-export:** Publishing satellite tracking may violate Commerce Control List (CCL)
   - **Jurisdiction:** May require OFAC/BIS review

3. **Legal Status:**
   - Making source code **open-source** (current Python repo) may expose you to export violation claims
   - Even publishing on GitHub can constitute "publication" under ITAR

**Recommendation:**

```
⚠️ LEGAL REVIEW REQUIRED BEFORE PROCEEDING

Action Items:
1. Consult with export compliance attorney
2. Review data sources for ITAR/EAR applicability
3. If ITAR-controlled:
   - Make PRIVATE immediately
   - Add ITAR notice to code
   - Restrict access to US persons only
   - Audit current public exposure
4. If not ITAR-controlled:
   - License as: COMMERCIAL - DATA LICENSE v1.0
   - Add attribution headers for all government data sources
   - Document data refresh rates and sources
5. Consider consulting:
   - BIS (Bureau of Industry and Security)
   - Your insurance provider
```

---

## PART 4: ACTION PLAN - MIGRATION STRATEGY

### **Phase 1: Secure Forks (Do NOT Change)**
```
No action. These must remain public and open-source.
- twenty, lago, midday, open-codesign, PlanExe, modelzoo, Legal
```

### **Phase 2: Audit Original Code (Week 1)**
```
For each proprietary repo:
1. Verify ownership (did we write it all, or did we use open-source?)
2. Scan dependencies (npm audit, pip audit)
3. Document ALL external components (APIs, libraries)
4. Flag government data integrations
5. Check for accidentally committed secrets (API keys, etc.)

Tools:
- npm ls / pip freeze (dependency tree)
- SPDX scanner (license audit)
- Snyk (vulnerability check)
- GitHub CodeQL (secret scanning)
```

### **Phase 3: Apply Proprietary Licenses (Week 2-3)**
```
For each original proprietary repo:

1. Create LICENSE file:
   - Copy appropriate template from PART 2
   - Customize for that repo type
   - Add current year and company name

2. Update README.md:
   - Add: "⚠️ PROPRIETARY - All rights reserved"
   - Add licensing terms summary
   - Add: "White-label available: contact sales@grea.site"

3. Add license header to all source files:
   // PROPRIETARY LICENSE - (repo name)
   // Copyright (c) 2026 lifecycleResearch. All rights reserved.
   // See LICENSE file for commercial licensing terms.
```

### **Phase 4: Change Visibility to Private (Week 3)**
```
Via GitHub API or CLI for each repo:

gh repo edit lifecycleResearch/[repo-name] --private

Or batch script:
for repo in $(cat private-repos.txt); do
  gh repo edit lifecycleResearch/$repo --private
done

Repos to privatize: ~220 repos (all except the 7 forks)
```

### **Phase 5: Create Landing Page URL Mapping (Week 4)**
```
On grea.site, create product discovery pages:

https://grea.site/products/meridian → Private repo (private-repo-not-shown)
https://grea.site/products/ai-video → Private repo (private-repo-not-shown)
https://grea.site/products/content-suite → List of 50+ private repos
https://grea.site/products/shadow-intelligence → Private repo (legal review link)

Benefits:
- Users discover products via URL (not GitHub source)
- Source code stays private
- Marketing can highlight features without exposing implementation
```

---

## PART 5: LICENSE TEMPLATES

### **Template A: COMMERCIAL - PROPRIETARY LICENSE v1.0**

```
PROPRIETARY LICENSE - [PRODUCT NAME]
© 2026 lifecycleResearch. All Rights Reserved.

GRANT:
This software is proprietary and confidential. You are granted a limited,
non-exclusive, non-transferable license to use this software solely for the
purposes authorized in a separate written agreement with lifecycleResearch.

RESTRICTIONS:
- No reproduction, distribution, or transmission without written consent
- No reverse engineering, decompilation, or disassembly
- No derivative works for commercial purposes
- No sublicensing or leasing

OPEN SOURCE COMPONENTS:
This software includes open-source components licensed under:
[List all OSS dependencies with their licenses]

LIMITATION OF LIABILITY:
To the fullest extent permitted by law, lifecycleResearch is not liable for
any damages arising from use of this software.

TERMINATION:
This license is effective until terminated. Your rights terminate if you
violate any provision of this agreement.
```

### **Template B: SERVER SIDE PUBLIC LICENSE (SSPL) v1.0 + Proprietary**

```
SSPL + PROPRIETARY DUAL LICENSE - [PRODUCT NAME]
© 2026 lifecycleResearch. All Rights Reserved.

You may use this software under either:

1. SSPL LICENSE (Free, but with conditions):
   - Can use internally without restriction
   - If offered as a service, must make source code available to users
   - See https://www.mongodb.com/licensing/server-side-public-license

2. PROPRIETARY COMMERCIAL LICENSE (Paid):
   - Full commercial rights
   - Service deployment without SSPL obligation
   - Priority support and SLA
   - Contact: sales@grea.site
```

### **Template C: COMMERCIAL - DATA LICENSE v1.0**

```
COMMERCIAL - DATA LICENSE - [PRODUCT NAME]
© 2026 lifecycleResearch. All Rights Reserved.

GRANT:
Licensee receives a limited, revocable license to access and use aggregated
data and analytics provided by this software.

DATA SOURCES & ATTRIBUTION:
This software aggregates data from:
- USGS Earthquake Hazards Program (public domain)
- ADS-B Exchange (Creative Commons Attribution 4.0)
- [Other sources...]

RESTRICTIONS:
- No redistribution of underlying data without separate license
- Regulatory compliance: Licensee is responsible for export controls
- Audit rights: Licensor retains the right to audit compliance

EXPORT COMPLIANCE:
Licensee certifies it is not subject to US trade embargoes or sanctions.
If applicable, Licensee agrees to comply with EAR/ITAR regulations.

DATA RETENTION & PRIVACY:
Licensee agrees to retain access logs for regulatory review.
```

---

## PART 6: REPOSITORY ACTION CHECKLIST

### **SaaS Platforms (Make Private)**

- [ ] `meridian` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `meridian-app` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `meridian-mobile` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `meridian-web` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `meridian-saas` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `client-retention-services` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `grea-leads` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `grea-site` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `grea-chatbot` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `apex-hq` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `microsaas-crm` — COMMERCIAL - PROPRIETARY LICENSE v1.0

### **Content Creation (Make Private)**

- [ ] `ai-video-generation-engine` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `animation-pilot` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `audiobook-builder` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `audiobook-narration-pilot` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `corporate-video-suite` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `documentary-builder` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `educational-video-content-hub` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `explainer-video-suite` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `food-video-content-suite` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `gaming-video-content-forge` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `interactive-fiction-pro` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `interactive-video-content-forge` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `jingle-studio` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `kids-builder` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `live-stream-engine` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `lyric-video-flow` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `meditation-studio` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `multilingual-video-content-pro` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `music-forge` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `music-remixing-platform` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `music-theory-flow` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `music-video-studio` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `pet-engine` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `podcast-advertising-builder` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `podcast-hub` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `podcast-intro-pro` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `real-estate-video-flow` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `short-film-studio` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `sports-video-content-pilot` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `travel-video-content-platform` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `video-builder` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `video-color-grading-hub` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `video-compilations-engine` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `video-dubbing-pro` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `video-editing-suite` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `video-intro-forge` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `video-marketing-content-platform` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `video-response-campaigns-pro` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `video-restoration-hub` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `video-script-writing-platform` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `video-seo-optimization-pilot` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `video-sourcing-engine` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `video-testimonials-suite` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `video-transcription-flow` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `virtual-event-hub` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `voiceover-studio` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `wedding-video-editing-pro` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `zoom-platform` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `asmr-audio-forge` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] `audio-cleaning-flow` — COMMERCIAL - CONTENT GENERATION LICENSE v1.0
- [ ] (+ ~10 more content repos)

### **AI Frameworks (Make Private)**

- [ ] `deer-flow` — SSPL v1.0 + PROPRIETARY LICENSE
- [ ] `codec` — SSPL v1.0 + PROPRIETARY LICENSE
- [ ] `Qwen-Image-Edit-2511-LoRAs-Fast-Lazy-Load` — COMMERCIAL - AI LICENSE v1.0
- [ ] `gigaGPT` — COMMERCIAL - AI LICENSE v1.0

### **Intelligence Systems (Make Private + Legal Review)**

- [ ] `shadowbroker` — **AWAITING LEGAL REVIEW** (ITAR compliance check)

### **Business Tools (Make Private)**

- [ ] `garage-sale-inventory` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `vendor` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `pima-taxlien-webapp` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `solvent-recycling-tucson` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `smokeshop-pro` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `check-if-email-exists` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `ringless-voip-app` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `saas-product-generator` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `digital_barista` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `spec_md_files` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `hermes-profile-templates` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `horizons-export-ai-age-improved` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `rick-industrybyrick` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `openfans-audited` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `openfans-dark` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `Herb` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `Enviro` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `USB` — COMMERCIAL - PROPRIETARY LICENSE v1.0

### **Design Systems (Make Private)**

- [ ] `lifecycleresearch` (Shadow DS) — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `design` — COMMERCIAL - PROPRIETARY LICENSE v1.0
- [ ] `ant` → **Migrate to shadow-design-private** or keep as MIT fork

### **Keep PUBLIC (Open-Source Forks)**

- ✅ `twenty` — AGPL v3 + Commercial (unchanged)
- ✅ `lago` — AGPL v3 (unchanged)
- ✅ `midday` — AGPL v3 (unchanged)
- ✅ `open-codesign` — MIT (unchanged)
- ✅ `PlanExe` — MIT (unchanged)
- ✅ `modelzoo` — Apache 2.0 (unchanged)
- ✅ `Legal` — AGPL v3 (unchanged)
- ✅ `awesome-selfhosted` — Other license (unchanged)

---

## PART 7: IMPLEMENTATION NOTES

### **Dependencies to Review:**
- `antd` (Ant Design) — MIT licensed. Can fork and make private copy.
- FFmpeg — LGPL/GPL (may have restrictions). Review video repos.
- Audio libraries — Audit each video/audio repo for GPL components.

### **API Dependencies (No License Risk):**
- OpenAI APIs — Proprietary SaaS. No license risk.
- Anthropic Claude — Proprietary SaaS. No license risk.
- Stripe — Proprietary SaaS. No license risk.
- Supabase — Open source (PostgreSQL) but cloud service, no redistribution.
- AWS SES — Proprietary SaaS. No license risk.

### **Next Steps:**
1. **This week:** Legal review of `shadowbroker` for export controls
2. **Next week:** Apply licenses to all 220 proprietary repos
3. **Week 3:** Change visibility to private
4. **Week 4:** Create landing page URL map on grea.site
5. **Ongoing:** Add proprietary license headers to all source files

---

## APPENDIX: LICENSE SELECTION FLOWCHART

```
Does the code contain/depend on open-source components?
├─ YES → Check if GPL/AGPL
│   ├─ YES → MUST stay PUBLIC (forks)
│   └─ NO (MIT/Apache) → Can privatize if original code dominates
└─ NO → Can be PRIVATE + PROPRIETARY

Is it a network service (API/SaaS)?
├─ YES → Consider SSPL or PROPRIETARY
└─ NO → PROPRIETARY

Does it use government data?
├─ YES → Check export controls (ITAR/EAR)
│   ├─ YES → Privatize + add compliance notice
│   └─ NO → PROPRIETARY + DATA LICENSE
└─ NO → PROPRIETARY

Does it use third-party APIs?
├─ YES → Add attribution to LICENSE file
└─ NO → PROPRIETARY
```

---

**Document Prepared By:** GitHub Copilot  
**For:** lifecycleResearch  
**Status:** DRAFT - Awaiting legal review and confirmation  
**Next Review:** After implementation phase 1-2
