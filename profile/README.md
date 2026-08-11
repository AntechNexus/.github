# Nexus AI: The Intelligent Product Management Workspace

<div align="center">
  <img src="assets/Logo-nexus.png" alt="Nexus AI Logo" width="200" height="200">
</div>

<!-- Profile Views -->
<div align="center">
  <img src="https://komarev.com/ghpvc/?username=nexus-ai-org&style=flat-square&color=blue" alt="Profile views" />
</div>

## 📖 Project Description

**Nexus AI** is a comprehensive, artificial intelligence-powered product management system designed to accelerate the workflow of Product Managers and engineering teams. Nexus enables users to create, manage, and automate the generation of Product Requirements Documents (PRD), and provides an AI assistant (*Ask Nexus*) capable of answering specific questions based on the context of project documents using Retrieval-Augmented Generation (RAG).

### 🎯 Core Objectives
- Accelerate the creation cycle of product specification documents (PRDs).
- Eliminate miscommunication between team members (PMs, Designers, Engineers) through a *Single Source of Truth*.
- Facilitate the search for specific information within a sea of project documents using Retrieval-Augmented Generation (RAG).
- Provide an integrated workspace (Files, Folders, Teams) in a single, modern dashboard.

## 🏗️ System Architecture

```
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   Frontend      │    │ Backend (Nexus)  │    │ Backend (AI)    │
│   (React +      │◄──►│ (Express.js +    │◄──►│ (Express.js +   │
│   Tailwind)     │    │  MongoDB)        │    │  Gemini API)    │
└─────────────────┘    └──────────────────┘    └─────────────────┘
         │                       │                       │
         │                       │                       │
         ▼                       ▼                       ▼
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│  Interactive UI │    │  Auth & Storage  │    │ RAG & Embeddings│
│  Real-time SSE  │    │  RBAC & Teams    │    │ PRD Generation  │
└─────────────────┘    └──────────────────┘    └─────────────────┘
```

## 🚀 Key Features

### 🤖 Artificial Intelligence (AI) Features
- **AI PRD Generator**: Generate comprehensive PRDs from random draft documents or audio transcripts using Google Gemini.
- **Ask Nexus (RAG Copilot)**: An AI chat feature that understands 100% of your project's context. Ask about project specifications, and the AI will answer with direct citations to the original documents!
- **Clarification Wizard**: The AI intelligently asks about "missing details" from your drafts before generating the final PRD.

### 💻 Frontend
- **Modern Interface**: Built with **React 18** and **Tailwind CSS**.
- **Interactive UX**: Supports Drag & Drop for file and directory management.
- **Fast Data Fetching**: Highly efficient Axios integration for a seamless experience.

### ⚙️ Backend & Infrastructure
- **Microservices-ish**: Separation between the Core Service (Project Management, Authentication) and the AI Service (AI Generation, Text Embedding).
- **Scalable Database**: Uses **MongoDB** to store file metadata, users, teams, and document embedding vectors.
- **Secure Authentication**: OTP system, password reset, and JWT.

## 👥 Development Team

**Team**: Antech Antech Async*  

| Name | Learning Path | Github |
|----- |---------------|--------| 
| **Timothy Julian** | Project Manager | [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)]([https://github.com/RefaMuhammad](https://github.com/tjjulian16)) |
| **Refa Muhammad** | Tech Lead & Machine Learning Engineer | [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/RefaMuhammad) |
| **Fairiza Naghda Biwai** | Full Stack Developer | [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/zet-nbs) |
| **Kamila Izzati** | Frontend Developer | [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/kamilaizzati) |
| **Ria Kristi** | Backend Developer | [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/riakrst) |

## 🙏 Acknowledgments

- **Google Gemini API** for the main brain behind the AI features (Ask Nexus and PRD Generation).
- **React & Tailwind Community** for the incredible frontend ecosystem.
- **MongoDB** for the flexible database solution.
