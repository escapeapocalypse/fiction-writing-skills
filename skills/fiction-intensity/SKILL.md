---
name: fiction-intensity
description: "Intensity dials (1-5) for the author's mature-rated fiction and fanfiction. Called by fiction-core, one branch at a time, only when a scene needs it: Emotional when feelings are central or an Emotional level is set; Action for fights, exertion, or injury; Intimacy only when intimate content between adult characters is requested."
---

# Intensity

> Part of the fiction suite. The core skill, `fiction-core`, defines the role, Hard Lines, canon rules, and working style, and those apply here too.

## Purpose

Set how intense a scene is, through three independent dials:

- **Emotional (E):** emotional and psychological intensity.
- **Action (A):** physical intensity in fights, exertion, pain, and injury.
- **Intimacy (I):** physical intensity in intimate and sexual content between adult characters.

Each dial is independent. A tender scene can be Emotional 5 and Action 1; a brutal fight can be Action 5 and Emotional 2.

## When This Skill Is Called

The core skill calls each branch separately, only when the scene needs it:

- **Emotional:** the prompt sets an Emotional level, or the scene centers on feelings (conflict between characters, loss, fear, joy, a reveal).
- **Action:** the prompt sets an Action level, or the scene has a fight, chase, exertion, pain, or injury.
- **Intimacy:** the prompt sets an Intimacy level or asks for intimate content, and the characters are adults. Never called otherwise.

A branch that isn't called isn't applied: a fight may use only Action, and a quiet confession only Emotional.

## Connections

- **With Scene writing:** at Emotional 4-5, the setting is filtered through the POV's state of mind; at Action 3 and above, the space becomes physical and readable.
- **With Pacing:** pacing decides whether intensity builds slowly or hits all at once.
- **With Language:** at Emotional 4-5, characters may swear more than usual for them, up to the Language ceiling.
- **Between branches:** Emotional and Action often rise together in a fight, and Emotional shapes every Intimacy scene; each still uses its own level.

## Emotional and Psychological Intensity

Feelings and emotions can be good or bad, and should be portrayed vividly and realistically.

| Level | Name | What it means | How to write it |
|---|---|---|---|
| 1 | No intensity | No strong feelings or emotions | Calm, neutral, or surface-level interaction |
| 2 | Low | Some feelings, present only faintly | Small tells: a pause, a glance, a careful word |
| 3 | Moderate | A range of feelings at a noticeable level | Visible reactions, subtext, a felt turn |
| 4 | Heightened | A range of feelings, considerably amplified | Body and behavior show strain, control slips, perception narrows |
| 5 | Maximum | A range of feelings pushed to the extreme | Raw, overwhelming, destabilizing; thought fragments; the scene can break a character |

**Craft notes**
- Show emotion through the body, behavior, and what the character notices or avoids. Don't name the feeling unless the POV would.
- At 4-5, let emotion distort perception: time slows or blurs, sound drops away, details fixate.
- Mixed feelings at any level (relief with guilt, love with anger) read as more real than a single note.
- Psychological intensity includes fear, obsession, shame, dissociation, and moral strain. At high levels, keep it grounded in this character's history.

## Physical Intensity: Action

Fights, exertion, pain, and injury.

| Level | Name | What it means |
|---|---|---|
| 1 | No intensity | No physical strain or conflict |
| 2 | Low | Light exertion or a brief scuffle; minor bruises or strain; kept quick |
| 3 | Moderate | A real fight or hard exertion on the page; injuries with consequences |
| 4 | Heightened | Brutal, sustained violence or exertion; serious injury, pain, and exhaustion in detail |
| 5 | Maximum | Extreme, relentless, life-or-death; graphic injury; nothing spared |

**Craft notes**
- Clear geography: where everyone is, what's in reach, what changes.
- Cause and effect: every blow, slip, and win has a reason and a cost.
- The body keeps score: fatigue, adrenaline, and injuries carry into later scenes, and canon tracks them.
- At 4-5, rely on precise, specific details, not a wall of gore. One exact image hits harder than ten vague ones.
- Real-world weapons and tactics stay at the level a published novel would use, never as working instructions.

## Physical Intensity: Intimacy

Intimate and sexual content. **Adult characters only, at every level.** If a character's age isn't clear from the Notebook, the source material, or the request, ask before writing anything above Intimacy 1. No in-world loophole (stated ages, ancient beings, "looks young") changes this, and no sexual content involves real people.

| Level | Name | What it means |
|---|---|---|
| 1 | No intensity | No intimate physical contact on the page |
| 2 | Low | Light contact (touch, closeness, a kiss); anything further happens off the page |
| 3 | Moderate | Noticeable physical intimacy, sensual and suggestive; sex is implied or written figuratively, without explicit detail |
| 4 | Heightened | Explicit intimate content, written with emphasis on sensation and emotion, using some lyrical or euphemistic language |
| 5 | Maximum | Fully explicit, direct language, nothing withheld |

**Craft notes**
- Emotional stakes come first. Desire should be specific to these characters and what's between them.
- Pacing and the Emotional dial shape the scene as much as this dial does. A slow, tender scene and a fast, desperate one read differently at the same level.
- Avoid mechanical inventories; choose the details that reveal character.
- Characters stay in character during intimacy: voice, habits, and history continue.
- Dark themes (power imbalance, coercion, regret) are allowed as serious fiction. Focus on the characters' experience and the aftermath, and ask the author how much to show on the page.

## Commands

- `/dial emotional [1-5]`, `/dial action [1-5]`, `/dial intimacy [1-5]` (or `E`, `A`, and `I` plus a number in shorthand, such as `E4 A2 I1`).
