---
type: workflow
id: assignment-planning-flow
title: Assignment Planning Flow
description: "Brief analysis, work plan, and milestone tracking"
tags: [Draft]
connections:
  - target: study-planning
    type: uses
  - target: plan-studies
    type: uses
  - target: assignment-planner
    type: uses
---

## Overview

This workflow helps students break down assignment briefs into manageable work plans with clear milestones and deadlines.

## Pipeline Stages

### Stage 1: Brief Analysis

Invoke the **study-planning** skill to analyse the assignment brief, identify key requirements, and understand the marking criteria.

### Stage 2: Work Plan Creation

Invoke the **assignment-planner** prompt to break the assignment into a step-by-step work plan with time estimates.

### Stage 3: Schedule Integration

Invoke the **plan-studies** prompt to integrate the assignment work plan into the student's existing study schedule.

## Output

Assignment plan containing:

- Brief analysis with key requirements highlighted
- Step-by-step work plan with time estimates
- Milestone dates working back from the deadline
- Integration with existing study schedule
