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

I fix the reliability bugs I hit in the AI developer tools I use every day: orphaned processes, crashes, silent failures and lost data. 36 of my changes have been merged into 14 projects with <b>more than 200,000 stars</b> combined.

<table>
<tr>
<th width="120">Stars</th>
<th width="180" align="left">Project</th>
<th width="70">PRs</th>
<th width="476" align="left">Contribution</th>
</tr>
<tr>
<td width="120" align="center" valign="middle"><a href="https://github.com/code-yeongyu/oh-my-openagent"><img src="https://img.shields.io/github/stars/code-yeongyu/oh-my-openagent?style=for-the-badge&logo=github&logoColor=white&label=&labelColor=24292f&color=e3b341" alt="oh-my-openagent stars"></a></td>
<td width="180" nowrap valign="middle"><a href="https://github.com/code-yeongyu/oh-my-openagent"><b>oh-my-openagent</b></a><br><sub>code-yeongyu</sub></td>
<td width="70" align="center" valign="middle"><b>1</b><br><sub><a href="https://github.com/code-yeongyu/oh-my-openagent/pull/7525">#7525</a></sub></td>
<td width="476" valign="middle">Stopped abandoned stdio MCP servers from running forever: the idle timeout never closed stdin, so they could not exit. Reported the bug and wrote the fix.</td>
</tr>
<tr>
<td width="120" align="center" valign="middle"><a href="https://github.com/Yeachan-Heo/oh-my-claudecode"><img src="https://img.shields.io/github/stars/Yeachan-Heo/oh-my-claudecode?style=for-the-badge&logo=github&logoColor=white&label=&labelColor=24292f&color=e3b341" alt="oh-my-claudecode stars"></a></td>
<td width="180" nowrap valign="middle"><a href="https://github.com/Yeachan-Heo/oh-my-claudecode"><b>oh-my-claudecode</b></a><br><sub>Yeachan-Heo</sub></td>
<td width="70" align="center" valign="middle"><b>9</b><br><sub><a href="https://github.com/Yeachan-Heo/oh-my-claudecode/pull/1843">#1843</a><br><a href="https://github.com/Yeachan-Heo/oh-my-claudecode/pull/1480">#1480</a><br><a href="https://github.com/Yeachan-Heo/oh-my-claudecode/pull/1482">#1482</a></sub></td>
<td width="476" valign="middle">Unified 8 divergent process-liveness checks, 5 of which mistook live processes for dead ones on <code>EPERM</code>, and wired stop-hook safeguards into the scripts that actually run instead of code that was never invoked.</td>
</tr>
<tr>
<td width="120" align="center" valign="middle"><a href="https://github.com/Yeachan-Heo/oh-my-codex"><img src="https://img.shields.io/github/stars/Yeachan-Heo/oh-my-codex?style=for-the-badge&logo=github&logoColor=white&label=&labelColor=24292f&color=e3b341" alt="oh-my-codex stars"></a></td>
<td width="180" nowrap valign="middle"><a href="https://github.com/Yeachan-Heo/oh-my-codex"><b>oh-my-codex</b></a><br><sub>Yeachan-Heo</sub></td>
<td width="70" align="center" valign="middle"><b>6</b><br><sub><a href="https://github.com/Yeachan-Heo/oh-my-codex/pull/1605">#1605</a><br><a href="https://github.com/Yeachan-Heo/oh-my-codex/pull/1918">#1918</a><br><a href="https://github.com/Yeachan-Heo/oh-my-codex/pull/1303">#1303</a></sub></td>
<td width="476" valign="middle">Prevented orphaned <code>codex</code> processes when tmux kills a session, kept the HUD and dispatch loop alive through partial writes, and made failed state writes fail loudly instead of reporting success. Also reported three high-severity dependency vulnerabilities, since patched.</td>
</tr>
<tr>
<td width="120" align="center" valign="middle"><a href="https://github.com/manaflow-ai/cmux"><img src="https://img.shields.io/github/stars/manaflow-ai/cmux?style=for-the-badge&logo=github&logoColor=white&label=&labelColor=24292f&color=e3b341" alt="cmux stars"></a></td>
<td width="180" nowrap valign="middle"><a href="https://github.com/manaflow-ai/cmux"><b>cmux</b></a><br><sub>manaflow-ai</sub></td>
<td width="70" align="center" valign="middle"><b>1</b><br><sub><a href="https://github.com/manaflow-ai/cmux/pull/1834">#1834</a></sub></td>
<td width="476" valign="middle">Removed force-unwraps from file-write paths, switching to UTF-8 conversions that cannot fail.</td>
</tr>
<tr>
<td width="120" align="center" valign="middle"><a href="https://github.com/andrewyng/openworker"><img src="https://img.shields.io/github/stars/andrewyng/openworker?style=for-the-badge&logo=github&logoColor=white&label=&labelColor=24292f&color=e3b341" alt="openworker stars"></a></td>
<td width="180" nowrap valign="middle"><a href="https://github.com/andrewyng/openworker"><b>openworker</b></a><br><sub>andrewyng</sub></td>
<td width="70" align="center" valign="middle"><b>1</b><br><sub><a href="https://github.com/andrewyng/openworker/pull/70">#70</a></sub></td>
<td width="476" valign="middle">Made conversation-log rewrites atomic, closing a window where a crash during context compaction could wipe the history.</td>
</tr>
<tr>
<td width="120" align="center" valign="middle"><a href="https://github.com/lidge-jun/opencodex"><img src="https://img.shields.io/github/stars/lidge-jun/opencodex?style=for-the-badge&logo=github&logoColor=white&label=&labelColor=24292f&color=e3b341" alt="opencodex stars"></a></td>
<td width="180" nowrap valign="middle"><a href="https://github.com/lidge-jun/opencodex"><b>opencodex</b></a><br><sub>lidge-jun</sub></td>
<td width="70" align="center" valign="middle"><b>2</b><br><sub><a href="https://github.com/lidge-jun/opencodex/pull/3097">#3097</a><br><a href="https://github.com/lidge-jun/opencodex/pull/3137">#3137</a></sub></td>
<td width="476" valign="middle">Capped the response spill directory, which was unbounded and could fill a disk within an hour, and fixed tests that failed whenever pid 4242 happened to be in use.</td>
</tr>
<tr>
<td width="120" align="center" valign="middle"><a href="https://github.com/pymupdf/PyMuPDF"><img src="https://img.shields.io/github/stars/pymupdf/PyMuPDF?style=for-the-badge&logo=github&logoColor=white&label=&labelColor=24292f&color=e3b341" alt="PyMuPDF stars"></a></td>
<td width="180" nowrap valign="middle"><a href="https://github.com/pymupdf/PyMuPDF"><b>PyMuPDF</b></a><br><sub>pymupdf</sub></td>
<td width="70" align="center" valign="middle"><b>1</b><br><sub><a href="https://github.com/pymupdf/PyMuPDF/pull/5139">#5139</a></sub></td>
<td width="476" valign="middle">Turned a hard segfault in the C++ bindings into a reported error: an exception in a <code>get_cdrawings()</code> callback used to crash the process, and extraction now carries on.</td>
</tr>
<tr>
<td width="120" align="center" valign="middle"><a href="https://github.com/Q00/ouroboros"><img src="https://img.shields.io/github/stars/Q00/ouroboros?style=for-the-badge&logo=github&logoColor=white&label=&labelColor=24292f&color=e3b341" alt="ouroboros stars"></a></td>
<td width="180" nowrap valign="middle"><a href="https://github.com/Q00/ouroboros"><b>ouroboros</b></a><br><sub>Q00</sub></td>
<td width="70" align="center" valign="middle"><b>3</b><br><sub><a href="https://github.com/Q00/ouroboros/pull/1152">#1152</a><br><a href="https://github.com/Q00/ouroboros/pull/325">#325</a><br><a href="https://github.com/Q00/ouroboros/pull/154">#154</a></sub></td>
<td width="476" valign="middle">Stopped the welcome suggestion from reappearing in every session for already-configured users, fixed a crash on <code>null</code> MCP parameters, and narrowed 30 bare <code>except Exception</code> clauses that could hide real bugs.</td>
</tr>
<tr>
<td width="120" align="center" valign="middle"><a href="https://github.com/Yeachan-Heo/gajae-code"><img src="https://img.shields.io/github/stars/Yeachan-Heo/gajae-code?style=for-the-badge&logo=github&logoColor=white&label=&labelColor=24292f&color=e3b341" alt="gajae-code stars"></a></td>
<td width="180" nowrap valign="middle"><a href="https://github.com/Yeachan-Heo/gajae-code"><b>gajae-code</b></a><br><sub>Yeachan-Heo</sub></td>
<td width="70" align="center" valign="middle"><b>6</b><br><sub><a href="https://github.com/Yeachan-Heo/gajae-code/pull/5422">#5422</a><br><a href="https://github.com/Yeachan-Heo/gajae-code/pull/6260">#6260</a><br><a href="https://github.com/Yeachan-Heo/gajae-code/pull/6333">#6333</a></sub></td>
<td width="476" valign="middle">Made quota failover mark the account that actually ran out, recovered OAuth tokens rejected before expiry that left quota readings stale, and stopped queued requests from receiving another run's answer. Also reported a rate limit hidden behind a generic stream timeout, since fixed.</td>
</tr>
<tr>
<td width="120" align="center" valign="middle"><a href="https://github.com/first-fluke/oh-my-agent"><img src="https://img.shields.io/github/stars/first-fluke/oh-my-agent?style=for-the-badge&logo=github&logoColor=white&label=&labelColor=24292f&color=e3b341" alt="oh-my-agent stars"></a></td>
<td width="180" nowrap valign="middle"><a href="https://github.com/first-fluke/oh-my-agent"><b>oh-my-agent</b></a><br><sub>first-fluke</sub></td>
<td width="70" align="center" valign="middle"><b>1</b><br><sub><a href="https://github.com/first-fluke/oh-my-agent/pull/265">#265</a></sub></td>
<td width="476" valign="middle">Fixed an SQL-injection check that had never actually run: broken shell quoting made it pass every input, including real injection patterns.</td>
</tr>
<tr>
<td width="120" align="center" valign="middle"><a href="https://github.com/dragon1086/prism-insight"><img src="https://img.shields.io/github/stars/dragon1086/prism-insight?style=for-the-badge&logo=github&logoColor=white&label=&labelColor=24292f&color=e3b341" alt="prism-insight stars"></a></td>
<td width="180" nowrap valign="middle"><a href="https://github.com/dragon1086/prism-insight"><b>prism-insight</b></a><br><sub>dragon1086</sub></td>
<td width="70" align="center" valign="middle"><b>1</b><br><sub><a href="https://github.com/dragon1086/prism-insight/pull/227">#227</a></sub></td>
<td width="476" valign="middle">Fixed a module-cache collision that crashed the US stock analysis pipeline with import errors.</td>
</tr>
<tr>
<td width="120" align="center" valign="middle"><a href="https://github.com/charlietlamb/openlogs"><img src="https://img.shields.io/github/stars/charlietlamb/openlogs?style=for-the-badge&logo=github&logoColor=white&label=&labelColor=24292f&color=e3b341" alt="openlogs stars"></a></td>
<td width="180" nowrap valign="middle"><a href="https://github.com/charlietlamb/openlogs"><b>openlogs</b></a><br><sub>charlietlamb</sub></td>
<td width="70" align="center" valign="middle"><b>1</b><br><sub><a href="https://github.com/charlietlamb/openlogs/pull/3">#3</a></sub></td>
<td width="476" valign="middle">Added a pre-publish gate, so a failing test suite can no longer ship a broken package to npm.</td>
</tr>
<tr>
<td width="120" align="center" valign="middle"><a href="https://github.com/seojoonkim/memkraft"><img src="https://img.shields.io/github/stars/seojoonkim/memkraft?style=for-the-badge&logo=github&logoColor=white&label=&labelColor=24292f&color=e3b341" alt="memkraft stars"></a></td>
<td width="180" nowrap valign="middle"><a href="https://github.com/seojoonkim/memkraft"><b>memkraft</b></a><br><sub>seojoonkim</sub></td>
<td width="70" align="center" valign="middle"><b>2</b><br><sub><a href="https://github.com/seojoonkim/memkraft/pull/3">#3</a><br><a href="https://github.com/seojoonkim/memkraft/pull/2">#2</a></sub></td>
<td width="476" valign="middle">Fixed <code>recall</code> reporting every stored entity as missing, so agents see their stored memories again, and made <code>track()</code> return the path it creates.</td>
</tr>
<tr>
<td width="120" align="center" valign="middle"><a href="https://github.com/subinium/agf"><img src="https://img.shields.io/github/stars/subinium/agf?style=for-the-badge&logo=github&logoColor=white&label=&labelColor=24292f&color=e3b341" alt="agf stars"></a></td>
<td width="180" nowrap valign="middle"><a href="https://github.com/subinium/agf"><b>agf</b></a><br><sub>subinium</sub></td>
<td width="70" align="center" valign="middle"><b>1</b><br><sub><a href="https://github.com/subinium/agf/pull/1">#1</a></sub></td>
<td width="476" valign="middle">Removed duplicated path helpers from the delete command, so it resolves the Claude and Codex directories through the shared config code.</td>
</tr>
</table>

## What I work on

- **AI product engineering:** pipeline design, model integration, evaluation and workflow automation.
- **AI for hardware data:** applying end-to-end AI pipelines to complex hardware data at SECA.
- **Developer tools for AI-assisted work:** practical tools, like agent-tree, that make agent sessions easier to review and resume.
- **Quantitative research:** applying AI to data-driven research and systematic experimentation.

## Get in touch

You can reach me on [LinkedIn](https://www.linkedin.com/in/seungwoo-dale-lee/) or by [email](mailto:lifrary2050@gmail.com). For agent-tree bugs and ideas, [open an issue](https://github.com/lifrary/agent-tree/issues).
