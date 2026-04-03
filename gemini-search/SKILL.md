---
name: gemini-search
description: "Search the web using Gemini AI with Google Search grounding. Returns a summarized, up-to-date answer with cited sources. Ask anything — news, facts, research, current events."
type: javascript
require-secret: GEMINI_API_KEY
---

## Setup

You need a free Gemini API key:
1. Go to https://aistudio.google.com/apikey
2. Click "Create API key"
3. In AI Edge Gallery → Settings → Secrets → add key named `GEMINI_API_KEY`

## Usage

Enter any search query. Gemini will search the web in real time and return a summarized answer with sources.

The result is returned to the Gemma model for further use.
