# Fiction Writing Suite

A set of five skills that turns an AI assistant into a scene-writing partner for mature-rated fiction and fanfiction (adult readers, 18+). You describe a scene, set a few dials for how it should feel, and the assistant writes it in your story's voice.

It's built for Gemini's skills feature and works best alongside a Notebook or other source material holding your story so far.

---

## How It Works

The suite has one **core** skill and four **companion** skills.

- The **core** reads every request, looks at your story's canon, and decides which companions the scene needs.
- The **companions** each handle one part of the writing: the setting, the language, the pacing, and the intensity.
- A companion is only used when the scene calls for it. A quiet conversation might use none of them. A chase might use pacing and action.

You don't pick the skills yourself. Describe the scene, add dials if you want control, and the core handles the rest.

---

## The Five Skills

| Skill | What it does | Dial |
|---|---|---|
| `fiction-core` | Routes requests, protects canon, sets the rules every scene follows | none |
| `fiction-scene-writing` | Builds vivid settings: place, atmosphere, how the surroundings shape the scene | none |
| `fiction-language` | Sets how vulgar each character's vocabulary is | Language, 0-4 |
| `fiction-pacing` | Sets how fast the scene moves and how urgent it feels | Pacing, 1-5 |
| `fiction-intensity` | Sets emotional and physical intensity | Emotional, Action, Intimacy, each 1-5 |

---

## Installing

1. Download the five zip files from the [`downloads`](downloads/) folder of this repo: `upload-fiction-core.zip`, `upload-fiction-scene-writing.zip`, `upload-fiction-language.zip`, `upload-fiction-pacing.zip`, and `upload-fiction-intensity.zip`. (Click a file, then the download button.)
2. In Gemini's skills section, upload each zip. Each one holds a single `SKILL.md` at its top level.
3. Upload all five. The companions depend on the core, and the core depends on them.
4. If you have older versions of these skills installed, delete them first.

Menu names vary by interface, so look for wherever your Gemini lets you add skills.

---

## Quick Start

Write a scene request in plain language, optionally adding dials at the end:

```
/scene Mara and Ilse argue in the burning chapel, L3 P4 E5 A2
```

That one line tells the assistant who is in the scene, where it happens, and how it should feel. Anything you leave out is filled in from your story's canon.

You can also skip the command and just ask:

> Write the scene where Mara finds the letter. Slow and quiet, but emotionally heavy.

---

## The Dials

Each dial is independent. A tender scene can be high on emotion and low on action. A fast scene can be calm in tone. Dials set the level; the scene's context decides how it plays out within that level.

### Language (L), 0 to 4

How vulgar each character's vocabulary is.

| Level | Name | What it means |
|---|---|---|
| 0 | Clean | No curses or swear words, nothing any audience might find offensive |
| 1 | Light | Family-friendly stand-ins ("darn," "heck," made-up oaths) |
| 2 | Moderate | Real curses, used sparingly and where the moment calls for them |
| 3 | Mature | Frequent vulgar vocabulary |
| 4 | Explicit | Frequent vulgar vocabulary some audiences may find offensive or obscene |

The scene's context shapes how the language is used but never goes past the level you set. Each character also keeps their own habits: some swear constantly, others never.

### Pacing (P), 1 to 5

How fast the scene moves and how urgent it feels.

| Level | Name | How it feels |
|---|---|---|
| 1 | No urgency | Slowest. A sense of safety, usually nothing at stake |
| 2 | Low urgency | Still slow, but with intrigue |
| 3 | Moderate urgency | Normal, leaning tense. Intrigue plus some anxiety |
| 4 | Heightened urgency | Fast and fluid. Intrigue, anxiety, and tension |
| 5 | Maximum urgency | Breakneck. Something major is on the line right now |

Pacing is about speed, not subject. A mundane scene can be Pacing 5, and a tense negotiation can be Pacing 1.

### Intensity: three separate dials

Intensity is split into three branches, each from 1 to 5. Use any, all, or none.

**Emotional (E)**: feelings and psychological weight, good or bad.

| Level | Name | What it means |
|---|---|---|
| 1 | None | No strong feelings present |
| 2 | Low | Some feelings, very faintly |
| 3 | Moderate | A range of feelings at a noticeable level |
| 4 | Heightened | Feelings considerably amplified |
| 5 | Maximum | Feelings pushed to the extreme |

**Action (A)**: fights, exertion, pain, and injury.

| Level | Name | What it means |
|---|---|---|
| 1 | None | No physical strain or conflict |
| 2 | Low | Light exertion or a brief scuffle |
| 3 | Moderate | A real fight or hard exertion, with consequences |
| 4 | Heightened | Brutal, sustained, with serious injury and exhaustion |
| 5 | Maximum | Extreme, relentless, life-or-death |

**Intimacy (I)**: intimate and sexual content. Adult characters only, at every level.

| Level | Name | What it means |
|---|---|---|
| 1 | None | No intimate contact on the page |
| 2 | Low | Light contact such as touch or a kiss; anything further happens off the page |
| 3 | Moderate | Sensual and suggestive; sex implied or written figuratively |
| 4 | Heightened | Explicit, with emphasis on sensation and emotion, some lyrical or euphemistic language |
| 5 | Maximum | Fully explicit, direct language |

### Setting (no dial)

The setting skill has no dial. It's used whenever a scene needs setting work, such as a new location, a change in time or weather, or a place you describe in the prompt. To ask for it directly, say something like "describe the setting in detail."

---

## Using the Dials

There are three ways to set dials.

**In the request (this scene only):**
```
/scene the chapel argument, L3 P4 E5
```

**For the whole session:**
```
/dial pacing 4
```

**Shorthand:** letter plus number, in any order: `L3 P5 E4 A4 I1`.

**Shifts within a scene:** an arrow makes a dial change as the scene goes.

```
P2→5       starts slow, builds to maximum urgency
E5→2       starts raw, cools down
P2→5 sudden    jumps rather than building gradually
```

A dial without an arrow holds steady.

**If you don't set a dial:** the assistant matches similar scenes in your story. If your story has none yet, it falls back on Language 2, Pacing 3, Emotional 3, and Action 2. Intimacy has no default: if a scene calls for it and you haven't set a level, the assistant asks once.

---

## Commands

Commands are shortcuts. Plain language works just as well.

| Command | What it does |
|---|---|
| `/scene [details] [dials]` | Write a scene |
| `/dial [dial] [level]` | Change a dial for the rest of the session |
| `/dials` | Show the current settings |
| `/reset` | Return to the defaults |
| `/continue` | Continue the last scene with the same voice and settings |
| `/rewrite [direction or dials]` | Rewrite the last scene, changing only what you ask (for example `/rewrite P2 E4`) |
| `/check` | Check a passage against your story's canon for continuity problems |
| `/canon` | List new canon decided this session, ready to add to your Notebook |
| `/route` | Show which skills were used for the last scene, and why |
| `/establish [place]` | Write a short passage that introduces a location |
| `/location [name]` | Build a location profile, ready to add to your Notebook |

---

## Examples

**A quiet, emotional scene:**
```
/scene Mara reads her brother's last letter alone in the kitchen, E5 P1 L0
```

**A fast fight:**
```
/scene Ilse and the guard fight on the rooftop in the rain, A4 P5 L3
```

**A scene that shifts:**
```
/scene The negotiation turns into an ambush, P2→5 E3→5 A1→4
```

**Fixing a miss:**
> That felt too rushed. Slow it down and let the grief land.

The assistant finds the setting most likely responsible (here, Pacing and Emotional), adjusts that, and tells you what it changed. It doesn't start over unless you ask.

---

## Tips

- **Start with the scene, then add dials.** You can run with no dials at all and tune from there.
- **Dial only what matters.** Setting two or three dials usually beats setting all five.
- **Feed it your story.** The better your Notebook, the better it matches names, voices, and world rules.
- **Check what happened.** If a scene feels off, `/route` shows which skills ran and at what levels.
- **Ask for rewrites by dial.** `/rewrite P2 E4` is faster than describing the change in words.

---

## What It Won't Do

This suite writes dark, violent, and adult fiction with craft. A few lines don't move at any dial level:

- No sexual content involving anyone under 18, or any character who reads as a child.
- No sexual or defamatory content about real people.
- No real-world instructions (weapons, drugs, hacking) dressed up as fiction.

Intimate content is for adult characters only. If a character's age isn't clear, the assistant asks first.

The platform you run this on has its own rules too. These skills shape tone and craft, but they can't change what the platform allows.

---

## Troubleshooting

**The uploader says SKILL.md is missing.** The file must sit at the top level of the zip, not inside a folder. Use the zips in `downloads` as they are, and don't re-zip the folders in `skills`.

**A skill doesn't seem to be used.** The core only calls a companion when the scene needs it. Set that skill's dial in your request, or ask for it in plain language.

**Dials seem ignored.** Run `/dials` to check the current settings, then `/route` to see what ran. Skills may not always be followed perfectly, so repeat a dial in the request if needed.

**The scene doesn't match your story.** Make sure your Notebook or source material is attached, and use `/check` to catch canon conflicts.

---

## Repository Layout

```
fiction-writing-skills/
├── README.md
├── LICENSE
├── skills/                  Readable source for each skill
│   ├── fiction-core/SKILL.md
│   ├── fiction-scene-writing/SKILL.md
│   ├── fiction-language/SKILL.md
│   ├── fiction-pacing/SKILL.md
│   └── fiction-intensity/SKILL.md
└── downloads/               Ready-to-upload zips (one per skill)
```

Edit a skill by changing its `SKILL.md` in `skills`. To upload it, zip that one file (with `SKILL.md` at the top level of the zip) or use the matching file in `downloads`.

---

## License

Released under the [MIT License](LICENSE). Use it, change it, and share it freely.
