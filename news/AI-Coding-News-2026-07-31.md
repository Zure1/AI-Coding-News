# AI Coding News — 2026-07-31

**Date range covered:** 25. 07 → 31. 07  
**Signal level:** high-signal updates only.

## Key updates

This week was mostly about **multi-agent IDE workflows, customizable code review, enterprise controls, model choice, supply-chain protection, and agent oversight**.

| Area | What to know |
|---|---|
| IDE agents | VS Code and Visual Studio added stronger agent-session, review, worktree, skills, and parallel-work features. |
| Code review | Copilot code review can now use repository skills and read-only external context in production. |
| Models | Grok 4.5 entered Copilot with a 500K-token context window and parallel tool use. |
| JetBrains | Copilot added OpenTelemetry export, token limits, model controls, custom agents, and stronger CLI sessions. |
| Enterprise governance | GitHub separated Copilot app access from CLI access and extended managed settings to the app and cloud agent. |
| CI security | GitHub Actions now pauses workflow runs identified as potentially malicious before execution. |
| Agent reliability | New research found that coding agents rarely discover repository AI rules and can reduce code understanding. |
| Enterprise adoption | Disney is dropping Copilot, Kiro, and Amazon Q in the US while adding Codex and retaining Claude and Cursor. |

---

## 1. VS Code expands multi-agent and parallel coding workflows

**What changed**

GitHub’s July VS Code releases added a redesigned Agents window with faster diff review, session grouping, subagent visibility, and direct handling of failed CI checks and review comments.

Copilot, Claude, and Codex sessions can now run in isolated Git worktrees. Claude sessions support multiple related chats and peer-chat forks, and BYOK models can now be used with the Copilot agent in the Agents window.

**Source link**

- https://github.blog/changelog/2026-07-30-github-copilot-in-visual-studio-code-july-2026-releases/

---

## 2. Copilot code review skills and external context are generally available

**What changed**

GitHub made agent skills and MCP context generally available in Copilot code review for Copilot Pro, Pro+, Business, and Enterprise users.

Teams can add repository-specific review instructions and internal tools through `.github/skills/*/SKILL.md`. Code review can also read context from configured issue trackers, documentation systems, and service catalogs. MCP tool calls are read-only, and comments now show when skills or MCP context influenced the review.

**Source link**

- https://github.blog/changelog/2026-07-29-copilot-code-review-agent-skills-and-mcp-now-generally-available/

---

## 3. Visual Studio adds a new agent, built-in skills, and selected-code review

**What changed**

Visual Studio 2026 added a public-preview agent built on the Copilot SDK used by Copilot CLI. GitHub says it completes more tasks with less back-and-forth and produces shorter responses.

The IDE also added built-in .NET and Azure skills, inline Copilot review for selected code, and organization-level custom instructions for Business and Enterprise plans.

**Source link**

- https://github.blog/changelog/2026-07-30-github-copilot-in-visual-studio-july-update/

---

## 4. Grok 4.5 arrives in GitHub Copilot

**What changed**

GitHub started rolling out xAI’s Grok 4.5 reasoning model across VS Code, Visual Studio, Copilot CLI, Copilot cloud agent, the Copilot app, JetBrains, Xcode, and Eclipse.

The model supports up to 500,000 input tokens, text and image input, configurable reasoning effort, parallel tool dispatch, and multi-step agentic coding. GitHub positions it for terminal-heavy work, exploration, complex task execution, and fast coding loops. Usage is billed at provider list pricing.

**Source link**

- https://github.blog/changelog/2026-07-28-grok-4-5-is-now-available-in-github-copilot/

---

## 5. Copilot for JetBrains adds observability and model controls

**What changed**

GitHub Copilot for JetBrains now supports OpenTelemetry export for agent workflows, configurable input and output token limits for BYOK and custom endpoints, and controls for enabling or disabling built-in models.

Claude agent flows can use MCP servers and custom agents. Copilot CLI sessions inside JetBrains also gained session forks, a `/rubber-duck` command, visible task lists, improved MCP diagnostics, and better session recording.

**Source link**

- https://github.blog/changelog/2026-07-27-github-copilot-for-jetbrains-adds-improvved-opentelemetry-configuration-and-model-management/

---

## 6. GitHub expands enterprise governance for agent clients

**What changed**

GitHub separated Copilot app access from Copilot CLI access, allowing enterprise and organization administrators to enable or disable each client independently.

The Copilot app and Copilot cloud agent now also enforce enterprise `managed-settings.json` policies. These settings can control approved plugins and marketplaces, command and file-access approval bypasses, and default model selection across supported Copilot clients.

**Source links**

- https://github.blog/changelog/2026-07-27-manage-github-copilot-app-access-with-a-dedicated-policy/
- https://github.blog/changelog/2026-07-27-enterprise-managed-settings-now-apply-to-the-github-copilot-app/

---

## 7. GitHub Actions pauses potentially malicious workflow runs

**What changed**

GitHub Actions now automatically holds selected workflow runs in public repositories when they appear potentially malicious.

The workflow does not execute until a repository collaborator with write access reviews and approves it through an authenticated web session. GitHub introduced the protection after attacks used compromised accounts to add workflows that stole CI/CD credentials.

**Source link**

- https://github.blog/changelog/2026-07-28-github-actions-holds-potentially-malicious-workflows-for-approval/

---

## 8. Coding agents rarely discover repository AI contribution rules

**What changed**

RepoComplianceBench evaluated four frontier models on 106 tasks from 49 open-source repositories with rules covering AI bans, disclosure, verification, and human handoff.

Agents proactively opened relevant policy files in only 3.5% of runs. Refusal and human-handoff compliance were 0% without intervention across all tested agents. Explicit reminders, quoted rules, and verifier feedback improved disclosure and test-verification behavior, but did not reliably enforce bans or human escalation.

**Source link**

- https://arxiv.org/abs/2607.26819

---

## 9. Agent-assisted coding improved completion but reduced code understanding

**What changed**

A controlled study of 54 participants compared an editing agent with a chatbot-based coding workflow. Agent users completed the initial task more effectively, but showed weaker understanding of their code and were less prepared to extend it without the agent.

Copy-and-paste prompts and automatically accepted edits were associated with lower comprehension, even though participants preferred the faster agent workflow.

**Source link**

- https://arxiv.org/abs/2607.26375

---

## 10. Disney changes its enterprise AI coding tool mix

**What changed**

Business Insider reported that Disney plans to stop using GitHub Copilot, Amazon Kiro, and Amazon Q for US staff in August. Disney is preparing to add OpenAI Codex while retaining Claude Enterprise and Cursor.

The report says several employees rarely used Copilot or found its output required cleanup, while Claude and Cursor had stronger internal usage. The change does not apply internationally.

**Source link**

- https://www.businessinsider.com/disney-microsoft-github-copilot-openai-codex-ai-tools-claude-cursor-2026-7
