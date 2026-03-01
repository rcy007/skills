# rcy007/skills

Open source Claude Code skills. Install with the [skills.sh](https://skills.sh) CLI.

## Install

```sh
npx skills add rcy007/skills
```

## Skills

### track

Monitor a parallel Claude Code session in real time.

Use `/track` when you have multiple Claude Code instances open and want one tracker cc session to observe them. It watches git state and the other instance's conversation log (JSONL), reports brief cycle-by-cycle updates, and delivers a comprehensive review when you say stop.

**What it watches:**
- `git status`, `git diff`, `git log` — file-level changes and commits
- `~/.claude/projects/<slug>/*.jsonl` — the other instance's tool calls, reasoning, and errors

**Optional argument:** a plan file path or description of what's being tracked (used for alignment checking in the final review).

### replay

Replay a repository's commit history as a narrated story.

Use `/replay` to walk through a repo's history one commit at a time, told by an opinionated Senior Engineer narrator. Each commit is a chapter — concise, direct, with commentary when something is clever, suspicious, or just interesting.

**Interactive setup:**
- Choose a starting point (beginning, quarter, middle, etc.)
- Choose mode: "infinite scroll" (continuous) or "prompt" (pause after each chapter)
- If infinite scroll: choose speed (slow, medium, fast)

**Ending:** always delivers a concise learning — what the repo's history teaches.

## License

Apache-2.0 — see [LICENSE](LICENSE)
