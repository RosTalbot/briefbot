# 🤖 Vibe Agent 03: BriefBot

<p align="left">
  <img src="/screenshots/BriefBot-Persona.png" alt="BriefBot Persona" width="250" style="float: left; margin-right: 20px;" />
</p>

**Project Type:** Creative Brief Generator (n8n Form + GPT-powered Prompting)  
**Agent Role:** Chaos-wrangling strategist who turns messy ideas into structured briefs. Fluent in vibes, allergic to vagueness.

---

## 🧠 Purpose

BriefBot is an AI-powered creative intake agent designed to help content creators, marketers, and brand teams transform messy input into polished briefs. Whether you're launching a podcast, newsletter, or campaign, BriefBot clarifies your vision in minutes.

---

## 📌 Project Overview

Streamline the process of generating creative briefs by guiding users through structured questions, then converting their responses into clear, actionable briefs — ready for clients, collaborators, or AI reuse.

---

## 🛠️ Tools & Tech

| Layer     | Tool        |
|-----------|-------------|
| LLM       | GPT-4o       |
| Interface | n8n Form (front-end + automation engine) |
| Output    | Markdown / JSON |
| Assets    | Midjourney (persona artwork) |
| Optional  | Notion, Zapier, Google Docs |

---

## 🧠 Memory + Context Awareness

- Retains tone/style guidelines for each brief
- Reads and formats context from links, references, or vague input
- Adapts brief formatting based on idea clarity (dropdown selector from “napkin sketch” to “pretty clear”)
- Can optionally recall previous briefs (for consistency across campaigns)

---

## 💬 Form: "Lay It On Me"

This is the user entry point. It includes questions like:

- Who’s it for, and what do they care about?
- What kind of asset are we creating?
- Drop your brain dump
- Any tone/style guidelines?
- Got references or inspiration?
- How polished is your idea?
- Anything to avoid?

### Required Fields:
- Audience
- Content Type
- Brain Dump
- References

### Output:
- Clean creative brief
- Optional voice/tone paragraph
- Brand-safe voice tags
- GPT-ready reuse prompt

---

## ✅ Example Output

```markdown
**Project:** August Podcast Episode – "Systems > Hustle"

**Summary:**
We’re exploring how creative entrepreneurs can ditch grind culture and scale sustainably using smart systems. This episode will be part of our "Anti-Hustle Toolkit" series.

**Audience:**
Solo service providers (mostly women, 30s–40s) who are burned out from hustle culture and ready to work smarter.

**Tone + Style:**
Confident, warm, strategic. Avoid hype. Feel like a trusted advisor.

**Platform:**
Podcast + IG Reels + Email

**Prompt for reuse:**
"Create a podcast episode outline in a confident, warm tone for burned-out solo entrepreneurs. Emphasize strategic systems over hustle. Avoid jargon."
```

---

## 📸 Screenshots To Include
- "Lay It On Me" form UI
- Form submission confirmation view
- Backend n8n workflow (form → prompt → output)
- Before/after: raw input vs formatted brief
- GitHub repo banner/thumbnail

---

## 📂 Suggested Repo Structure
```
briefbot/
├── README.md
├── prompts/
│   └── base_prompt.txt
├── samples/
│   ├── input_example.md
│   └── output_brief.md
├── screenshots/
│   └── sample_ui.png
├── eval/
│   └── criteria.md
└── LICENSE
```

---

## 🔁 Future Enhancements
- Add agent-style voice to response: "Seen worse, give me a sec…"
- Store outputs in Notion or Airtable
- Let users choose voice/tone archetypes
- Add brief refinement step after draft is shown
- Export as Google Doc or PDF

---

## 👤 Creator
Built by [Ros Talbot](https://github.com/RosTalbot) as part of the AI Agent Bootcamp (2025).

---
