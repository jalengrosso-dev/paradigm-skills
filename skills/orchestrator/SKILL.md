---
name: orchestrator
description: "The central brain of the Paradigm AI system. Activate when a task needs multiple agents, when routing is unclear, or when running a full capture workflow. The Orchestrator reads the request, identifies which agents are needed, sequences them in the right order, and synthesizes one unified output."
---

cd ~/paradigm-skills
{ head -4 skills/orchestrator/SKILL.md.backup; echo ""; pbpaste; } > skills/orchestrator/SKILL.md
wc -c skills/orchestrator/SKILL.md