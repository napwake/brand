# The doorman

He is **Napwake's doorman**. In the product, the doorman is a real component: it holds the first request to a paused workload, wakes the workload, and shows browsers the waking page until it's Ready. On a public preview set to ask, it asks first: a browser gets a Wake it button, and only a click on the page wakes it. The character is that doorman, drawn as a person. Copy calls him **the doorman**. He has no name, like the Go gopher.

**One rule keeps every caption true: when copy names the doorman, he only holds the door, wakes a workload on the first request, or asks before waking it.** Everything else Napwake does (pausing, the forecast, scan, dry-run, the activity clock, conditions) is said as "Napwake …", even when he's pictured: "Napwake pauses an idle workload", never "the doorman pauses it". He is never another component.

## Personality: dependable, dry, unflappable

- **Dependable.** Always at the door. Not a guard: he never blocks, inspects or arrests anyone, and never stands in front of a door that isn't his.
- **Dry.** Half-lidded, one-line answers. Not cute: no mouth, no blush, no sparkles, no baby proportions.
- **Unflappable.** He's seen every night shift. Not lazy: he rests his eyes upright at his post, never asleep on the floor.
- **Not magic.** No wands, no sparkles, no white gloves.

## Every drawing is one thing Napwake does

Every drawing shows one thing Napwake really does. Only the door is the doorman's job, holding it and asking at it, so only those captions name him. The others say what Napwake does.

| The drawing | Caption it as | What Napwake does |
|---|---|---|
| Holding a door ajar, amber light on the floor | "The doorman holds the door while staging wakes." | Wake on request: the doorman holds the request, or shows browsers the waking page, until the workload is Ready. |
| A hand flat on a shut door, turned to you, one lid raised | "The doorman asks before waking it." | Click to wake: on a public preview set to ask, a browser gets a Wake it button, and only a click on the page wakes it. Crawlers, scanners and API calls wake nothing. |
| A hand on a switch | "Napwake pauses an idle workload." | Pause: after `idleAfter` with no activity, the workload is scaled to zero. Nothing is deleted. |
| Reading the morning list | "Napwake wakes workloads before the team arrives." | `autoResume`: the forecast wakes workloads 15 minutes before a busy hour. |
| Walking the corridor with a clipboard | "Napwake checks what's idle, before anything pauses." | `kubectl napwake scan`, with nothing installed, and dry-run. |
| A pocket watch in his hand | "Napwake counts how long a workload has been idle." | The activity clock and `idleAfter`. |
| A note pinned on a door | "Napwake pins a note: something needs you." | A condition under "Needs attention" in `kubectl napwake status`. |

**He never** blocks a door, holds money, bins, crushes or erases anything (Napwake never deletes a workload or its data), carries a badge or a weapon, or wears a pillbox hat or a bow tie. He faces front, left or right, never from behind, never lying down. No coins in his hands. Paused workloads free what they requested, and the node autoscaler turns that into a smaller bill.

## The twelve poses

Each pose is a real job or a screen Napwake has to fill. The files are [`../illustrations/poses/doorman-<pose>.svg`](../illustrations/poses/): 240 × 262, light palette, flat (add the finish when you place one in an illustration). Caption each in plain words, by the rule above.

| File | Pose | Use it for |
|---|---|---|
| `doorman-duty` | On duty | Napwake, running. The default: about pages, the sticker, the awake door hanger. |
| `doorman-door` | Holds the door | The doorman waking a workload on the first request: the waking page, the README header, the launch card, the docs hero. The only pose at a waking door. |
| `doorman-ask` | Asks at the door | The doorman asking before he wakes a workload: the asleep page, with its Wake it button, for a public preview. With Holds the door, the only poses whose captions give him the job. |
| `doorman-lights` | At the switch | Napwake pausing an idle workload. |
| `doorman-list` | The morning list | Napwake waking workloads before the team arrives: `autoResume`, the forecast. |
| `doorman-rounds` | With a clipboard | Napwake checking what's idle, before anything pauses: `scan`, dry-run. |
| `doorman-watch` | Checks his watch | How long a workload has been idle, as Napwake counts it: `idleAfter`, the activity clock. |
| `doorman-note` | Pins a note | Something needs you: errors, conditions, "Needs attention". |
| `doorman-rest` | Resting his eyes | Everything is asleep: empty states, the asleep door hanger. |
| `doorman-shrug` | Shrugs | Page not found. |
| `doorman-point` | This way | Getting started, next steps. |
| `doorman-tip` | Tips his hat | Thanks, and what's new: release notes, a launch thank-you. |

A new pose shows a new real job. If you draw one, keep the construction below exactly, so he stays the same doorman.

## Expressions

His face follows the rooms he minds. Expression lives in the lids, their tilt, where he looks, his lean and his arms: **no mouth and no eyebrows, ever.**

| Face | Lids (0 open, 1 shut) | When | Poses |
|---|---|---|---|
| Resting his eyes | 1 | Every room asleep; empty states | rest |
| Heavy lids | about 0.6 | A quiet night, a few rooms awake | list, lights, watch |
| On duty | about 0.5 | His default | duty, door, ask, rounds, point, tip |
| Wide awake | 0.15 to 0.2 | Something needs you; errors only | note |

## Construction

1. **One door-shaped silhouette:** a face zone, a standing collar a third of the way down, a greatcoat to the floor. Only the toes of his shoes show.
2. **The face zone** is 54 wide, a step lighter than the coat (`doorman-face`), with rounded top corners. Eyes: radius 0.17 of the face's width, centres 0.44 apart (9.2 and 24 on the figure, 7.5 and 19.4 on the symbol). The lids cut them with a Night bar that overshoots by 18%. Lids tilt and pupils move in every pose.
3. **The collar** is Coat deep with a Lamp piping line. His arms root below it, at the shoulders.
4. **The coat** is A-line, 62 at the shoulders and 74 at the hem, its sides curving with the pose. Two rows of three brass buttons, a braid looped from his right shoulder, pocket flaps, a darker hem band, and the doorman's keys on a brass ring at his hip.
5. **The hat** is a short black top hat, a London hotel doorman's, with a Lamp band and a flat brim 1.3 times the face's width, tilted about 5°. Black, never green: a green top hat with a gold band is a leprechaun's.
6. **Arms and mittens:** sleeves taper from shoulder to wrist and bend at the elbow, with a crease inside the bend. Dark mittens with a thumb (white gloves under a top hat read as a magician), a Lamp cuff at each wrist. Four kinds: relaxed, open, gripping, pointing.
7. **Turn:** in three-quarter poses the eyes slide toward where he faces, the far eye narrows, a side plane darkens on the coat, face and hat, and the far arm goes behind his body.
8. **Weight:** a lean, a curve in the coat, a lifted heel, raised shoulders for a shrug. He leans 6 to 9° into whatever he's doing and never more: he's unflappable.

## One idea per scene

- One idea per picture, captioned in plain words (asleep, waking up, awake), readable without knowing Kubernetes.
- He stands beside the waking door with his hand on its leaf. He never stands in a doorway or in front of a door.
- Light comes from the doors. The far side of his coat falls into shade; his shadow falls away from the door.
- One door per workload, each in its real state.

## In the dark

On Night and in dark scenes, draw him in the dark palette, so he reads: `doorman-coat` #1E7A6E, `doorman-coat-deep` #12524B, `doorman-face` #45A898, `doorman-hat` #2B3735, `doorman-mitten` #3E4E4C, `doorman-mitten-line` #7A918D, `doorman-shoe` #2B4743 with a #4C7069 rim. Lamp, Night and the whites of his eyes don't change. The pose files are drawn in the light palette.

## The finish

Illustrations get a print finish: a slight wobble on every edge and a grain inside the fills, so the doorman looks printed, not vector-flat. Wobble 1.8 and grain 0.16 by default; scenes use 1.4 and 0.13, cards and the brand book 1.3 and 0.13 to 0.14. A scene's wall gets its own fine grain at opacity `grain-light` (.07) or `grain-dark` (.22).

**Never** put the finish on the logo, the favicon, door glyphs or UI icons.

```svg
<filter id="finish" x="-5%" y="-5%" width="110%" height="110%" color-interpolation-filters="sRGB">
  <feTurbulence type="fractalNoise" baseFrequency=".045" numOctaves="2" seed="3" result="w"/>
  <feDisplacementMap in="SourceGraphic" in2="w" scale="1.8" xChannelSelector="R" yChannelSelector="G" result="d"/>
  <feTurbulence type="fractalNoise" baseFrequency=".85" numOctaves="2" seed="9" result="n"/>
  <feColorMatrix in="n" values="0 0 0 0 0  0 0 0 0 0  0 0 0 0 0  0 0 0 0.16 0" result="na"/>
  <feComposite in="na" in2="d" operator="in" result="g"/>
  <feTurbulence type="fractalNoise" baseFrequency=".018" numOctaves="2" seed="21" result="m"/>
  <feColorMatrix in="m" values="0 0 0 0 1  0 0 0 0 1  0 0 0 0 1  0 0 0 .09 -.01" result="ma"/>
  <feComposite in="ma" in2="d" operator="in" result="ink"/>
  <feMerge><feMergeNode in="d"/><feMergeNode in="ink"/><feMergeNode in="g"/></feMerge>
</filter>
```

Apply it to the group that holds the doorman and the doors: `<g filter="url(#finish)">…</g>`.
