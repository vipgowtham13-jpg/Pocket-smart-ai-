# Phase 3: Project Design

## System Architecture
- **Client Tier:** Dynamic HTML5/CSS3 templates served via Jinja2.
- **Server Tier:** Asynchronous FastAPI backend running on Uvicorn.
- **AI Processing Tier:** Google Generative AI API (Gemini 1.5 Flash) for multimodal parsing.
- **Infrastructure:** Containerized web service running on Render cloud.

## Data Flow
1. User uploads a receipt image via the web client.
2. FastAPI processes the payload and forwards the image to the Gemini multimodal endpoint.
3. Gemini extracts itemized details and spending insights.
4. Jinja2 renders and returns the structured results view to the user.
5. 
