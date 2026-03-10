# Agentic KYC FastPass: Product Requirements Document (PRD) Summary - 1 Pager

## 1. Problem Definition
Traditional KYC (Know Your Customer) in banking is high-friction, often taking up to 72 hours for manual review.This leads to high drop-off  rates and increased operational costs for US-based financial firms. 

**Why Agentic AI?** Standard rule-based systems fail on "unstructured data" like blurry ID photos. This system uses Agentic AI to "plan" a recovery—autonomously asking the user for specific corrections (e.g., "Please retake the photo without glare"). 

## 2. Solution Overview
An automated, multi-agent orchestration system that handles end-to-end customer onboarding. [cite: 4]

### Key Components
* **Image Quality Validator Agent:** Detects glare, blur, and framing issues using Vision LLMs. [cite: 28, 55]
* **Document Extraction Agent:** Vision-based data extraction from government IDs with >95% accuracy. [cite: 29]
* **Deterministic Decision Journal:** Provides a clear audit trail for every automated approval or flag to meet SEC/FINRA standards. 

## 3. Core Metrics
*North Star Metric:** Reduce Time-to-Account-Open from 72 hours to <10 minutes.
**Secondary Metric:** False Rejection Rate (Ensuring legitimate customers aren't blocked). 

## 4. Risk Assessment & Responsible AI
| Component | Risk Level | Mitigation Strategy |
| :--- | :--- | :--- |
| Image Validation | Low | Using Vision LLMs to detect visual artifacts. 
| Document Extraction | Low | Manual verification for data fields; >[cite_start]95% accuracy goal. 
| Self-Correction | High | [cite_start]Routing to human-in-the-loop if automation fails 3 times. 

**Privacy & Bias:** The system implements PII redaction and is audited for demographic bias in the manual review queue. 

## 5. Roadmap
* **MVP:** Approve low-risk retail customers with US Driver’s Licenses only (6-8 weeks).
* **Phase 2:** Support for other US Gov IDs and Utility Bills (8-10 weeks).

## 6. Detaild PRD Link (Google Doc)
https://docs.google.com/document/d/17NzzgnugslPehR4gtPcdnhAXYEz0Ly6gaXg40buI0tM/edit?tab=t.0#heading=h.h5j7feud39z1 
