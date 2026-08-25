# SetuLingua-AI
An offline-first, Speech-to-Speech (S2S) and Speech-to-Text (S2T) bilingual pedagogy suite engineered 

## 🎨 Interactive UI Prototype Layout
We have engineered a highly responsive, user-centric mobile interface inspired by Jharkhand's natural landscapes. You can explore our live, comprehensive screen designs and multi-agent console views directly via our Figma canvas:

👉 **[Click Here to View Our Live Figma Interactive UI Mockup](https://www.figma.com/make/pLCjbE1pxeNraBkaiXKb34/Premium-Teacher-Android-Screen?fullscreen=1&t=kWgUjzBwl2CIFQPE-1&code-node-id=0-9)**

### 🌐 Note on UI Localisation & Dynamic String Swapping
Please note that the English/हिंदी toggle button on the Figma canvas is a static visual placement. 

During the 30-hour City Battle, this feature will be fully implemented using native Android local resource configurations (`strings.xml` bundles). When the toggle is flipped, our Jetpack Compose UI engine will dynamically swap text vectors completely on-device with zero latency, entirely offline. Subagent 4 (The UI Architect) will automatically recalculate text container heights and line spacing to adapt to Devanagari script padding rules, preventing layout clipping.
## 🛠️ On-Device System Architecture
*   **Local AI Core Engine:** Mapped directly to the iQOO Hardware NPU via Android NNAPI using an offline Ollama local loopback container (Port 11434).
*   **Linguistic AI Model Base:** Quantized INT4 GGUF weights of the Nous Research Hermes-3 model.
*   **Mobile Interface Platform:** Native Android written in Kotlin & Jetpack Compose using a dual-state environmental theme (Sunlit Canopy Light / Forest Night Dark).

## 🗂️ Pre-Planned Project Directory Framework
├── android/                  # Native Android Kotlin Application Codebase
│   └── app/src/main/java/com/iqoo/setulingua/engine/MultiAgentOrchestrator.kt
├── ollama_config/            # Offline Model Parameter Configuration Files
│   ├── Modelfile.leader      # Subagent 1: Grammatical Translator
│   └── Modelfile.pedagogy    # Subagent 2: NIPUN Bharat FLN Auditor
