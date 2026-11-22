# AGENT_WORKFLOW.md

## User goal
[One clear outcome]

## Agent workflow
| Step | User input | Agent action | Tool / data source | Permission | Failure fallback |
| --- | --- | --- | --- | --- | --- |
| 1 | [Request] | [Clarify] | None | None | Ask a question |
| 2 | [Details] | [Retrieve] | [API] | Read-only | Show unavailable status |
| 3 | [Review] | [Recommend] | [Model] | None | Explain uncertainty |
| 4 | [Confirm] | [External action] | [Tool] | Explicit approval | Human handoff |

## Action boundaries
- Never claim to have placed an order, called someone or completed a payment unless a real integration confirms it.
- Ask before external actions and show what will happen.
- Label simulated data and estimated prices.
- Do not expose private information in logs or prompts.

## Voice-specific checks
- Tamil + English switching
- Noisy background and interruption handling
- Recognition errors and repeat-back
- Latency, call cost and consent
- Text or human fallback
