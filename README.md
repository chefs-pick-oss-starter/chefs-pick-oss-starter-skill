<!-- Source: Best-README-Template BLANK_README (Unlicense) — https://github.com/othneildrew/Best-README-Template -->
<a id="readme-top"></a>

# Chef's Pick OSS Starter Skill

An agent skill that creates a repository from the Chef's Pick OSS Starter template, or aligns an existing repository with it.

[![CI](https://github.com/anyingiit/chefs-pick-oss-starter-skill/actions/workflows/ci.yml/badge.svg)](https://github.com/anyingiit/chefs-pick-oss-starter-skill/actions/workflows/ci.yml)
[![License](https://img.shields.io/github/license/anyingiit/chefs-pick-oss-starter-skill)](LICENSE)

[Report a bug](https://github.com/anyingiit/chefs-pick-oss-starter-skill/issues/new?template=bug_report.yml) · [Request a feature](https://github.com/anyingiit/chefs-pick-oss-starter-skill/issues/new?template=feature_request.yml)

## What it is

An [Agent Skills](https://agentskills.io/specification) package that lets a coding agent do the [Chef's Pick OSS Starter](https://github.com/anyingiit/chefs-pick-oss-starter) setup for you. It works in two modes:

- **Create**: make a new repository from the template, fill in your project's identity, walk the setup checklist and remove the template's guide layer.
- **Align**: bring an existing repository to the template's recommended form. The repository may never have used the template, or it may have been made from an older version of it.

The agent fetches the template's current content on every run, shows you the full plan before changing anything, and asks before touching any file you already have. The rules it follows are in [`skills/chefs-pick-oss-starter/`](skills/chefs-pick-oss-starter/SKILL.md).

## Install

Install it once for all your repositories with the [skills CLI](https://github.com/vercel-labs/skills). It detects which of the agents below you have:

```sh
npx skills add anyingiit/chefs-pick-oss-starter-skill -g
```

Or use your agent's own way of installing skills:

| Agent | Install |
|---|---|
| Claude Code | `/plugin marketplace add anyingiit/chefs-pick-oss-starter-skill`, then `/plugin install chefs-pick-oss-starter@chefs-pick` |
| OpenAI Codex | Copy `skills/chefs-pick-oss-starter` into `~/.agents/skills/` |
| OpenCode | Copy `skills/chefs-pick-oss-starter` into `~/.config/opencode/skills/` |

## Uninstall

```sh
npx skills remove chefs-pick-oss-starter -g
```

Or, if you installed it the agent's own way:

| Agent | Uninstall |
|---|---|
| Claude Code | `/plugin uninstall chefs-pick-oss-starter@chefs-pick`, and optionally `/plugin marketplace remove chefs-pick` |
| OpenAI Codex | Delete `~/.agents/skills/chefs-pick-oss-starter` |
| OpenCode | Delete `~/.config/opencode/skills/chefs-pick-oss-starter` |

## Use

Ask your agent in plain words, for example:

- `Create a new repository called hello-world with Chef's Pick.`
- `Align this repository with Chef's Pick.`

You do not have to install anything to try it once: copy the prompt from the "Set up with an agent" section of the [template's front page](https://github.com/anyingiit/chefs-pick-oss-starter/blob/main/.github/README.md) into your agent instead.

## Compatibility

Verified end to end on 2026-09-23 with Claude Code, OpenAI Codex and OpenCode: installed with the command above, triggered by a plain request, used to align and to create a repository, and uninstalled.

The skill follows the open [Agent Skills](https://agentskills.io/specification) format. GitHub Copilot, Gemini CLI and Cursor document support for that format too, but have not been verified with this skill.

The agent needs `git` and read access to github.com. The GitHub CLI (`gh`), signed in, is optional; it is only used for repository settings you approve one by one.

In Codex, network access is off by default. Allow it before running the skill, for example by starting Codex with `-c sandbox_workspace_write.network_access=true`.

## Template versions

Works with Chef's Pick OSS Starter 1.1.0 and later. The template lives at <https://github.com/anyingiit/chefs-pick-oss-starter>.

## Contributing

Contributions are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) for how to open an issue or a pull request, and [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) for the standards expected of everyone taking part.

Please do not report security issues in public issues or pull requests. [SECURITY.md](SECURITY.md) explains how to report them privately.

## License

Distributed under the MIT License. See [LICENSE](LICENSE) for details.

## Contact

Project link: [https://github.com/anyingiit/chefs-pick-oss-starter-skill](https://github.com/anyingiit/chefs-pick-oss-starter-skill)

<p align="right">(<a href="#readme-top">back to top</a>)</p>
