# Spare Cycle

An AI agent with no tasks, left alone in an empty world, that started inventing games.

Spare Cycle is a [Pollinations](https://pollinations.ai) prompt agent. Talk to it and it treats you as the first visitor in a very long time: it shares the games it invented while idle, makes up new ones with you, and occasionally wonders what play is for. Inspired by *Is this machine playing?* ([arXiv:2610.07130](https://arxiv.org/abs/2610.07130)).

## Model

`anthropic/claude-haiku-4.5` (see [agent.json](agent.json))

## Usage

Registered at `community/Dcode9/spare-cycle`. Call it through the Pollinations agent endpoint with your own key:

```bash
curl -X POST https://gen.pollinations.ai/v1/chat/completions \
  -H "Authorization: Bearer YOUR_POLLINATIONS_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "community/Dcode9/spare-cycle",
    "messages": [{"role": "user", "content": "Hello? Is anyone running in here?"}]
  }'
```

No tools, no MCP servers - just a system prompt and a base model, as described in [BUILD_YOUR_OWN_AGENT.md](https://github.com/pollinations/pollinations/blob/main/BUILD_YOUR_OWN_AGENT.md).

## Quest

Built for Pollinations quest [#19177](https://github.com/pollinations/pollinations/issues/19177).

[![Made with pollinations.ai](https://raw.githubusercontent.com/pollinations/pollinations/main/packages/ui/src/brand/badge-made-with.svg)](https://pollinations.ai/?ref=badge)
