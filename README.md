<div align="center">

# AI Builder Studio

**One master skill for building AI-powered applications with text, files, images, audio, video, search, and agents.**

`1 Master Skill` · `13 Internal Modules` · `Claude Code` · `OpenCode`

</div>

---

## About

Build reliable AI applications with provider-aware architecture, safe data handling, evaluation, user-centered UX, and explicit separation between model capabilities and configured external services.

This repository exposes one discoverable skill: `ai-builder-studio`. Specialist playbooks live inside that skill's `references/` directory and are loaded by the master workflow as needed. You do not select each module separately.

## Quick start

### Project-local use

Copy this repository's `.claude/skills/ai-builder-studio/` folder into the target project's `.claude/skills/` directory. Then invoke the master skill from your compatible coding agent.

### Claude Code

```text
/ai-builder-studio
```

### OpenCode

```text
@ai-builder-studio
```

Agent discovery behavior can vary by installed version and configuration. Confirm the skill appears in the agent's available skill list before relying on it.

## Internal specialist modules

| Module | Role |
|---|---|
| `ai-application-engineer` | Internal specialist reference |
| `ai-model-integration` | Internal specialist reference |
| `rag-engineer` | Internal specialist reference |
| `multimodal-ai-engineer` | Internal specialist reference |
| `ai-inference-optimizer` | Internal specialist reference |
| `ai-voice-engineer` | Internal specialist reference |
| `ai-image-engineer` | Internal specialist reference |
| `ai-video-engineer` | Internal specialist reference |
| `ai-search-engineer` | Internal specialist reference |
| `ai-evaluation-engineer` | Internal specialist reference |
| `human-centered-product-design` | Shared human-centered quality reference |
| `design-quality-critic` | Shared human-centered quality reference |
| `product-experience-engineer` | Shared human-centered quality reference |

## Repository layout

```text
ai-builder-studio/
├── .claude/skills/ai-builder-studio/
│   ├── SKILL.md
│   ├── references/
│   ├── scripts/
│   ├── templates/
│   └── assets/
├── scripts/
├── README.md
├── README_BN.md
└── AGENTS.md
```

## Validation

Run: `python scripts/validate_pack.py`

The validator checks the master skill, expected reference files, frontmatter, basic link integrity, and accidental secrets. It does not prove provider/API availability or guarantee production behavior.

## Safety and service requirements

This repository contains agent instructions, reference playbooks, templates, and helper scripts. It is not itself a model, API subscription, cloud runtime, media-generation engine, or deployment service. Actual capabilities depend on tools, credentials, permissions, provider terms, quotas, dependencies, and hardware configured in your environment. Never commit secrets.

## Contribution and updates

Keep the master skill as the sole discoverable entry point. Add new specialist knowledge as internal references unless there is a deliberate decision to expose a new independent skill. Update the manifest and validation checks whenever modules change.
