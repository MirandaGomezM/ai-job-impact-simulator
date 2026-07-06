# AI Job Impact Simulator

Final project — AI & Innovation Program (Microsoft & Founderz)
**Student:** Miranda Gomez

## What is this?

A working web prototype that analyzes a person's job title, sector, and day-to-day tasks, and returns a personalized, task-by-task breakdown of how exposed that job is to AI-driven automation — on what timeline, and what to do about it.

Instead of generic headlines like *"40% of jobs will be automated,"* this tool gives an individualized, evidence-based estimate for the person's actual role, powered by Claude (Anthropic).

## Features

- 📋 Simple input form: job title, sector, years of experience, and main daily tasks
- 🌅 **Automation horizon** — a visual timeline plotting each task by risk level (high / medium / low) and timeframe (happening now / 2–5 years / 5+ years)
- 🛠️ Personalized list of skills worth developing
- ✅ A concrete action plan for the current week
- 👍 In-app feedback mechanism to validate whether each analysis felt useful
- ⚖️ Responsible AI disclaimers built into the interface (educational estimate, not a certain prediction or professional career advice)

## How it works

The frontend (React, single HTML file) sends the user's job description to Claude via the Anthropic API, using a structured system prompt that requests a strict JSON response (summary, tasks with risk/timeframe/reasoning, skills, action plan). The interface then renders that structured data as an interactive automation horizon.

## Try it

Open `simulador-impacto-ia.html` directly in an environment that supports calling the Anthropic API from the browser (e.g. as a Claude.ai artifact). It won't work by simply double-clicking the file locally, since the API call needs that environment.

## Responsible AI

This tool is explicitly designed to avoid both alarmism and false reassurance. It is framed as a starting point for reflection, not a verdict on anyone's career — and it says so, twice, inside the interface itself.

## Project deliverables

- `simulador-impacto-ia.html` — functional MVP (this repo)
- Final report (PDF/Word) — problem statement, solution description, validation & feedback, responsible AI considerations, key learnings
