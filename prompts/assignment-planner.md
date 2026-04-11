---
type: prompt
id: assignment-planner
title: Assignment Planner
description: "Task prompt for breaking down assignment briefs into work plans"
tags: [Production, Learning, Planning]
inputs:
  assignment_brief:
    label: "Assignment Brief"
    description: "The full assignment brief or instructions"
    example: "Write a 1500-word report analysing the causes of inflation in the UK economy"
    required: true
    type: text
  deadline:
    label: "Deadline"
    description: "When the work is due"
    example: "2026-05-20"
    required: true
    type: text
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
