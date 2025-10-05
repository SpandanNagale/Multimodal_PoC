# Multimodal AI Agent (Text → Image → Audio Caption)

### Overview
An end-to-end open-source multimodal AI system that takes a text prompt, generates an image, captions it, and converts the caption into speech — built using only open-source models and free infra.

### Workflow
Text → Image (Stable Diffusion) → Caption (BLIP) → Audio (Coqui TTS)

## Architecture Summary & Cost Optimization

- Modular LangGraph pipeline for flexible multimodal orchestration.
- Lightweight open-source models for image, caption, and audio generation.
- Designed for zero-cost execution using Google Colab free-tier GPU.
- Can be easily ported to LangChain or N8N for scalable workflow automation.


### Tools Used
- Diffusers (Stable Diffusion)
- HuggingFace Transformers (BLIP)
- Coqui TTS
- LangGraph (Agentic Orchestration)
- Colab (Free GPU)

### Output Example
Input Prompt: *"A futuristic city skyline at sunset with flying cars"*

Output:  
🖼️ Generated Image  
🗣️ Spoken Caption: “A futuristic city skyline with glowing buildings and flying cars.”

### Notes
- 100% Open Source (no paid APIs)
- Runs fully on Google Colab
- Built to demonstrate multimodal orchestration and resourceful design
