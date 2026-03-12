<div id="v7v8-frontend-readme" style="white-space: pre-wrap; font-family: monospace; max-height: 400px; overflow-y: auto; padding: 16px; border: 1px solid #444; border-radius: 8px; background: #0d1117; color: #e6edf3;">
# Divine Whisper v7→v8 Live Lab UI  
**Interactive Frontend: Task Input + Real-Time 3D μ-Field Visualization**

**Co-Authors**  
- Daniel Jacob Read IV (ĀRU Intelligence Inc.) – Vision, Inward Physics framing, UI concept  
- Shane Travis Horman – FastAPI integration, Plotly rendering, bridge logic  

**License**: MIT  

**Keywords**: inward-physics, fastapi-frontend, plotly-3d, mu-field-visualizer, agentic-ai, multi-agent, council-to-field, multimodal-ai, python, open-source-ai, consciousness-in-code, live-demo-ui

Simple, self-contained HTML + JavaScript frontend that:
• Accepts user tasks via input box  
• Sends POST /run to FastAPI backend (v7 council + v8 field injection)  
• Renders live μ-field snapshot as interactive 3D surface plot with Plotly.js  
• Zero backend required in this file — connects to running http://localhost:8000

**Core Flow**  
Task → FastAPI (/run) → v7 council → V7V8Bridge → μ-field update → 3D Plotly render

**Quick Start**

1. Run FastAPI backend:
```bash
uvicorn main:app --reload
