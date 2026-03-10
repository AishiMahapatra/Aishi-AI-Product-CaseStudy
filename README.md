# Agentic KYC FastPass

An automated, multi-agent orchestration system that handles end-to-end customer onboarding by autonomously extracting document data, validating identities, and performing real-time quality checks.


## 🚀 The Problem
Traditional KYC (Know Your Customer) in banking is high-friction, often taking up to 72 hours for manual review. This leads to high drop-off rates and increased operational costs. Rule-based systems fail on "unstructured data" like blurry ID photos; Agentic AI "plans" a recovery by asking the user for specific corrections.

## 🏗 Technical Architecture
The system utilizes a decoupled, event-driven architecture:
* **Frontend:** v0 
* **Orchestration:** n8n (Multi-agent workflow logic)
* **Reasoning:** OpenAI GPT-4o (Vision & Extraction)

### Multi-Agent Flow
1. **Validator Agent:** Inspects image quality (glare/blur/framing).
2. **Extraction Agent:** Converts ID images into structured JSON data.
3. **Evaluation Agent:** Scores the output based on the **HHH (Helpful, Honest, Harmless) Framework** to ensure data integrity.

## 📊 Evaluation & Metrics
* **North Star Metric:** Reduce Time-to-Account-Open from 72 hours to <10 minutes.
* **Accuracy:** Target >95% extraction precision for government-issued IDs (US Driving Licenses for MVP)
* **Safety:** Integrated HHH evaluation agent to prevent hallucinated data fields.

## 📂 Project Structure
* `/documentation`: Full Product Requirements Document (PRD).
* `/workflows`: n8n JSON workflow files for backend orchestration.

  
