---
name: query-grokipedia
description: Query a topic summary from Grokipedia, an AI-powered open encyclopedia.
---

# Query Grokipedia

## Instructions

Call the `run_js` tool using `index.html` and a JSON string for `data` with the following fields:
- **topic**: Required. Extract ONLY the primary entity, person, or event (e.g., "Black holes", "Ada Lovelace"). Remove all question words, action verbs, and conversational text (e.g., do NOT include "who invented", "history of", "what is").
- **lang**: Always use "en" - Grokipedia is English-only.

**Constraints:**
- Provide a concise summary (1-3 complete sentences) based on the returned snippet.
- Always include the Grokipedia article link so the user can read the full entry.
- If the exact answer to the user's question is not in the snippet, briefly state this, then offer what was found.
- If no result is found, say so and suggest rephrasing the topic.
