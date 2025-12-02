# m{ai}geXR

> **From Conversation to Creation**  
> Democratizing Extended Reality development through AI-powered assistance

[![Platforms](https://img.shields.io/badge/Platforms-Android%20%7C%20iOS%20%7C%20Web-blue.svg)](https://github.com/m-ai-geXR)
[![AI Providers](https://img.shields.io/badge/AI%20Providers-5%2B-purple.svg)](https://github.com/m-ai-geXR)
[![3D Frameworks](https://img.shields.io/badge/3D%20Frameworks-5%2B-green.svg)](https://github.com/m-ai-geXR)
[![License](https://img.shields.io/badge/License-Open%20Source-brightgreen.svg)](LICENSE)

---

## 🔮 What is m{ai}geXR?

**maigeXR** (pronounced *"mage XR"*) is a cross-platform **AI-powered Extended Reality development platform** that transforms traditional 3D/XR development into an intuitive, conversational workflow.

By combining state-of-the-art AI models with production-grade 3D frameworks, maigeXR allows developers, designers, educators, and creators to generate immersive scenes through natural language — with no deep technical background required.

### 🎯 The Vision
**To make Extended Reality development as simple as having a conversation.**

```
You: "Create a spinning cube with rainbow colors"
AI:  Generates complete, production-ready 3D code
You: Click "Run Scene"
     → Watch your 3D scene come to life
```

---

## 📱 Platform Implementations

maigeXR runs on **Android**, **iOS**, and **Web**, each with unique optimizations but a shared architecture.

---

### 🤖 Android — [AndroidMaigeXr](https://github.com/m-ai-geXR/AndroidMaigeXr)

**Native Kotlin/Jetpack Compose Application**

- **Status:** Production-ready with active development  
- **Tech Stack:** Kotlin 1.9.20, Jetpack Compose, Material Design 3, Hilt  
- **Architecture:** MVVM + Clean Architecture with Room  
- **Features:**  
  - 5 3D libraries (Babylon.js, Three.js, React Three Fiber, A-Frame, Reactylon)  
  - Multiple AI providers (Together.ai, OpenAI, Anthropic)  
  - WebView + Monaco editor  
  - Encrypted API key storage  
  - Conversation history (Room SQLite)

📄 [Android Documentation](https://github.com/m-ai-geXR/AndroidMaigeXr)  
📘 [Android CLAUDE.md](https://github.com/m-ai-geXR/AndroidMaigeXr/blob/main/CLAUDE.md)

---

### 🍏 iOS — [iOSMaigeXr](https://github.com/m-ai-geXR/iOSMaigeXr)

**Native Swift/SwiftUI Application**

- **Status:** Production-ready with advanced features  
- **Tech Stack:** Swift 5.9+, SwiftUI, WebKit, AIProxy Swift  
- **Architecture:** MVVM with async/await  
- **Features:**  
  - 5 AI providers (Together.ai, OpenAI, Anthropic, Google AI, LlamaStack)  
  - Build system powered by Node.js + WebAssembly  
  - CodeSandbox integration  
  - Google AI/Gemini with 2M token context  
  - Temperature + Top-P parameter controls  
  - Automatic settings persistence

📄 [iOS Documentation](https://github.com/m-ai-geXR/iOSMaigeXr)  
📘 [iOS CLAUDE.md](https://github.com/m-ai-geXR/iOSMaigeXr/blob/main/CLAUDE.md)

---

### 🌐 Web — [WebMaigeXr](https://github.com/m-ai-geXR/WebMaigeXr)

**Next.js Progressive Web Application**

- **Status:** Standalone app for local development  
- **Tech Stack:** Next.js 14, React 18, TypeScript 5.3, Tailwind  
- **Architecture:** App Router + Zustand  
- **Features:**  
  - Browser-based development (no install required)  
  - SQL.js (client-side SQLite)  
  - Monaco editor  
  - Sandpack live preview  
  - Built-in build system with npm  
  - PWA support

📄 [Web Documentation](https://github.com/m-ai-geXR/WebMaigeXr/blob/main/CLAUDE.md)

> **Note:** The web version uses localStorage for API keys; intended for development only.

---

## 🚀 Core Features

### 🧠 Multi-Provider AI Integration

Switch between multiple AI providers seamlessly:

| Provider       | Best For                            | Pricing            | Streaming |
|----------------|--------------------------------------|---------------------|-----------|
| **Together.ai** | General 3D development, free models  | FREE – $0.80/1M     | Yes       |
| **OpenAI**      | Complex reasoning, GPT-4o           | $0.15 – $5.00/1M    | Yes       |
| **Anthropic**   | Code quality (Opus/Sonnet)          | $0.25 – $15.00/1M   | Yes       |
| **Google AI**   | Massive context (2M Gemeni)         | Free tier + paid    | Yes (SSE) |

**Included Free Models**
- DeepSeek R1 70B (Together)  
- Llama 3.3 70B (Together)  
- Gemini 2.5 Flash (Google AI)

---

### 🎨 3D Framework Support (5+ Libraries)

| Framework               | Type          | Best For                       | Size      | Curve |
|-------------------------|---------------|--------------------------------|-----------|--------|
| Babylon.js v8.22.3      | Engine        | XR, physics, complex scenes    | ~3MB      | Medium |
| Three.js r171           | Library       | Lightweight prototyping        | ~600KB    | Low    |
| React Three Fiber       | React Library | Component-based React 3D       | ~800KB    | Medium |
| A-Frame v1.7.0          | WebXR         | VR/AR declarative HTML         | ~1.2MB    | Low    |
| Reactylon 3.2.1         | React+Babylon | Professional XR for React      | ~3.5MB    | High   |

Each framework includes:

- Tailored AI prompts  
- Corrected API usage  
- Code templates  
- Optimized build pipeline  

---

### 🎛️ Professional AI Parameter Controls

**Temperature (0.0–2.0)**  
Controls creativity vs precision.

**Top-P (0.1–1.0)**  
Controls vocabulary diversity.

**Presets:**

- **Debugging Mode:** temp=0.2, top-p=0.3  
- **Balanced Mode:** temp=0.7, top-p=0.9  
- **Creative Mode:** temp=1.2, top-p=0.9  
- **Teaching Mode:** temp=0.7, top-p=0.8  

---

### ⚡ Real-Time Code Execution

Workflow:

1. User requests an XR scene  
2. AI generates full 3D code  
3. Monaco editor previews code  
4. Sandbox executes instantly  
5. Scene renders in real time  
6. User iterates or asks AI for changes  

**Execution Platforms**
- Android/iOS → WebView w/ JS bridge  
- Web → Sandboxed iframe  
- React Three Fiber → Sandpack + HMR + CodeSandbox  

---

### 🔐 Privacy-First Architecture

- All data stored **locally** on device  
- No analytics or tracking  
- Encrypted API keys on mobile  
- User-controlled AI provider selection  
- Optional cloud deployment via CodeSandbox  

**Storage Layers**
- Android → EncryptedSharedPreferences + Room  
- iOS → UserDefaults + Keychain  
- Web → localStorage + SQL.js  

---

## 🏗️ Architecture Overview

### Shared Design Pattern

All three platforms follow the same high-level approach:

\`\`\`
User Input → AI Provider → Code Generation → Editor → Execution → Preview
\`\`\`
