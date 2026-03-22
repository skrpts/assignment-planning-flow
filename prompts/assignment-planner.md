---
type: prompt
id: assignment-planner
title: Assignment Planner
description: "Task prompt for breaking down assignment briefs into work plans"
tags: [Production]
connections:
  - target: study-planning
    type: derived_from
---

## Purpose

Breaks down an assignment brief into a structured, step-by-step work plan with realistic time estimates.

## Prompt

**Assignment brief:** {{input.assignment_brief}}
**Deadline:** {{input.deadline}}

Break down the above assignment brief into a step-by-step work plan. For each step, provide: 1) A clear task description. 2) Estimated time required. 3) Dependencies on other steps. 4) Resources or materials needed. 5) A suggested milestone date working back from the deadline. Include steps for research, planning, drafting, revision, and final formatting.
