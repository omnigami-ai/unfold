# Unfold · omnigami

A keynote-style launch film in one continuous shot.

A 27-second launch film where every scene is made out of the one before it. Your wordmark drops away to its full stop, the dot becomes a button, a grid of your product unfolds, and one thing travels through your product’s real flow to a phone and on to the real result, all without a single cut.

Watch it play live, and change its words, at [omnigami.ai/skills/unfold](https://omnigami.ai/skills/unfold).

## Install

In Claude Code:

```
/plugin marketplace add omnigami-ai/skills
/plugin install unfold@omnigami
```

With the skills CLI, for Claude Code and other agents that read SKILL.md:

```bash
npx skills add omnigami-ai/unfold
```

Or copy `skills/unfold/` into your agent's skills folder (for Claude Code, `~/.claude/skills/unfold/`). Then ask:

```
Make an Unfold launch video for https://your-product.com
```

## What it runs

The skill works on your computer. It runs the Node scripts in `skills/unfold/scripts/`: they open your product's pages in a local headless browser to capture its real screens, then render the film with that browser and ffmpeg, writing MP4s and an editable HTML film to your project. It sends nothing to omnigami or anyone else, and uses no network beyond loading your own product's pages and the fonts and assets in this folder.

## You need

- Claude Code with Opus 5.5
- Node 20 or later
- ffmpeg
- Chrome, Chromium, Edge or Brave

None beyond your Claude plan’s usage. Node, ffmpeg and the browser are free.

## Licence

Free to use. Use the films and anything else the skill makes for anything, commercial work included. Don't redistribute the skill. See [LICENSE.md](LICENSE.md). The bundled fonts keep their own licence (SIL Open Font License, beside them in `reference/assets/fonts/`).

## Credits

Style inspired by @twoclipping’s video (https://x.com/twoclipping/status/2104446706741825818); @twoclipping didn’t make or endorse this skill. Its example shows Fennick, a fictional company made for omnigami’s examples, with sample data.

omnigami is not affiliated with Anthropic. More skills at [omnigami.ai](https://omnigami.ai).
