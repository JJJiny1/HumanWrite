# HumanWrite

An Agent Skill for natural prose, user-directed writing, and consistent essay arguments. Version: 0.1.0.

HumanWrite is an instruction package for AI assistants that support skills. It is not a standalone application and requires no API key or runtime dependencies. Project documentation is in English; writing output follows the user's requested language.

## Features

- Natural, clear writing by default, with an automatic review for vague language, repetition, and mechanical phrasing.
- Two or three suggested directions when a new writing task has no clear direction. Drafting starts after the user chooses, unless they delegate the choice.
- Direct handling of clear theses, outlines, polishing, translation, summaries, and revisions.
- Optional personal writing profiles, disabled by default. Private samples are not saved without permission.
- Mandatory essay review covering thesis, paragraph claims, facts, concepts, and evidence. Counterarguments and conditional claims are distinguished from contradictions.

Reviews can reduce errors but cannot guarantee that every logical problem will be found or replace checking original sources. HumanWrite does not promise AI-detector evasion or invent citations or personal experiences.

## Quick Start

### Option 1: Copy & Paste (No Installation)

For ChatGPT, Claude, Gemini, and other AI assistants.

1. Open [HumanWrite Full Prompt](prompts/HumanWrite-Full.md).
2. Copy the entire prompt.
3. Paste it into your AI assistant.
4. Start writing naturally.

No installation or additional files required.

### Option 2: Install as an Agent Skill

For Codex, Claude Code, and compatible AI agents.

```bash
npx skills add JJJiny1/HumanWrite
```

Or follow the manual installation instructions below.


## Installation

Install the complete `skills/humanwrite/` folder, including `SKILL.md`, `references/`, and `agents/`.

For environments that use `~/.codex/skills` as their user skill directory, download or clone this repository and run these commands from the repository root:

```sh
mkdir -p ~/.codex/skills
cp -R skills/humanwrite ~/.codex/skills/
```

If the destination already exists, back up the old version before updating to avoid mixing obsolete files. Replace the destination if your environment uses a custom skill directory. Refresh skill discovery or start a new session as required by your host, then try `$humanwrite`. Compatibility and installation procedures for other agents depend on their own skill support.

## Usage

```text
Use $humanwrite to help me write an essay about globalization. Suggest a few directions first.
```

```text
Use $humanwrite to write an 800-word essay arguing that globalization can support growth in developing countries, but its benefits are unevenly distributed.
```

```text
Use $humanwrite to review this essay for contradictions. Preserve counterarguments and report issues before rewriting.
```

```text
Use $humanwrite to polish the following paragraph without changing its meaning. For this task, use my preferred style: concise, restrained, and free of stock phrases.
```

See the optional [personal writing profile](skills/humanwrite/references/personal-writing-profile.md).

## Project contents

- [SKILL.md](skills/humanwrite/SKILL.md): entry point and writing workflow.
- [Essay consistency](skills/humanwrite/references/essay-consistency.md): mandatory argument review.
- [Quality checklist](skills/humanwrite/references/quality-checklist.md): pre-delivery checks.
- [Acceptance scenarios](examples/acceptance-scenarios.md): manual behavioral evaluation.
- [Contributing](CONTRIBUTING.md): changes and validation.

## Repository and validation

Repository: [JJJiny1/HumanWrite](https://github.com/JJJiny1/HumanWrite).

Version 0.1.0 has received structural and internal-link checks. Real model behavior still needs evaluation in a compatible host using the acceptance scenarios. Structural checks do not establish writing quality.

Do not upload private writing samples, personal profiles, or secrets. `.gitignore` helps prevent accidental Git commits but does not prevent manual browser uploads.

## License

[MIT](LICENSE).
