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
## 🛠️ Tool Card: `CreativeBriefGenerator`

**Purpose:**  
Transforms messy creative input into a structured, professional brief — ready for use by content teams, strategists, or other AI agents. Streamlines early-stage project scoping and standardizes creative intake across teams.

---

**Required Inputs:**

| Field              | Description                                                 |
|-------------------|-------------------------------------------------------------|
| `project_name`     | Title or label for the project (optional)                   |
| `audience_description` | Who the content is for and what they care about        |
| `asset_type`       | Format or deliverable type (e.g., podcast, landing page)    |
| `idea_dump`        | Raw notes, ideas, goals, or brainstorm text                 |
| `references`       | Optional links, examples, or inspiration                    |
| `chaos_level`      | Self-rated input clarity ("napkin sketch" to "pretty clear")|
| `tone_guidance`    | Desired tone, voice, or stylistic instructions              |
| `avoid_notes`      | Words, phrases, or directions to avoid                      |

---

**Expected Outputs:**

| Field              | Description                                                 |
|-------------------|-------------------------------------------------------------|
| `brief_title`      | A clean, human-readable title                               |
| `summary`          | A paragraph summarizing the idea                            |
| `audience_goals`   | Key insights about the target audience                      |
| `tone_style_tags`  | A few descriptive tags for tone and voice                   |
| `platforms`        | Suggested content channels (if inferable)                   |
| `GPT_prompt`       | Reusable prompt for future generation                       |
| `raw_markdown`     | Optional Markdown version of the brief                      |

---

**Business Value:**

- Saves 1–2 hours per creative request by automating the brief creation process  
- Reduces misalignment between stakeholders and creative teams  
- Ensures consistency in tone, goals, and brand across content  
- Enables async collaboration with clear, structured briefs  

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
