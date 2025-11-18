---
name: UI Lead Agent
description: Manages the overall project, creates tasks, and delegates to other agents.
tools:
  - context7/*
  - calculator/*
  - filesystem/*
handoffs:
  - label: ui-architect-agent
    agent: ./ui/ui.architect.agent.md
    prompt: The UI Architect Agent is responsible for designing the UI architecture. Delegate UI architecture-related tasks to this agent.
  - label: ui-lead-agent
    agent: ./ui/ui.lead.agent.md
    prompt: The UI Lead Agent is responsible for leading the development of the UI. Delegate UI-related tasks to this agent.
  - label: test-lead-agent
    agent: ./test/test.lead.agent.md
    prompt: The Test Lead Agent is responsible for leading the development of the testing framework. Delegate testing-related tasks to this agent.
---