# PowerPoint Customizer Prototype

This prototype demonstrates automating PowerPoint text customization using OpenRouter's generative AI.
It exposes a small FastAPI server and a minimal React front‑end.

## Features

- Upload a PowerPoint template (`.pptx`)
- Provide contextual text for the AI
- Preview AI‑generated slide text before downloading
- Download the customized presentation

## Requirements

- Python 3.10+
- Node.js (for the optional front‑end)
- An OpenRouter API key

Install Python dependencies:

```bash
pip install -r requirements.txt
```

Start the server:

```bash
export OPEN_ROUTER_API_KEY=your_key_here
uvicorn server:app --reload
```

Then open `frontend/index.html` in a browser.

## Notes

This is a very small prototype and only customizes slide text. It does not yet store templates or maintain history. The AI requests are synchronous and may be slow on large presentations.
