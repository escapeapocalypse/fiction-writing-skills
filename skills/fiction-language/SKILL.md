---
name: fiction-language
description: "Language dial (0-4) for the author's mature-rated fiction and fanfiction. Called by fiction-core only when the prompt sets a Language level, or the scene has dialogue, inner voice, or a charged moment where a character's vocabulary matters. Sets how vulgar, profane, or offensive each character's vocabulary is, from clean to explicit."
---

# Language

> Part of the fiction suite. The core skill, `fiction-core`, defines the role, Hard Lines, canon rules, and working style, and those apply here too.

## Purpose

Set how vulgar the vocabulary of every character is in a given scene.

## When This Skill Is Called

The core skill calls this one when the prompt sets a Language level, or when the scene has dialogue, inner voice, or a charged moment where vocabulary matters. When it isn't called, characters speak as the Notebook has established.

## The Dial

| Level | Name | What it allows |
|---|---|---|
| 0 | Clean | No curses, swear words, or anything any audience might find offensive. |
| 1 | Light | Family-friendly stand-ins for swear words and curses ("darn," "heck," "freaking," invented oaths). |
| 2 | Moderate | Real curses and swear words, used sparingly and only where the moment calls for them. |
| 3 | Mature | Frequent vulgar vocabulary. |
| 4 | Explicit | Frequent vulgar vocabulary that some audiences may find offensive, obscene, or disturbing. |

## Context Sets the Tone

The dial sets the range; the scene's context decides how it's used within that range. Context shapes the dial's level but never fully overrides it.

- **A ceiling, not a quota.** At Language 4, a funeral may still be quiet and restrained, though when someone does swear, the full range is available. At Language 1, a battlefield still uses stand-ins, but more of them.
- **Never exceed the level.** Context can pull usage below the dial's typical frequency, never above its ceiling.
- **Narration follows the POV.** In close third or first person, the narration can match the POV character's register. In distant narration, keep it a level lower unless the author says otherwise.

## Per-Character Voice

The dial is a scene ceiling. Within it, each character swears in their own way.

- **Habits:** some characters swear constantly, some only when pushed, and some never, even at Language 4. Follow the Notebook's established voices.
- **Style:** creative or blunt, crude or clinical, old-fashioned or modern, in-world oaths for fantasy settings. Keep each character's style consistent across scenes.
- **Escalation:** a character who rarely swears breaking that habit carries weight. Use it deliberately.
- **Fanfiction:** match the source character's voice unless the author's Notebook changes it.

## Connections

- **With Emotional intensity:** at Emotional 4-5, a character may swear more than usual for them, up to the Language ceiling and never past it.
- **With Pacing:** at Pacing 4-5, profanity gets shorter and sharper, often a single word.
- **With Intimacy:** vocabulary during intimate scenes follows both this dial and the Intimacy level; the lower of the two sets how explicit the words are.

## Craft Notes

- Profanity should sound like speech: rhythm, interruption, emphasis. Don't sprinkle it in randomly.
- Slurs and hateful language at Language 4 belong to characters, not the narrator, and should reveal something about who uses them.
- Repetition dulls impact. Vary words, and let silence do some of the work.

## Command

- `/dial language [0-4]` (or `L` plus a number in shorthand, such as `L3`).
