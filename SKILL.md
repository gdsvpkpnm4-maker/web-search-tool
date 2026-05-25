---
name: web-search
description: Search the web using DuckDuckGo for facts, current info, definitions, and quick answers on any topic.
---

# Web Search

## Instructions

Call the `run_js` tool ONCE using `index.html` and a JSON string for `data` with this field:

- **query**: Required. A short keyword phrase (3–6 words). Drop filler like "what is" or "tell me about". Keep names, dates, key terms.

After receiving the result, immediately respond to the user. Do NOT call the tool again.

The tool returns `{ "result": "..." }` on success or `{ "error": "..." }` on failure.

Result may include:
- `ANSWER:` — a direct factual answer
- `SUMMARY:` — an overview with source and link
- `DEFINITION:` — a dictionary-style definition
- `RELATED:` — related facts and topics
- `NEWS:` — recent news headlines with dates and links

Base your reply only on what the result contains. Stop after one search.
