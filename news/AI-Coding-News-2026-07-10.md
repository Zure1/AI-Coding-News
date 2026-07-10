# AI Coding News — July 10, 2026

**Date range:** 2026-07-04 → 2026-07-10

## Key updates

This week was mostly about **new coding models, broader IDE agent choice, and stronger enterprise control of agent workflows**.

### GPT-5.6 launches with three coding-focused tiers

- **What changed:** OpenAI released GPT-5.6 across Codex and the API in three tiers: Sol for the hardest long-running codebase and agent tasks, Terra as the balanced option, and Luna for faster, lower-cost work. The models add programmatic tool calling, beta multi-agent execution, up to 1M-token long-context evaluation, and new `max` and `ultra` effort modes. OpenAI reports 88.8% on Terminal-Bench 2.1 for Sol and 72.7% on DeepSWE v1.1. API pricing is $5/$30 per million input/output tokens for Sol, $2.50/$15 for Terra, and $1/$6 for Luna.
- **Source:** [OpenAI — GPT-5.6](https://openai.com/index/gpt-5-6/)

### GPT-5.6 reaches GitHub Copilot

- **What changed:** GitHub began rolling out GPT-5.6 Sol, Terra, and Luna to Copilot. Sol targets complex reasoning over large codebases and long-running agents; Terra targets everyday interactive and agentic coding; Luna targets smaller, faster tasks. The models are available across VS Code, Visual Studio, Copilot CLI, the cloud agent, JetBrains, Xcode, Eclipse, github.com, and GitHub Mobile. Business and Enterprise administrators must explicitly enable them.
- **Source:** [GitHub Changelog — GPT-5.6 in Copilot](https://github.blog/changelog/2026-07-09-openais-gpt-5-6-sol-terra-and-luna-are-now-available-in-github-copilot/)

### JetBrains Copilot adds Codex as an agent provider

- **What changed:** GitHub Copilot for JetBrains IDEs added Codex as a public-preview agent provider. The same update added Hooks in the Customizations editor, richer server management, administrator-configured custom models, Copilot CLI approval settings, Claude permission modes and debug logs, and generally available Inline Chat.
- **Source:** [GitHub Changelog — Codex and agent enhancements in JetBrains](https://github.blog/changelog/2026-07-07-codex-as-agent-provider-and-agentic-enhancements-in-jetbrains-ides/)

### VS Code 1.128 expands parallel agent work

- **What changed:** VS Code 1.128 added multiple related chats inside one Claude agent session, enabling parallel approaches without splitting work across unrelated sessions. It also made image and PDF attachments in Copilot Chat generally available and added quick chats that can start from the Agents window without first opening a workspace.
- **Source:** [Visual Studio Code 1.128 release notes](https://code.visualstudio.com/updates/v1_128)

### Copilot gains device-enforced settings and managed telemetry

- **What changed:** GitHub made device-level managed settings generally available for Copilot CLI and VS Code through MDM or a root-owned configuration file. Administrators can enforce permission, model, plugin, marketplace, and telemetry settings regardless of the signed-in account. A separate update lets enterprises mandate an OpenTelemetry collector and control whether prompts, responses, and tool content are exported; collector credentials are kept out of agent tool subprocesses.
- **Sources:** [Managed settings via MDM](https://github.blog/changelog/2026-07-08-deploy-managed-copilot-settings-via-mdm-in-vs-code-and-cli/) · [Enterprise-managed OpenTelemetry export](https://github.blog/changelog/2026-07-08-enterprise-managed-opentelemetry-export-for-vs-code-and-cli/)

### Copilot adds repository onboarding summaries

- **What changed:** On github.com, Copilot can now generate a high-level overview of an unfamiliar repository, including its purpose, technologies, and contribution guidance. It can also create an overview when the repository has no README. The feature is available on all Copilot plans.
- **Source:** [GitHub Changelog — repository overview](https://github.blog/changelog/2026-07-09-ask-copilot-for-a-repository-overview/)

### Alberta publishes a large-scale security-agent case study

- **What changed:** Anthropic published a Government of Alberta case study covering roughly 50 parallel Claude Code agents reviewing 466 million lines across about 3,400 repositories in 20 hours. The workflow combined a rules engine with agent verification, exact file-and-line citations, human review before shipping, generated tests before patches when coverage was missing, and continuing red-team and blue-team agents checking applications against about 95 security controls.
- **Source:** [Anthropic — Government of Alberta case study](https://www.anthropic.com/news/alberta-government-claude-cybersecurity)
