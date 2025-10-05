# Multimodal AI Agent: Text → Image → Audio Caption

## 🚀 Impact Statement  
Demonstrates a **zero-cost**, open-source multimodal pipeline that ingests text, generates an image, captions it, and produces narration — all orchestrated agentically. This prototype is designed as a minimal yet powerful building block for client-facing applications in marketing, accessibility, and content automation.

## ✍️ Architecture & Workflow  
1. **LangGraph (Agent Controller)** — directs which model to call next  
2. **Stable Diffusion** — converts prompt → image  
3. **BLIP** — captions the generated image  
4. **Coqui TTS** — converts caption → audio narration  


## 🔧 Tooling & Design Rationale  
- 100% open-source (no paid APIs)  
- Optimized to run on free GPU tiers (Colab, Kaggle)  
- Modular nodes: You can swap the captioning or TTS model easily  
- Mappable to alternative orchestration frameworks like **LangChain** or **N8N** by converting each node into a chain or workflow block

## 🧩 Limitations & Extensions  
- Current demo handles single-prompt → single-output; doesn’t support iterative refinement  
- If image generation fails (complex prompt), fallback to a simpler diffusion prompt  
- **Future upgrades**: integrate LLaVA-1.6 or Mistral vision modules, multilingual TTS (Bark / XTTS), integrate memory or feedback loop in LangChain

## 🧾 Clone & Run  
```bash
git clone ...
cd Multimodal_PoC
# Open the notebook in Colab
