<p align="center">
  <img src="./assets/header.svg" width="100%" alt="Seungwoo Lee — AI-native engineer. From research to real-world systems. Co-founder at SECA, Seoul." />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/seungwoo-dale-lee/">LinkedIn</a> &nbsp;&nbsp;
  <a href="mailto:lifrary2050@gmail.com">Email</a> &nbsp;&nbsp;
  <a href="https://github.com/lifrary/agent-tree">agent-tree</a>
</p>

## Hi, I'm Seungwoo (Dale) Lee

I'm an AI engineer and **co-founder at SECA**, an AI startup spun out of LG Electronics, based in Seoul.

I design end-to-end AI pipelines and turn them into products people can use: data processing, models, tools and evaluation, connected into one system. I use AI throughout development to build, test and refine that work. At SECA, I apply this approach to complex hardware data.

Before SECA I worked at **LG Electronics AI LAB** and **NAVER**, and did research at **Seoul National University**.

## Selected work

### [agent-tree](https://github.com/lifrary/agent-tree)

[![npm](https://img.shields.io/npm/v/@seungwoolee/agent-tree.svg?color=cb3837&label=npm)](https://www.npmjs.com/package/@seungwoolee/agent-tree)
[![GitHub stars](https://img.shields.io/github/stars/lifrary/agent-tree?style=flat&logo=github&label=stars)](https://github.com/lifrary/agent-tree/stargazers)
[![license: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/lifrary/agent-tree/blob/main/LICENSE)

**Navigate Claude Code and Codex sessions as numbered trees, and pick up from any point.**

A long agent session is hard to look back on. agent-tree reads the session logs that Claude Code and Codex CLI already keep and turns each one into a numbered outline: every prompt you typed, with the reads, edits and commands it triggered nested underneath. Pick any step and you get a ready-to-paste prompt that **continues** from there in a fresh session, or **forks** to try another way.

<p align="center">
  <a href="https://github.com/lifrary/agent-tree">
    <img src="https://raw.githubusercontent.com/lifrary/agent-tree/main/docs/demo.svg" width="760" alt="agent-tree printing a Claude Code session as a numbered tree with two starred resume points" />
  </a>
</p>

- **In the terminal:** an interactive tree, plus `--list`, `--diff` and `--json` output for scripts.
- **Inside Claude Code:** a plugin with six MCP tools, so Claude can list, browse and resume sessions for you.
- **Local and redacted:** it reads the logs already on your machine and strips API keys, tokens and card numbers before anything is shown, copied or exported.

```bash
npm install -g @seungwoolee/agent-tree
```

[Repository](https://github.com/lifrary/agent-tree) &nbsp;·&nbsp; [npm package](https://www.npmjs.com/package/@seungwoolee/agent-tree) &nbsp;·&nbsp; [Latest release](https://github.com/lifrary/agent-tree/releases/latest)

If it saves you a long scroll through a session log, a star on the repo helps other people find it.

## Open source contributions

I fix the reliability bugs I run into in the AI developer tools I use every day. 36 of my changes have landed in 14 projects. Most of them fix processes that never exit, crashes, silent failures and lost data.

| Project | Stars | Landed | What I fixed |
|:--|:--|:-:|:--|
| [**oh-my-claudecode**](https://github.com/Yeachan-Heo/oh-my-claudecode)<br><sub>Yeachan-Heo</sub> | ![stars](https://img.shields.io/github/stars/Yeachan-Heo/oh-my-claudecode?style=flat&logo=github&label=) | 9 | Unified 8 copies of the process-liveness check, 5 of which treated `EPERM` as a dead process ([#1843](https://github.com/Yeachan-Heo/oh-my-claudecode/pull/1843)); moved stop-hook enforcement into the scripts that actually run ([#1480](https://github.com/Yeachan-Heo/oh-my-claudecode/pull/1480), [#1482](https://github.com/Yeachan-Heo/oh-my-claudecode/pull/1482)). |
| [**oh-my-codex**](https://github.com/Yeachan-Heo/oh-my-codex)<br><sub>Yeachan-Heo</sub> | ![stars](https://img.shields.io/github/stars/Yeachan-Heo/oh-my-codex?style=flat&logo=github&label=) | 6 | Stopped `codex` from being orphaned when tmux kills its session ([#1605](https://github.com/Yeachan-Heo/oh-my-codex/pull/1605)); made the runtime bridge survive partial writes ([#1918](https://github.com/Yeachan-Heo/oh-my-codex/pull/1918)) and report failed disk writes instead of exiting 0 ([#1303](https://github.com/Yeachan-Heo/oh-my-codex/pull/1303)). |
| [**oh-my-openagent**](https://github.com/code-yeongyu/oh-my-openagent)<br><sub>code-yeongyu</sub> | ![stars](https://img.shields.io/github/stars/code-yeongyu/oh-my-openagent?style=flat&logo=github&label=) | 1 | Fixed idle stdio MCP servers that could never exit, because the idle timeout never closed stdin. Reported in [#6547](https://github.com/code-yeongyu/oh-my-openagent/issues/6547); both commits landed in [#7525](https://github.com/code-yeongyu/oh-my-openagent/pull/7525). |
| [**openworker**](https://github.com/andrewyng/openworker)<br><sub>andrewyng</sub> | ![stars](https://img.shields.io/github/stars/andrewyng/openworker?style=flat&logo=github&label=) | 1 | Made the conversation-log rewrite atomic, so a crash during context compaction can no longer wipe a conversation history ([#70](https://github.com/andrewyng/openworker/pull/70)). |
| [**opencodex**](https://github.com/lidge-jun/opencodex)<br><sub>lidge-jun</sub> | ![stars](https://img.shields.io/github/stars/lidge-jun/opencodex?style=flat&logo=github&label=) | 2 | Capped the response spill directory, which had no total size limit and could fill a disk within an hour ([#3097](https://github.com/lidge-jun/opencodex/pull/3097)); fixed tests that assumed pid 4242 is always free ([#3137](https://github.com/lidge-jun/opencodex/pull/3137)). |
| [**PyMuPDF**](https://github.com/pymupdf/PyMuPDF)<br><sub>pymupdf</sub> | ![stars](https://img.shields.io/github/stars/pymupdf/PyMuPDF?style=flat&logo=github&label=) | 1 | Fixed a segfault in the C++ bindings when a `get_cdrawings()` callback raises; the failure is now reported and extraction continues ([#5139](https://github.com/pymupdf/PyMuPDF/pull/5139)). |
| [**gajae-code**](https://github.com/Yeachan-Heo/gajae-code)<br><sub>Yeachan-Heo</sub> | ![stars](https://img.shields.io/github/stars/Yeachan-Heo/gajae-code?style=flat&logo=github&label=) | 6 | A quota failure now marks the account that actually failed ([#5422](https://github.com/Yeachan-Heo/gajae-code/pull/5422)); an OAuth token rejected before its expiry is refreshed instead of leaving quota readings stale ([#6260](https://github.com/Yeachan-Heo/gajae-code/pull/6260)). |
| [**ouroboros**](https://github.com/Q00/ouroboros)<br><sub>Q00</sub> | ![stars](https://img.shields.io/github/stars/Q00/ouroboros?style=flat&logo=github&label=) | 3 | Stopped the welcome suggestion from firing forever for already-configured users ([#1152](https://github.com/Q00/ouroboros/pull/1152)); fixed a crash on `null` MCP parameters ([#325](https://github.com/Q00/ouroboros/pull/325)). |
| [**cmux**](https://github.com/manaflow-ai/cmux)<br><sub>manaflow-ai</sub> | ![stars](https://img.shields.io/github/stars/manaflow-ai/cmux?style=flat&logo=github&label=) | 1 | Replaced force-unwrapped UTF-8 conversions on file-write paths ([#1834](https://github.com/manaflow-ai/cmux/pull/1834)). |

Smaller fixes also landed in [oh-my-agent](https://github.com/first-fluke/oh-my-agent/pull/265) (an SQL-injection check that had never actually run), [memkraft](https://github.com/seojoonkim/memkraft/pull/3) (`recall` reported every stored entity as missing), [prism-insight](https://github.com/dragon1086/prism-insight/pull/227), [agf](https://github.com/subinium/agf/pull/1) and [openlogs](https://github.com/charlietlamb/openlogs/pull/3).

Two problems I reported were fixed by the maintainers: gajae-code showed an Anthropic rate limit as a generic stream timeout ([#1368](https://github.com/Yeachan-Heo/gajae-code/issues/1368), fixed in [#1369](https://github.com/Yeachan-Heo/gajae-code/pull/1369)), and oh-my-codex shipped with three high-severity vulnerable dependencies ([#888](https://github.com/Yeachan-Heo/oh-my-codex/issues/888), patched in [#889](https://github.com/Yeachan-Heo/oh-my-codex/pull/889) together with a Dependabot setup).

## What I work on

- **AI product engineering:** pipeline design, model integration, evaluation and workflow automation.
- **AI for hardware data:** applying end-to-end AI pipelines to complex hardware data at SECA.
- **Developer tools for AI-assisted work:** practical tools, like agent-tree, that make agent sessions easier to review and resume.
- **Quantitative research:** applying AI to data-driven research and systematic experimentation.

## Get in touch

You can reach me on [LinkedIn](https://www.linkedin.com/in/seungwoo-dale-lee/) or by [email](mailto:lifrary2050@gmail.com). For agent-tree bugs and ideas, [open an issue](https://github.com/lifrary/agent-tree/issues).
