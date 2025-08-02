# 🤖 Vibe Agent 03: BriefBot

**BriefBot** is an AI-powered assistant that transforms messy creative input into structured, professional briefs — perfect for content creators, marketers, and async teams.

Whether you're planning a podcast, writing a newsletter, or launching a campaign, BriefBot helps clarify your vision in minutes.

---

## 🧠 Purpose

Streamline the process of generating creative briefs by guiding users through a few simple questions, then converting the answers into a polished brief — ready for clients, collaborators, or AI agents.

---

## 🛠️ How It Works

**Input:**  
User answers 4–6 short questions:
- What’s the project or content about?
- Who’s it for?
- What’s the desired tone or vibe?
- What’s the main message or goal?

**Output:**  
A clean, structured creative brief:
- Title + Summary
- Audience & Goals
- Tone + Style tags
- Platform + Format
- Optional GPT-ready prompt for future reuse

---

## 🔌 Tools & Tech

| Layer     | Tool        |
|-----------|-------------|
| LLM       | GPT-4       |
| Interface | Replit Form or n8n (optional UI) |
| Output    | Markdown / JSON |
| Optional  | Zapier, Notion, Docs export |

---

## 🧠 Context Awareness

- Auto-adapts format based on project type (e.g. podcast vs. newsletter)
- Detects vague input and asks for clarification
- Uses embedded tone classifiers to recommend matching brand voice prompts

---

## 🧠 Memory (Optional Extension)

If using in a multi-session environment (e.g., Notion or a local workspace):
- BriefBot can recall previously written briefs to ensure consistency
- Can compare new input to past briefs to highlight shifts in tone or audience

---

## 💡 Example Output

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

## 🚀 Status: MVP v1

- Current version is a prompt-based prototype. 
- Next step: Replit or Streamlit form for structured inputs
- Optional: Add JSON/Markdown export button

---

## 📸 Recommended Screenshots for Repo

- Input form (Replit or mockup)
- Raw user input → Polished brief comparison
- Before/after sample for tone shifts
- Prompt + Output pairing

---

## 📂 Repo Structure (Suggestion)

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

## 👤 Creator
Built by [Ros Talbot](https://github.com/RosTalbot) as part of the AI Agent Bootcamp (2025).

---
