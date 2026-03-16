My Linkedin: https://www.linkedin.com/in/aishi-mahapatra-4638178/

# Agentic KYC 

An automated, multi-agent orchestration system that handles end-to-end customer onboarding by autonomously extracting document data, validating identities, and performing real-time quality checks.


## 🚀 The Problem
Traditional KYC (Know Your Customer) in banking is high-friction, often taking up to 72 hours for manual review. This leads to high drop-off rates and increased operational costs. Rule-based systems fail on "unstructured data" like blurry ID photos; Agentic AI "plans" a recovery by asking the user for specific corrections.

## 🏗 Technical Architecture
The system utilizes a decoupled, event-driven architecture:
* **Frontend:** v0 
* **Orchestration:** n8n (Multi-agent workflow logic)
* **Reasoning:** OpenAI GPT-4o (Vision & Extraction)

## Proof of Concept Artifacts
* Frontend: V0 https://v0-kyc-landing-page-2b.vercel.app/
* Backend: n8n
* <img width="937" height="531" alt="image" src="https://github.com/user-attachments/assets/d4af49fa-0124-4ca5-b1f1-525d2f4fe700" />

* <img width="754" height="443" alt="image" src="https://github.com/user-attachments/assets/6f130fc1-69ff-4df0-ae96-8e66343890a4" />



## 📊 Evaluation & Metrics
* **North Star Metric:** Reduce Time-to-Account-Open 
* **Accuracy:** Target >95% extraction precision for government-issued IDs (US Driving Licenses for MVP)
* **Safety:** Integrated HHH evaluation agent to prevent hallucinated data fields.

## 📂 Project Structure
* `/documentation`: Full Product Requirements Document (PRD).
* `/workflows`: n8n JSON workflow files for backend orchestration.
* *(Detailed 15-page+ Internal PRD available for review upon request)*.

  
