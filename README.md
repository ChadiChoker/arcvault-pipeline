# ArcVault AI-Powered Intake & Triage Pipeline

## Valsoft AI Engineer Technical Assessment

### Tools Used
- **n8n** (self-hosted) — workflow orchestration
- **Groq** (Llama 3.3 70B) — LLM classification & enrichment
- **Webhook.site** — output destination

### Files
- `n8n_workflow.json` — importable n8n workflow (change API key before running)
- `processed_requests.json` — structured output for all 5 sample requests
- `Architecture_WriteUp_and_Prompt_Documentation.docx` — system design, prompts, and rationale

### How to Run
1. Install n8n: `npm install -g n8n && n8n start`
2. Import `n8n_workflow.json` into n8n
3. Add your Groq API key in the Classification and Enrichment nodes
4. Add your Webhook.site URL in the output nodes
5. Send POST requests to the webhook endpoint
