# Research Notes: What Is Working Right Now

This is a practical synthesis of public updates and successful open-source patterns.

## 1) Capability Direction

Recent Anthropic updates emphasize:
- stronger coding and long-context reasoning models,
- agent-building features in API workflows,
- better cost/latency controls for long-running tasks.

For builders, this means:
- ship agents that do multi-step work,
- keep context stable without exploding cost,
- connect tools using protocol-based integrations.

## 2) Why MCP Matters

MCP reduces one-off integrations by standardizing how tools are exposed to models.
Instead of writing custom glue for every SaaS, teams can reuse MCP server patterns.

Practical takeaway:
- choose 2-5 essential tool connections first,
- avoid enabling too many tools at once (context and reliability degrade),
- create narrow, task-specific toolkits per workflow.

## 3) Why Prompt Caching Matters

Prompt caching can drastically reduce repeated prompt cost and latency in agent loops.
Good use cases:
- repeated workflows with heavy instructions,
- long background context used across many runs,
- multi-step automations where the prefix is stable.

Bad use cases:
- one-off prompts with constantly changing context.

## 4) Why Public Repos Go Viral

Public utility repos that spread fastest usually have:
- immediate copy/paste value,
- clear use-case positioning,
- practical examples over abstract concepts,
- active maintenance and issue responses.

## 5) Build Strategy for This Repo

To maximize adoption:
1. Teach practical patterns quickly.
2. Give templates people can use in 10 minutes.
3. Include launch/checklist guidance, not just code.
4. Keep messaging professional and outcome-driven.

