<div align="center">

<a href="https://clawskills.sh/">
<img width="1500" height="500" alt="social" src="https://github.com/user-attachments/assets/a6f310af-8fed-4766-9649-b190575b399d" />
</a>

<br/>
<br/>

<div align="center">
    <strong>Discover 5200+ community-built OpenClaw skills, organized by category.
    </strong>
    <br />
    <br />
</div>
  
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Skills Count](https://img.shields.io/badge/skills-5198-blue?style=flat-square)](#table-of-contents)
[![Last Update](https://img.shields.io/github/last-commit/VoltAgent/awesome-clawdbot-skills?label=Last%20update&style=flat-square)](https://github.com/VoltAgent/awesome-clawdbot-skills/pulls?q=is%3Apr+is%3Amerged+sort%3Aupdated-desc)
<a href="https://github.com/VoltAgent/voltagent">
  <img alt="VoltAgent" src="https://cdn.voltagent.dev/website/logo/logo-2-svg.svg" height="20" />
</a> 
[![Discord](https://img.shields.io/discord/1361559153780195478.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://s.voltagent.dev/discord)

</div>

<div align="center">
    <strong>More awesome collections for developers</strong>
    <br />
    <br />
</div>

<div align="center">

[![Agent Skills](https://img.shields.io/github/stars/VoltAgent/awesome-agent-skills?style=classic&label=%E2%9A%A1%20Agent%20Skills&color=black)](https://github.com/VoltAgent/awesome-agent-skills)
[![Claude Code Subagents](https://img.shields.io/github/stars/VoltAgent/awesome-claude-code-subagents?style=classic&label=Claude%20Code%20Subagents&color=D97757&logo=claude&logoColor=D97757)](https://github.com/VoltAgent/awesome-claude-code-subagents)
[![Codex Subagents][codex-badge]][codex-link]
[![AI Agent Papers](https://img.shields.io/github/stars/VoltAgent/awesome-ai-agent-papers?style=classic&label=AI%20Agent%20Papers&color=b31b1b&logo=arxiv)](https://github.com/VoltAgent/awesome-ai-agent-papers)

</div>

</div>

</div>

# Awesome OpenClaw Skills

OpenClaw is a locally-running AI assistant that operates directly on your machine. Skills extend its capabilities, allowing it to interact with external services, automate workflows, and perform specialized tasks. This collection helps you discover and install the right skills for your needs. It can also serve as a source of inspiration for OpenClaw use cases.

Skills in this list are sourced from ClawHub (OpenClaw's public skills registry) and categorized for easier discovery.

### Installation

#### ClawHub CLI


```bash
clawhub install <skill-slug>
```

#### Manual Installation

Copy the skill folder to one of these locations:

| Location | Path |
|----------|------|
| Global | `~/.openclaw/skills/` |
| Workspace | `<project>/skills/` |

Priority: Workspace > Local > Bundled

#### Alternative

You can also paste the skill's GitHub repository link directly into your assistant's chat and ask it to use it. The assistant will handle the setup automatically in the background.


### Why This List Exists?

OpenClaw's public registry (ClawHub) hosts **13,729 community-built skills** as of February 28, 2026. This awesome list has **5,211 skills**. Here's what we filtered out:

| Filter | Excluded |
|--------|----------|
| Possibly spam — bulk accounts, bot accounts, test/junk | 4,065 |
| Duplicate / Similar name | 1,040 |
| Low-quality or non-English descriptions | 851 |
| Crypto / Blockchain / Finance / Trade | 886 |
| Malicious — identified by security audits published by researchers (excluding VirusTotal) | 373 |
| **Total not taken from OpenClaw's official skill registry** | **7,215** |


#### Want to add a skill?

This list only includes skills that are **already published** in the `github.com/openclaw/skills` repository. We do not accept links to personal repos, gists, or any other external source. If your skill isn't in the OpenClaw skills repo yet, publish it there first. 

Include both the ClawHub link (e.g. `https://clawhub.ai/steipete/slack`) and the GitHub link (e.g. `https://github.com/openclaw/skills/tree/main/skills/steipete/slack`) in your PR description. See [CONTRIBUTING.md](CONTRIBUTING.md) for details.


## OpenClaw Ecosystem Tools

### 🔌 Connecting to External Services

OpenClaw agents can interact with external services like GitHub, Slack, Gmail, and more. You can build integrations yourself with Skills or Plugins, or use a managed service to handle auth, token refresh, and permissions across all your connections.

<a href="https://composio.dev/claw?utm_source=github&utm_campaign=volt-agent">
<img src="https://cdn.voltagent.dev/awesome-repo/composio-img.png" alt="Composio"  />
Managed OAuth, scoped permissions, and logged native toolcalls across 1000+ apps.
</a>


### 🤖 Model Providers

OpenClaw works with **25+ LLM providers** out of the box Anthropic, OpenAI and many more. Switch between them with a single config change.

<details>
<summary><strong>Example: Using OpenAI models</strong></summary>

OpenClaw supports `gpt-5.4` and `gpt-5.4-pro` via direct API key or ChatGPT/Codex OAuth. WebSocket transport is enabled by default for lower latency.

```bash
openclaw onboard --auth-choice openai-api-key
# or use subscription-based access:
openclaw onboard --auth-choice openai-codex
```
</details>


### ☁️ Hosting & Deployment

You can deploy OpenClaw on any VPS or cloud platform run your skills securely on your own infrastructure, or a managed host. Docker, Podman, Nix, and Ansible are all supported as install methods.

> **Tip:** If you're looking for a quick cloud setup, spin up a VPS with your preferred provider, install OpenClaw via Docker, and you're good to go.


<div align="center">

<table>
<tr>
<td align="center" width="100%">

<h3>🦞 You can feature your OpenClaw ecosystem tool in the section above.</h3>

<p></p>

<sub>📈 <strong>+1M monthly views</strong> — the #1 most visited community resource after the official OpenClaw resource</sub>

<br/>

<a href="mailto:necati@voltagent.dev"><img src="https://img.shields.io/badge/📩_Become_a_Sponsor-Contact_Us-blue?style=for-the-badge&logoColor=white" alt="Become a Sponsor" /></a>

</td>
</tr>
</table>

</div>

## Security Notice

Skills in this list are **curated, not audited**. They may be updated, modified, or replaced by their original maintainers at any time after being added here.

Before installing or using any Agent Skill, review potential security risks and validate the source yourself. OpenClaw has a **VirusTotal partnership** that provides security scanning for skills, visit a skill's page on ClawHub and check the VirusTotal report to see if it's flagged as risky.

**Recommended tools:**

- [Snyk Skill Security Scanner](https://github.com/snyk/agent-scan)
- [Agent Trust Hub](https://ai.gendigital.com/agent-trust-hub)
  
> Agent skills can include prompt injections, tool poisoning, hidden malware payloads, or unsafe data handling patterns. Always review the source code before installing and use skills at your own discretion.

If you believe a skill in this list should be flagged or has a security concern, please [open an issue](https://github.com/VoltAgent/awesome-clawdbot-skills/issues) so we can review it.

## Table of Contents

| | | |
|---|---|---|
| [Git & GitHub](#git--github) (167) | [Marketing & Sales](#marketing--sales) (102) | [Communication](#communication) (146) |
| [Coding Agents & IDEs](#coding-agents--ides) (1184) | [Productivity & Tasks](#productivity--tasks) (205) | [Speech & Transcription](#speech--transcription) (45) |
| [Browser & Automation](#browser--automation) (322) | [AI & LLMs](#ai--llms) (176) | [Smart Home & IoT](#smart-home--iot) (41) |
| [Web & Frontend Development](#web--frontend-development) (919) | [Data & Analytics](#data--analytics) (28) | [Shopping & E-commerce](#shopping--e-commerce) (51) |
| [DevOps & Cloud](#devops--cloud) (393) | [Calendar & Scheduling](#calendar--scheduling) (65) | |
| [Image & Video Generation](#image--video-generation) (170) | [Media & Streaming](#media--streaming) (85) | [PDF & Documents](#pdf--documents) (105) |
| [Apple Apps & Services](#apple-apps--services) (44) | [Notes & PKM](#notes--pkm) (69) | [Self-Hosted & Automation](#self-hosted--automation) (33) |
| [Search & Research](#search--research) (345) | [iOS & macOS Development](#ios-and-macos-development) (29) | [Security & Passwords](#security--passwords) (53) |
| [Clawdbot Tools](#clawdbot-tools) (37) | [Transportation](#transportation) (110) | [Moltbook](#moltbook) (29) |
| [CLI Utilities](#cli-utilities) (180) | [Personal Development](#personal-development) (50) | [Gaming](#gaming) (35) |
| [Health & Fitness](#health--fitness) (87) | | |

> Mirror note: this file was copied into this repository. The source list repo is `VoltAgent/awesome-openclaw-skills`.

## License

MIT License - see [LICENSE](LICENSE)

Skills in this list are sourced from the OpenClaw official skills repo and categorized for easier discovery. Skills listed here are created and maintained by their respective authors, not by us. We do not audit, endorse, or guarantee the security or correctness of listed projects. They are not security-audited and should be reviewed before production use.

If you find an issue with a listed skill or want your skill removed, please open an issue and we'll take care of it promptly.

[codex-badge]: https://img.shields.io/github/stars/VoltAgent/awesome-codex-subagents?style=classic&label=Codex%20Subagents&color=000000&logo=data:image/svg%2bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdiIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJ3aGl0ZSI+PHBhdGggZD0iTTIyLjI4MiA5LjgyMWE1Ljk4NSA1Ljk4NSAwIDAgMC0uNTE2LTQuOTEgNi4wNDYgNi4wNDYgMCAwIDAtNi41MS0yLjlBNi4wNjUgNi4wNjUgMCAwIDAgNC45ODEgNC4xOGE1Ljk4NSA1Ljk4NSAwIDAgMC0zLjk5OCAyLjkgNi4wNDYgNi4wNDYgMCAwIDAgLjc0MyA3LjA5NyA1Ljk4IDUuOTggMCAwIDAgLjUxIDQuOTExIDYuMDUxIDYuMDUxIDAgMCAwIDYuNTE1IDIuOUE1Ljk4NSA1Ljk4NSAwIDAgMCAxMy4yNiAyNGE2LjA1NiA2LjA1NiAwIDAgMCA1Ljc3Mi00LjIwNiA1Ljk5IDUuOTkgMCAwIDAgMy45OTctMi45IDYuMDU2IDYuMDU2IDAgMCAwLS43NDctNy4wNzN6TTEzLjI2IDIyLjQzYTQuNDc2IDQuNDc2IDAgMCAxLTIuODc2LTEuMDRsLjE0MS0uMDgxIDQuNzc5LTIuNzU4YS43OTUuNzk1IDAgMCAwIC4zOTItLjY4MXYtNi43MzdsMi4wMiAxLjE2OGEuMDcxLjA3MSAwIDAgMSAuMDM4LjA1MnY1LjU4M2E0LjUwNCA0LjUwNCAwIDAgMS00LjQ5NCA0LjQ5NHpNMy42IDE4LjMwNGE0LjQ3IDQuNDcgMCAwIDEtLjUzNS0zLjAxNGwuMTQyLjA4NSA0Ljc4MyAyLjc1OWEuNzcxLjc3MSAwIDAgMCAuNzggMGw1Ljg0My0zLjM2OXYyLjMzMmEuMDguMDggMCAwIDEtLjAzMy4wNjJMOS43NCAxOS45NWE0LjUgNC41IDAgMCAxLTYuMTQtMS42NDZ6TTIuMzQgNy44OTZhNC40ODUgNC40ODUgMCAwIDEgMi4zNjYtMS45NzNWMTEuNmEuNzY2Ljc2NiAwIDAgMCAuMzg4LjY3Nmw1LjgxNSAzLjM1NS0yLjAyIDEuMTY4YS4wNzYuMDc2IDAgMCAxLS4wNzEgMGwtNC44My0yLjc4NkE0LjUwNCA0LjUwNCAwIDAgMSAyLjM0IDcuODcybTE2LjU5NyAzLjg1NWwtNS44MzMtMy4zODdMMTUuMTE5IDcuMmEuMDc2LjA3NiAwIDAgMSAuMDcxIDBsNC44MyAyLjc5MWE0LjQ5NCA0LjQ5NCAwIDAgMS0uNjc2IDguMTA1di01LjY3OGEuLjc5Ljc5IDAgMCAwLS40MDctLjY2N3ptMi4wMS0zLjAyM2wtLjE0MS0uMDg1LTQuNzc0LTIuNzgyYS43NzYuNzc2IDAgMCAwLS43ODUgMEw5LjQwOSA5LjIzVjYuODk3YS4wNjYuMDY2IDAgMCAxIC4wMjgtLjA2MWw0LjgzLTIuNzg3YTQuNSA0LjUgMCAwIDEgNi42OCA0LjY2bS0xMi42NCA0LjEzNWwtMi4wMi0xLjE2NGEuMDguMDggMCAwIDEtLjAzOC0uMDU3VjYuMDc1YTQuNSA0LjUgMCAwIDEgNy4zNzUtMy40NTNsLS4xNDIuMDhMOC43MDQgNS40NmEuNzk1Ljc5NSAwIDAgMC0uMzkzLjY4MXptMS4wOTctMi4zNjVsMi42MDItMS41IDIuNjA3IDEuNXYyLjk5OWwtMi41OTcgMS41LTIuNjA3LTEuNXoiLz48L3N2Zz4=
[codex-link]: https://github.com/VoltAgent/awesome-codex-subagents