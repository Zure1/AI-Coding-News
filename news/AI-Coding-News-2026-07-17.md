# AI Coding News — July 17, 2026

**Date range:** 2026-07-11 → 2026-07-17

## Key updates

This week was mostly about **agents gaining direct access to IDE intelligence, AI security checks moving into active code review, and more flexible model and provider setups**.

### JetBrains 2026.2 connects coding agents to deeper IDE context

- **What changed:** JetBrains’ 2026.2 release wave moved agent support closer to the IDE’s own analysis and runtime data. IntelliJ IDEA and WebStorm added native GitHub Copilot integration and reusable agent skills, with IntelliJ also adding AI completion support for third-party providers. CLion introduced a debugger skill that lets ACP-compatible agents use stack traces, breakpoints, and variable values through GDB, LLDB, and DAP debuggers. The Rider 2026.2 release candidate added skills that expose coverage, profiler, and code-analysis data to agents, plus support for official Microsoft .NET, Aspire, and Azure skills and native Copilot integration.
- **Sources:** [IntelliJ IDEA 2026.2](https://blog.jetbrains.com/idea/2026/07/intellij-idea-2026-2/) · [WebStorm 2026.2](https://blog.jetbrains.com/webstorm/2026/07/webstorm-2026-2/) · [CLion 2026.2](https://blog.jetbrains.com/clion/2026/07/2026-2-release/) · [Rider 2026.2 RC](https://blog.jetbrains.com/dotnet/2026/07/15/rider-2026-2-release-candidate-is-out/)

### GitHub Copilot for JetBrains expands custom and local agent setups

- **What changed:** Copilot for JetBrains IDEs added bring-your-own-key support for OpenAI-compatible custom endpoints. The update also added Claude agent customizations for agents, skills, and instructions; local sandbox configuration; marketplace and source-repository plugin management; and a public-preview debugger skill for Copilot CLI sessions. GitHub also improved provider switching, authentication recovery, session persistence, and long-running session reliability.
- **Source:** [GitHub Changelog — Copilot for JetBrains BYOK and agent updates](https://github.blog/changelog/2026-07-14-github-copilot-for-jetbrains-expands-byok-capabilities/)

### The GitHub Copilot app adds on-demand security reviews

- **What changed:** The Copilot desktop app added the `/security-review` command in public preview. It scans current workstream changes for high-confidence findings, scores severity and confidence, and returns fix suggestions that can be applied and checked without leaving the app. GitHub says the scan targets common high-impact classes including injection, cross-site scripting, insecure data handling, path traversal, and weak cryptography.
- **Source:** [GitHub Changelog — security reviews in the Copilot app](https://github.blog/changelog/2026-07-14-security-reviews-now-available-in-the-github-copilot-app/)

### GitHub code scanning surfaces AI findings directly on pull requests

- **What changed:** GitHub code scanning can now run AI-powered detections when a pull request is opened or updated, extending coverage to languages and frameworks outside CodeQL’s built-in support. Findings appear directly on the pull request with an `AI` label and are informational rather than merge-blocking. The public preview requires GitHub Code Security, CodeQL default setup, an enabled enterprise and organization policy, a Copilot license, and AI credits.
- **Source:** [GitHub Changelog — AI security detections on pull requests](https://github.blog/changelog/2026-07-14-code-scanning-shows-ai-security-detections-on-pull-requests/)

### Copilot in Visual Studio expands modernization and pull-request workflows

- **What changed:** GitHub’s Visual Studio update made the Copilot modernization agent’s MSVC upgrade scenarios generally available for C++, with automated and guided execution modes. Copilot can now use a pull request’s description, changed files, and comments as chat context, while Visual Studio can review, approve, and complete GitHub or Azure DevOps pull requests inside the IDE. The update also added longer-range next-edit suggestions and real-time usage and limit alerts.
- **Source:** [GitHub Changelog — Copilot in Visual Studio June update](https://github.blog/changelog/2026-07-14-github-copilot-in-visual-studio-june-update)
