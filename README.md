# Fiction Writing Suite

Turn Gemini into a scene-writing partner for mature fiction and fanfiction (adult readers, 18+). Describe a scene, set a few dials for how it should feel, and Gemini writes it in your story's voice.

## Quick Start

1. **[Download Writing-Assistant.zip]** and DON'T unzip it.
2. Open the **Skills** section in Gemini and drag in the ZIP file you just downloaded, and it should upload without issues and be ready for use!
3. Try it:

```
/scene Two old friends meet again at a train station, L2 P2 E4
```

## What's Inside

One core skill that routes your requests, plus six that each handle one part of a scene. Gemini only uses the ones a scene needs.

| Skill | Handles | Dial |
|---|---|---|
| `fiction-core` | Routing, canon, working rules | none |
| `fiction-scene-writing` | Settings and atmosphere | none |
| `fiction-language` | How vulgar the vocabulary is | `L` 0-4 |
| `fiction-pacing` | How fast and urgent the scene feels | `P` 1-5 |
| `fiction-intensity-emotional` | Emotional weight | `E` 1-5 |
| `fiction-intensity-action` | Fights, exertion, injury | `A` 1-5 |
| `fiction-intensity-intimacy` | Intimate content (adult characters only) | `I` 1-5 |

Set dials at the end of a request with a letter and a number, like `L3 P4 E5 A2 I1`. Add an arrow to change one mid-scene: `P2→5` starts slow and builds.

## Commands

`/scene` `/dial` `/dials` `/reset` `/continue` `/rewrite` `/check` `/canon` `/route` `/establish` `/location`

Plain language works too: "Write the scene where Mara finds the letter. Slow and quiet, but emotionally heavy."

## Limits

Intimate content is for adult characters only. No sexual content involving minors or real people, and no real-world weapon, drug, or hacking instructions. These apply at every dial level. The platform you run this on has its own rules too.

## Troubleshooting

**"SKILL.md is missing" when uploading?** Upload the small zips exactly as they are. Don't unzip them or re-zip a folder.

## More

The [full guide](GUIDE.md) lists every dial level and command. The [`skills`](skills/) folder has the readable source. Released under the [MIT License](LICENSE).
