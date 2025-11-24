# 🏥 Bangladesh Healthcare AI Agent (Google x Kaggle Capstone)

This project is my Capstone submission for the **5-Day AI Agents Intensive Course with Google**. It is an AI agent that helps Bangladeshi users understand their health symptoms and find nearby hospitals, using Bangla-English mixed language and the Gemini API via ADK.


## 📋 Project Summary

**Category:** Healthcare AI Agent  
**Target Region:** Bangladesh 
**Language:** Bangla-English mixed  
**Framework:** Google Agent Development Kit (ADK)  
**Model:** Gemini 2.5 Flash Lite  
**Level:** Level 2 Strategic Problem-Solver (multi-tool orchestration)  

**Key Features:**
- ✅ Symptom triage (emergency/moderate/mild classification)
- ✅ Hospital finder 
- ✅ Medicine reminder setup guide
- ✅ Safe, responsible health guidance (not a doctor, always recommends consultation)
- ✅ Bangla-English mixed responses for accessibility

## 🎯 Problem & Motivation

In Bangladesh, especially in cities like Sylhet and Dhaka:
- Many people don't know when a health symptom is **mild**, **needs a doctor soon**, or is an **emergency**
- Hospital information is scattered and not easily accessible in Bangla
- Students and families often rely on unreliable sources for health guidance
- Medical consultations are expensive and hospitals are crowded

**This agent helps by:**
- Providing simple Bangla-English triage guidance
- Suggesting nearby hospitals for serious cases
- Helping users set medicine reminders
- Always reminding users to consult real doctors for treatment

**Target users:** Students, families, and general public in Bangladesh who need quick health guidance in their preferred language.

**Tech Stack:**
- Google ADK for agent framework
- Gemini 2.5 Flash Lite as LLM
- 3 custom Python FunctionTools
- InMemoryRunner for orchestration

**Submission for:** Google x Kaggle 5-Day AI Agents Intensive Course - Capstone Project

## 🧠 Agent Architecture & Workflow

User Query (Bangla-English mixed)

↓

[Level 2 Strategic Agent]
(Gemini 2.5 Flash Lite + ADK)

↓

Step 1: triage_symptoms tool

↓

Classification: emergency / moderate / mild

↓ 

Step 2: Conditional tool selection

├─ Emergency → find_nearby_hospitals (MUST call)

│ + Strong hospital recommendation

├─ Moderate → find_nearby_hospitals (recommended)

│ + Self-care tips + doctor suggestion

└─ Mild → Home care tips

+ setup_medicine_reminder (if requested)
+ Optional hospital info (if asked)

↓

Step 3: Combine all tool outputs

↓

Final Answer (safe, clear, Bangla-English)

"Not a doctor" disclaimer

"Consult real doctor" reminder


**Design Principles:**
- Safety First: Emergency cases prioritized
- Multi-tool Orchestration: Agent chooses appropriate tools based on severity
- Context-Aware: Bangla-English mix for Bangladesh users
- Responsible AI: No prescriptions, always recommends professional consultation

## 🎓 Conclusion

This capstone project demonstrates:
- **Level 2 Strategic Agent** using Google ADK and Gemini 2.5 Flash Lite
- **Multi-tool orchestration** with 3 custom FunctionTools
- **Real-world problem solving** for healthcare access in Bangladesh
- **Responsible AI** design with safety-first approach
- **Local context awareness** through Bangla-English language support

The agent successfully triages symptoms, suggests hospitals, and helps with medication reminders while maintaining strict safety guidelines and always recommending professional medical consultation.

**Thank you for reviewing this submission!** 


**Author:** Tarequl Islam, Undergraduate Student, 5th Semester, Department of Statistics, SUST.

**Course:** Google x Kaggle 5-Day AI Agents Intensive

**Date:** November 21, 2025

