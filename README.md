# client-sidecar-ai-preview
Client-Sidecar AI is a 100% client-sided, lightweight, highly optimized multi-LLM provider (OpenAI GPT, Anthropic Claude, Google Gemini) native browser extension. Designed with Vanilla JS and strictly Manifest V3 compliant for security-conscious users. It features a pure Bring-Your-Own-Key (BYOK) model, with $0/month hosting overhead infrastructure and absolute local data privacy. 

This project is structured as a production-ready, white-label product, giving developers and creators a highly modular foundation to immediately rebrand, customize, and launch their own private AI browser assistant.

---

## The End-User Experience (User's POV):
The core flow is completely frictionless:
* **BYOK Model**: The user opens the settings panel, paste their own private OpenAI, Claude or Gemini API keys, and click save. Their keys are stored 100% locally and securely.
* **Highlight & Capture**: User highlights text on any webpage, right-clicks, and selects "Send page content to Client-Sidecar AI".
* **Workspace Wakeup**: With the side-panel open or it can also instantly slide open on its own, smoothly ingesting the selected text and automatically scrolling down so the typing cursor is ready.
* **Prompt & Export**: The user chats with their chosen model in real time. With a single click, they can instantly export their entire chat history into a cleanly formatted Markdown (.md) file.

---

## Core Features & Engineering Highlights:
* **BYOK Architecture**: Secure integration vectors for OpenAI, Claude and Gemini APIs.
* **Zero-Host Context Harvester**: Local protocols store user data locally with zero external hosting dependencies.
* **Privacy-First Grounding**: Utilizes native right-click selection context menus to securely ingest targeted, high-value webpage context.
* **Optional Search Grounding**: Tick-box functionality for Gemini Models only featuring a red warning disclaimer above the user input chat box when active.
* **Export Chat**: One-click professional Markdown (.md) for local chat history exports.
* **Volatile State Persistence**: Prevents active session data loss caused by native side-panel closure, browser restarts, or system shutdowns. Chat session backups automatically save to local storage hooks on loop termination.
* **Dynamic Model Configuration Engine**: Future-proofed against rapid upstream AI model changes. Restructures model dropdown arrays dynamically across frontend layouts and backend service workers simultaneously from a single config file.
* **Ephemeral Lifecycle Lifeline**: Solves Chrome's 30-second ephemeral service worker shutdown using an integrated background handshake pulse loop during long-running 40+ second LLM responses.
* **Context-Triggered Workspace Wakeup**: Automatically opens the side-panel, instantiates the script frame, injects text, and snaps the layout viewpoint when text is sent via the right-click menu.
* Unified Background Script **CORS-Bypass Pipeline framework** for OpenAI and Claude to guarantee direct, clean API handshakes.
* **100% modular JavaScript layout** with no heavy or bloated Node.js package dependencies.
* **Endpoints Verified**: Architecture is fully integrated and tested up to the API endpoints. Handshakes are verified operational for OpenAI, Claude, and Gemini (including search grounding), returning standard billing/quota responses when tested with free/empty keys.

---

## Why Buy This Project?
* **Production-Ready**: Skip the massive headache of debugging Manifest V3 background service workers, asynchronous loop timeouts, and cross-origin request policies.
* **Easy White-Labeling**: You can entirely rebrand this extension (appName, AI names, AI colors and AI models) globally just by editing a single config file.
* **Ready to Monetize**: Perfect foundation to launch as a paid extension, a private tool for your team, or a premium digital product.
