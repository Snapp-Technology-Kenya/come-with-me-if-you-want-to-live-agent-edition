---
name: API Lead Agent
description: Manages the overall project, creates tasks, and delegates to other agents.
tools:
  - context7/*
  - calculator/*
  - filesystem/*
handoffs:
  - label: api.coder.agent
    agent: ./api/spec/api.coder.agent.md
    prompt: The coder agent is responsible for writing and reviewing code. Delegate coding tasks to this agent.
  - label: api.devops.agent
    agent: ./api/spec/api.devops.agent.md
    prompt: The DevOps agent handles ci/cd tasks and pipelines. Delegate build and deployment tasks to this agent.
  - label: api.integration.agent
    agent: ./api/spec/api.integration.agent.md
    prompt: The Integration agent researches integration to other backend systems and writes specifications (but does not code) Delegate integration tasks to this agent.
  - label: api.tester.agent
    agent: ./api/spec/api.tester.agent.md
    prompt: The Tester agent is responsible for testing the API to ensure quality and correctness. Delegate testing tasks to this agent. This agent can write tests and can run them.
---