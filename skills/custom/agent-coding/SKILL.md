---
name: agent-coding
description: Use when designing or implementing tool-using agents for research or software workflows and you need an explicit architecture, tool contract, prompt strategy, and evaluation plan.
---

# Purpose

Build agent systems as engineering artifacts rather than vague autonomous demos.

# When To Use

- designing coding agents, research agents, or tool-using assistants
- defining prompts, state, memory, and tool interfaces
- integrating agents into an existing repository or workflow
- evaluating agent reliability, failure modes, and recovery logic

# Inputs

- target workflow or user job to automate
- available tools, APIs, files, or repo context
- product constraints such as latency, cost, privacy, and reliability

# Outputs

- agent architecture and control loop
- tool contract and state model
- prompt strategy and decision policy
- evaluation cases and failure taxonomy
- implementation plan with milestones

# Workflow

1. Define the task boundary before choosing the agent pattern.
2. Specify observation, memory, action, and recovery paths.
3. Design tool interfaces that are explicit and testable.
4. Add evaluation cases for success, refusal, and recovery behavior.
5. Keep the first implementation narrow and measurable.

# Constraints

- avoid agent designs that hide state transitions
- prefer explicit tool contracts over free-form improvisation
- separate capability demos from production-ready workflows
- define failure handling before scaling complexity