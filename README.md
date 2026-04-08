# HyperDev Plugins for Claude Code

Official plugin marketplace by [HyperDev](https://gohyperdev.com) — lightweight, Rust-based tools for Claude Code multi-agent workflows.

## Install

Add the marketplace:

```
/plugin marketplace add gohyperdev/hyperdev-claude-plugins
```

## Available Plugins

### hdcd-telegram

Rust-based Telegram channel for Claude Code. Drop-in replacement for the official Bun-based plugin.

- 3.5 MB binary vs ~100 MB Bun runtime
- ~5 MB RAM vs ~100 MB per instance
- <50 ms startup vs 2-3 seconds
- Clean shutdown — no zombie 409 Conflict
- Full feature parity + voice transcription via Whisper

**Install:**
```
/plugin install hdcd-telegram@hyperdev-plugins
```

**Setup:**
```
/hdcd-telegram:configure <your-bot-token>
```

**Launch:**
```bash
claude --channels plugin:hdcd-telegram@hyperdev-plugins
```

For full documentation see [hdcd-telegram](https://github.com/gohyperdev/hdcd-telegram).

## License

Apache-2.0
