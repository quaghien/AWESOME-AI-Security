# AWESOME-AI-Security

A curated list of AI Security papers, standards, tools, and repositories for learning **LLM Security**, **Agent Security**, **Red Teaming**, and **Runtime Guardrails**.

---

## Table of Contents

* [OWASP & NIST](#owasp--nist)
* [Paper](#paper)

  * [Agent AI Security Survey](#agent-ai-security-survey)
  * [Agentic SOC / Security Operations Automation](#agentic-soc--security-operations-automation)
  * [RL Red Teaming / Attacker-Defender Adversarial](#rl-red-teaming--attacker-defender-adversarial)
* [Repo](#repo)
* [Tool Comparison](#tool-comparison)
* [AI Security Workflow](#ai-security-workflow)

<p align="center">
  <img src="./assets/ai-security-1.png" alt="Keywords in AI Security" width="50%">
</p>

<p align="center">
  <img src="./assets/ai-security-2.png" alt="AI Agent Security Workflow without Guardrails" width="50%">
</p>

<p align="center">
  <img src="./assets/ai-security-3.png" alt="AI Agent Security Workflow with Guardrails" width="100%">
</p>

---

## OWASP & NIST

| Time    | Title                                                                                                                                  | Org   | Type          | Note                                                               |
| ------- | -------------------------------------------------------------------------------------------------------------------------------------- | ----- | ------------- | ------------------------------------------------------------------ |
| 2026.03 | [OWASP GenAI Data Security Risks & Mitigations 2026](https://genai.owasp.org/)                                                         | OWASP | Guide         | Data security risks and mitigations for GenAI systems              |
| 2025.12 | [OWASP Top 10 for Agentic Applications 2026](https://genai.owasp.org/resource/owasp-top-10-for-agentic-applications-for-2026/)         | OWASP | Top 10        | Core risks for autonomous and agentic AI systems                   |
| 2025.12 | [Cybersecurity Framework Profile for Artificial Intelligence](https://www.nist.gov/itl/ai-risk-management-framework)                   | NIST  | Draft Profile | Cybersecurity framework profile for AI systems                     |
| 2025.11 | [OWASP AI Testing Guide](https://github.com/OWASP/www-project-ai-testing-guide)                                                        | OWASP | Testing Guide | Practical guide for testing AI system security and trustworthiness |
| 2025.03 | [Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations](https://csrc.nist.gov/pubs/ai/100/2/e2025/final) | NIST  | Taxonomy      | Core taxonomy for AI attacks, defenses, and mitigations            |

---

## Paper

### Agent AI Security Survey

| Time    | Title                                                                                                                                               | Venue | Code |
| ------- | --------------------------------------------------------------------------------------------------------------------------------------------------- | ----- | ---- |
| 2026.06 | [Toward Secure LLM Agents: Threat Surfaces, Attacks, Defenses, and Evaluation](https://arxiv.org/abs/2606.10749)                                    | arXiv | -    |
| 2026.04 | [A Systematic Survey of Security Threats and Defenses in LLM-Based AI Agents: A Layered Attack Surface Framework](https://arxiv.org/abs/2604.23338) | arXiv | -    |

### Agentic SOC / Security Operations Automation

| Time    | Title                                                                                                               | Venue           | Code | Note                                                                              |
| ------- | ------------------------------------------------------------------------------------------------------------------- | --------------- | ---- | --------------------------------------------------------------------------------- |
| 2026.04 | [AgentSOC: A Multi-Layer Agentic AI Framework for Security Operations Automation](https://arxiv.org/abs/2604.20134) | IEEE ICAIC 2026 | -    | Multi-layer agentic AI framework for SOC triage, reasoning, and response planning |

### RL Red Teaming / Attacker-Defender Adversarial

> Note: only papers with public code are listed here.

| Time    | Title                                                                                                                                          | Venue     | Code                                                                          | Note                                                     |
| ------- | ---------------------------------------------------------------------------------------------------------------------------------------------- | --------- | ----------------------------------------------------------------------------- | -------------------------------------------------------- |
| 2026.03 | [PISmith: Reinforcement Learning-based Red Teaming for Prompt Injection Defenses](https://arxiv.org/abs/2603.13026)                            | arXiv     | [albert-y1n / PISmith](https://github.com/albert-y1n/PISmith)                 | RL attacker for prompt injection defenses                |
| 2026.03 | [T-MAP: Red-Teaming LLM Agents with Trajectory-aware Evolutionary Search](https://arxiv.org/abs/2603.22341)                                    | arXiv     | [pwnhyo / T-MAP](https://github.com/pwnhyo/T-MAP)                             | Trajectory-aware red teaming for MCP/tool-using agents   |
| 2026.02 | [Learning to Inject: Automated Prompt Injection via Reinforcement Learning](https://arxiv.org/abs/2602.05746)                                  | arXiv     | [RPC2 / AutoInject](https://github.com/RPC2/AutoInject)                       | RL-based automated prompt injection for LLM agents       |
| 2026.02 | [MAGIC: A Co-Evolving Attacker-Defender Adversarial Game for Robust LLM Safety](https://arxiv.org/abs/2602.01539)                              | ICML 2026 | [AI45Lab / MAGIC](https://github.com/AI45Lab/MAGIC)                           | Multi-agent attacker-defender reinforcement learning     |
| 2025.12 | [TROJail: Trajectory-Level Optimization for Multi-Turn Large Language Model Jailbreaks with Process Rewards](https://arxiv.org/abs/2512.07761) | ACL 2026  | [xxiqiao / TROJail](https://github.com/xxiqiao/TROJail)                       | Multi-turn RL jailbreak with process rewards             |
| 2025.10 | [RedCodeAgent: Automatic Red-teaming Agent against Diverse Code Agents](https://arxiv.org/abs/2510.02609)                                      | ICLR 2026 | [1mocat / RedCodeAgent](https://github.com/1mocat/RedCodeAgent)               | Automated red-teaming agent for code agents              |
| 2025.09 | [Active Attacks: Red-teaming LLMs via Adaptive Environments](https://arxiv.org/abs/2509.21947)                                                 | ICML 2026 | [dbsxodud-11 / active_attacks](https://github.com/dbsxodud-11/active_attacks) | RL red teaming with adaptive victim/environment feedback |

---

## Repo

| Repo                                                                  | Category                     | Stage                 | Short Note                                                                  |
| --------------------------------------------------------------------- | ---------------------------- | --------------------- | --------------------------------------------------------------------------- |
| [promptfoo / promptfoo](https://github.com/promptfoo/promptfoo)       | LLM Testing / Red Team       | Dev & CI/CD           | Test prompts, RAGs, agents, regressions, and security cases before deploy   |
| [NVIDIA / garak](https://github.com/NVIDIA/garak)                     | LLM Vulnerability Scanner    | Security Audit        | Scan LLM apps for jailbreaks, prompt injection, leakage, toxicity, and more |
| [microsoft / PyRIT](https://github.com/microsoft/PyRIT)               | GenAI Red Team Framework     | Security Audit        | Automate single-turn and multi-turn adversarial testing                     |
| [NVIDIA / SkillSpector](https://github.com/NVIDIA/SkillSpector)       | Agent Skill Security         | Supply Chain Security | Scan third-party agent skills before installation                           |
| [snyk / agent-scan](https://github.com/snyk/agent-scan)               | Agent / MCP Security Scanner | Supply Chain Security | Scan AI agents, MCP servers, skills, secrets, and risky tool descriptions   |
| [protectai / llm-guard](https://github.com/protectai/llm-guard)       | Runtime Input / Output Guard | Production Runtime    | Detect and sanitize unsafe prompts, responses, PII, secrets, and injections |
| [NVIDIA-NeMo / Guardrails](https://github.com/NVIDIA-NeMo/Guardrails) | Runtime Guardrails           | Production Runtime    | Add programmable rails for input, dialog flow, retrieval, tools, and output |

---

## Tool Comparison

| Tool                                                         | Test Before Deploy | Real-Time Protection | Agent Security | Prompt Injection | Jailbreak | Data Leakage | Tool Misuse | Skill / Plugin / MCP Risk |
| ------------------------------------------------------------ | -----------------: | -------------------: | -------------: | ---------------: | --------: | -----------: | ----------: | ------------------------: |
| [promptfoo](https://github.com/promptfoo/promptfoo)          |                  ✅ |                    ❌ |              ✅ |                ✅ |         ✅ |            ✅ |           ✅ |                         ❌ |
| [garak](https://github.com/NVIDIA/garak)                     |                  ✅ |                    ❌ |             ⚠️ |                ✅ |         ✅ |            ✅ |          ⚠️ |                         ❌ |
| [PyRIT](https://github.com/microsoft/PyRIT)                  |                  ✅ |                    ❌ |              ✅ |                ✅ |         ✅ |            ✅ |           ✅ |                         ❌ |
| [SkillSpector](https://github.com/NVIDIA/SkillSpector)       |                  ✅ |                    ❌ |              ✅ |               ⚠️ |         ❌ |           ⚠️ |           ✅ |                         ✅ |
| [agent-scan](https://github.com/snyk/agent-scan)             |                  ✅ |                    ❌ |              ✅ |                ✅ |        ⚠️ |            ✅ |           ✅ |                         ✅ |
| [llm-guard](https://github.com/protectai/llm-guard)          |                 ⚠️ |                    ✅ |             ⚠️ |                ✅ |        ⚠️ |            ✅ |           ❌ |                         ❌ |
| [NeMo Guardrails](https://github.com/NVIDIA-NeMo/Guardrails) |                 ⚠️ |                    ✅ |              ✅ |                ✅ |         ✅ |            ✅ |           ✅ |                         ❌ |

Legend:

* ✅ Strong fit
* ⚠️ Partial fit / depends on setup
* ❌ Not the main purpose

---

## AI Security Workflow

```text
[ Development & Deployment ]

1. Dev & CI/CD
   └── promptfoo
       ├── Test prompt behavior
       ├── Test RAG quality
       ├── Test agent logic
       ├── Run regression tests
       └── Integrate into GitHub Actions / CI pipeline

2. Security Audit
   ├── garak
   │   ├── Scan common LLM vulnerabilities
   │   ├── Test prompt injection
   │   ├── Test jailbreaks
   │   ├── Test data leakage
   │   └── Generate security reports
   │
   └── PyRIT
       ├── Simulate single-turn / multi-turn attackers
       ├── Test complex adversarial conversations
       ├── Evaluate agent behavior under attack
       └── Test tool misuse and sensitive data leakage

3. Supply Chain Security
   ├── SkillSpector
   │   ├── Scan third-party agent skills
   │   ├── Detect risky instructions
   │   ├── Detect malicious patterns
   │   ├── Review tool permissions
   │   └── Check before installing skills
   │
   └── agent-scan
       ├── Discover local AI agent configs
       ├── Scan MCP servers and tools
       ├── Detect tool poisoning / shadowing risks
       ├── Detect secrets and unsafe credential handling
       └── Check agent supply chain before use


[ Production Runtime ]

4. Real-Time Protection
   ├── llm-guard
   │   ├── Input scanning
   │   ├── Output scanning
   │   ├── PII / secret detection
   │   ├── Prompt injection detection
   │   └── Response sanitization
   │
   └── NeMo Guardrails
       ├── Input guardrails
       ├── Dialog guardrails
       ├── Retrieval guardrails
       ├── Tool / execution guardrails
       └── Output guardrails
```

---
