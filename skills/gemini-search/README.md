# Gemini Search Skill

A specialized AI Edge Gallery skill providing live web search, source-backed answers, and Gemini grounding for current factual questions.

## Overview
This skill transforms the local LLM into a search assistant for questions that need current information, live web lookup, or source-backed answers. It preserves the user's original question as closely as possible, sends it to Gemini with Google Search grounding, and returns a concise response with sources when available.

## Installation

### Quick Install (Android)
1. Open the **Google AI Edge Gallery** app.
2. Select the **Agent Skills** option from the main menu.
3. Select the **Gemma-4-E2B-it** model by pressing the **Try it** button and wait for everything to load.
4. Press the **Skills Icon** at the bottom of the GUI.
5. Press the **Plus (+)** icon and select **Load skill from URL**.
6. Enter the following URL:  
   `https://raw.githubusercontent.com/StrinGhost/gemma-skills/main/skills/gemini-search/SKILL.md`
7. Select **Add**.

### Quick Install (iPhone / iOS)
1. Open the [SKILL.md URL](https://raw.githubusercontent.com/StrinGhost/gemma-skills/main/skills/gemini-search/SKILL.md) in Safari.
2. Tap the **Share** icon and select **Save to Files**. Save it to your **Downloads** folder.
3. Open the **Google AI Edge Gallery** app.
4. Select the **Gemma-4-E2B-it** model and press **Try it**.
5. Press the **Skills Icon** at the bottom of the GUI.
6. Press the **Plus (+)** icon and select **Load skill from Local**.
7. Navigate to your **Downloads** folder and select the `SKILL.md` file you just saved.

### Manual Install
1. Create a folder named `gemini-search` in your local AI Edge Gallery skills directory.
2. Save the `SKILL.md` and `README.md` files into that folder.
3. Open the **Google AI Edge Gallery** app.
4. Navigate to **Agent Skills** and tap the **Refresh** icon to activate.

## Usage
Trigger this skill by asking for current or source-backed information, such as:
- "Did OpenAI just raise a new funding round?"
- "Is the Nintendo Switch 2 available in Singapore yet?"
- "What's the latest on the tax filing deadline?"
- "Can you check whether Italy will qualify for the next World Cup?"

## Input Format
The skill expects a JSON payload with one field:

```json
{
  "query": "Did OpenAI just raise a new funding round?"
}
```

## Output Format
The skill returns:
- A concise answer grounded in Google Search
- Source links when grounding data is available
- An error message if the API key is missing or the request fails

## Important Notice
This skill requires a valid Gemini API key and is intended for live search and factual questions only. Keep the query as close as possible to the user's original wording, and double-check any critical information with the original sources before taking action.

---

Copyright 2026
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
[http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)
