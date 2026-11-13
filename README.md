# Practical AI Agent Architecture Patterns

An interactive cheat sheet for understanding practical AI agent architectures through animated diagrams, customer-support examples, and quality checkpoints.

**Created by [Yogesh Deshmukh](https://www.linkedin.com/in/ypdeshmukh/)**  
*Connecting Quality Engineering with Agentic AI*

## Explore the guide

**[Open the interactive cheat sheet →](https://yogeshdeshmukh86.github.io/-ai-architecture-cheatsheet/)**

Select a pattern to explore its control flow, when to use it, a short line to remember it, and an illustrative example.

## Patterns covered

| Pattern | Main idea |
| --- | --- |
| Single agent | One agent, one reasoning role; it may handle multiple related tasks and use tools. |
| Tool-using agent | The agent decides when to call tools or APIs. |
| Workflow + agent | The workflow sets the sequence; an agent reasons within a step. |
| Router | Classify a request, then send it down the appropriate path. |
| Evaluator | Draft, check against criteria, then revise, escalate or deliver. |
| Supervisor–worker | Delegate to specialist reasoning roles and synthesise their results. |

These are practical teaching examples. Patterns can overlap, and the number of agents depends on the implementation.

## What you can learn

- **Follow the flow:** animated arrows show control, tool calls, and result or review feedback.
- **Compare the same request:** each pattern handles an illustrative customer-support enquiry about a late order.
- **Understand the harness:** the **“Where does the harness fit?”** toggle highlights the surrounding system and explains its role in the selected pattern.
- **Explore the components:** select a diagram box to see its role, input and output.
- **Think about quality:** each pattern includes quality checkpoints and suggested AI evals, with expandable evaluation guidance.

## What is an agent harness?

The harness is the software around the model that supplies context and tools, manages state and control flow, and enforces checks.

The guide illustrates instructions and context, tools and data access, memory and state, routing and orchestration, permissions and guardrails, and evaluation and traces.

**Count reasoning roles, not boxes.** A single agent can use tools or sit inside a workflow. A model call is not automatically an agent, and a tool can expose another agent. Count the independently acting agents in the actual implementation. The harness is not an extra agent.

## Use locally

1. Download this repository.
2. Open `index.html` in a modern browser.
3. Select a pattern and try the harness toggle.

No build step is required. An internet connection allows the page's externally hosted helper scripts to load.

The examples illustrate architecture decisions; they do not connect to a live order system or run AI models.

## Project structure

```text
index.html   Website, diagrams, styling, examples, and interactions
README.md    Project overview and usage
```

The interactive content runs inside a sandboxed iframe. The page includes Content Security Policy declarations and supports reduced-motion preferences for its flow animations.

## Hosting

Published with **GitHub Pages** from the `main` branch and repository root. Changes to `index.html` are published through the repository's Pages build and deployment.

## Further reading

- [Building effective agents — Anthropic](https://www.anthropic.com/research/building-effective-agents)
- [Harness definition in evaluation guidance — OpenAI](https://openai.com/index/trustworthy-third-party-evaluations-foundations/)
- [Agents as tools — OpenAI Agents SDK](https://openai.github.io/openai-agents-python/tools/)
- [Demystifying evals for AI agents — Anthropic](https://www.anthropic.com/research/demystifying-evals-for-ai-agents)

## Connect

[Connect with Yogesh on LinkedIn](https://www.linkedin.com/in/ypdeshmukh/)
