# Napwake brand guidelines

Napwake pauses idle Kubernetes workloads in staging, preview and dev, and wakes them on the first request. It never deletes a workload or its data. It's open source (Apache 2.0): an operator, a `kubectl napwake` plugin, a Helm chart, and docs at napwake.dev.

It's for platform and infrastructure engineers who run non-production environments on their own Kubernetes clusters, behind a VPN, SSO or an IP allowlist. Environments open to the internet get woken by crawlers, so Napwake isn't for them.

**The headline:** Non-prod environments that sleep when nobody's using them, and wake when someone does.

**The plain line,** under the headline everywhere, and alone where space is short (GitHub About, Artifact Hub): Pauses idle Kubernetes workloads in staging, preview and dev, and wakes them on the first request.

## The idea

Napwake is **the night porter** of your non-production cluster: he lets the rooms nobody's using sleep, holds the door for the first request, and wakes the right room. Every room is an arched door. Shut and dark is asleep; ajar with amber light is waking up; open and lit green is awake. Anyone reads it at a glance, Kubernetes or not, so every picture carries one idea in plain words.

Before you make anything, read the section for it:

- **[The logo](logo.md):** the one logo, its approved versions, clear space, minimum sizes, misuses.
- **[The night porter](night-porter.md):** how he's built, his eleven poses and when to use each, what he does and never does, the finish.
- **[Using the brand](using-the-brand.md):** talks, posts, slides and community projects.

## Voice

Everything Napwake says follows six rules.

1. **Say what it does, in the reader's words.** Not "Intelligent Kubernetes workload lifecycle management"; "Pauses idle staging workloads and wakes them on the first request."
2. **A terminal snippet over an adjective.** Not "Effortless setup"; "`kubectl napwake scan` shows what's idle, with nothing installed."
3. **Every number carries its source or its assumption.** Not "Workloads sit idle 60-80% of the time"; "A team that works 10 hours a day, five days a week, uses staging 50 of 168 hours. The other 70%, it's idle."
4. **Say what it won't do.** "It never deletes a workload or its data." "Environments open to the internet get woken by crawlers; put them behind a VPN or SSO."
5. **Name the alternatives fairly.** Headlines, the README and launch posts lead with what Napwake does best and never claim what it doesn't do. Comparison pages and replies say plainly when another tool fits better: "Want everything off at 8pm whatever happens? kube-green does that well."
6. **Calm, not cute.** No "magic", "seamless" or "intelligent"; no exclamation marks or emoji in the docs; the sleep metaphor once per page, not in every line. Not "Put your cluster to sleep and watch the savings roll in!"; "Paused workloads free the CPU and memory they requested; your node autoscaler turns that into a smaller bill."

**The number** is arithmetic with its assumption, never a percentage on its own: "A team that works 10 hours a day, five days a week, uses staging 50 of 168 hours. The other 70%, it's idle. `kubectl napwake scan` shows your cluster's own number before you install anything."

**His register** is short, dry, and plain about what happens and what doesn't:

> This environment was paused while nobody was using it. It's starting now, and this page opens it on its own when it's ready. (the waking page)

> Your first request waits at the door while the workload starts. Usually that's a slow response, not an error; the docs say when it isn't. (README)

> Staging sleeps. The night porter doesn't. (the sticker: true of Napwake, whose operator and doorman keep running while workloads are paused)

**Words.** Say "pause idle" and "sleep" and "wake": the words users use. Don't call Napwake "scale to zero" or "hibernate"; in Kubernetes those mean other things. Write "Napwake" in text, `napwake` in commands; the wordmark is lowercase. Headings in sentence case. Dates absolute.

## Two vocabularies

| State | In pictures and pages anyone reads | In the CLI and reference docs | Its door |
|---|---|---|---|
| asleep | asleep | paused | shut and dark, a slate leaf, a brass knob |
| waking | waking up | resuming | ajar, amber room light and a wedge on the floor, the porter's hand on it |
| awake | awake | running | wide open, the room lit green, a green lamp over it |
| error | needs you | needs attention | shut, a note pinned on it |

- Use the plain words in scenes, captions, the waking page, launch posts and swag.
- Use the product words in `kubectl napwake` output, reference docs, API fields and anything a user types or searches for.
- Where both appear, plain first: "Asleep · paused".
- The character is **the night porter**. The doorman is a real Napwake component, the Service-level proxy that holds requests; never call the porter the doorman, and never say he is a Deployment.

## Doors as states

- Every room is an arched door: round top, flat bottom, the same arch as the wordmark's counters.
- Asleep: shut, slate (`glyph-slate`, `scene-leaf`). Waking up: ajar, the room in Lamp light (`scene-room-amber`), an amber wedge on the floor, and the only door with the porter's hand on it. Awake: wide open, the room lit green (`scene-room-green`), a green lamp over the door (`scene-green`). Needs you: shut, a note pinned on it (`note-pin`); a note, never an alarm bell, and it says what to fix.
- Use the door glyphs in [`../illustrations/doors/`](../illustrations/doors/) (`door-<state>.svg` on light, `door-<state>-dark.svg` on dark).
- Always put the state's word beside its door. Colour is never the only signal: waking's amber outline is 1.71:1 on Paper, and awake and error are equally light.
- His face follows the rooms he minds: resting his eyes when every room is asleep, heavy lids on a quiet night, on duty by default, wide awake only when something needs you.
- In a scene, show one door per workload, each in its real state.

## Colour

A night porter's coat, the light from a door, and the dark corridor.

- **Coat** `coat` #14695F is the brand's teal. **Lamp** `lamp` #F5B53F is the warm light. **Night** `night` #0F1716 and **Paper** `paper` #F8F8F5 are dark and light. **Coat deep** `coat-deep`, **Face** `face`, **Hat** `hat` and **Mitten** `mitten` belong to the porter.
- Pages: `bg` for the page, `surface` for raised cards, `text` for copy, `muted` for secondary text, `line` for hairlines. Set body copy in `text` on `bg` or `surface`.
- Actions: `action` (Coat on light, Lamp on dark) for links, buttons and the focus ring. Text on an action fill is `on-action` (Paper on Coat, Night on Lamp), never plain white.
- Lamp is a fill on light, never text (1.71:1 on Paper). Amber text on light is `accent-text` #8A5A00.
- State words take `asleep`, `waking`, `awake` and `error`. Use them for states only, never for decoration.
- The porter has his own tokens (`porter-*`), lighter in dark so he reads on Night. Scenes use `scene-*`; door glyphs use `glyph-*`.
- Every token in [`../tokens/tokens.json`](../tokens/tokens.json) has a note that says where it goes and its contrast on the grounds it sits on; [`tokens.css`](../tokens/tokens.css) has them as CSS variables, light and dark. Three pairs miss 4.5:1 and are flagged in their notes: `faint` on light, state words on the light scene floor, and two small labels on printed swag.
- No colours outside `tokens.json`. Never a gradient, and never purple or blue-to-purple.

## Type

- **Big Shoulders Display ExtraBold** (`display`), designed for Chicago's city signage, shares the wordmark's proportions. Set h1 and marketing headlines in it (`display-1`, `display-2`), and nothing else.
- **Atkinson Hyperlegible Next** (`sans`), by the Braille Institute, has letters that can't be confused. Set body copy and every heading from h2 down in it (`h2`, `h3`, `body`, `small`), so long reference pages don't shout.
- **Atkinson Hyperlegible Mono** (`mono`) sets commands, output and state labels (`mono`, `state-label`).
- All three are free under the SIL Open Font License 1.1, on Google Fonts.
- State labels go in capitals with 0.06em tracking (`state-label`). Everything else in sentence case.

## Iconography

- The **door glyphs** ([`../illustrations/doors/`](../illustrations/doors/)) are the state icons: 24 grid, filled, a light and a dark file each.
- Six **UI icons** ([`../illustrations/icons/`](../illustrations/icons/)) cover Napwake's own features: scan, pause, wake, status, forecast (`autoResume`) and cost. 24 grid, filled, arch-topped where there's a door, one ink with white details: `brand` (Coat on light, #4FB3A6 on dark). Use the `-dark` file on dark grounds.
- No other icon set and no emoji. A feature without an icon gets a word, not a borrowed icon.
- Three shapes make everything: the **arch** (doors, the wordmark's counters, glyphs, icons, the sticker's cut), the **wedge** (light from a door) and the **circle** (buttons, eyes, lamps).

## Illustration

- Corridors, lobbies and doorways at night: the porter, doors, a floor. Props only when the job needs them: a list, a clipboard, a switch, a watch, a note.
- One idea per drawing, captioned in plain words. One true joke at most.
- Light comes from doors. The far side of the coat falls into shade; his shadow falls away from the door.
- Illustrations get the print finish: a slight wobble on every edge and a grain inside the fills ([night-porter.md](night-porter.md#the-finish) has the filter). Never on the logo, the favicon, door glyphs or UI icons.
- No coins, bins, clouds, moons or Zzz, and nothing being thrown out: Napwake never deletes anything.
- Illustrations go on pages, cards, empty states and release notes, never inside documentation steps.

## Motion

- Progress is a door opening. Waiting is a door held ajar, breathing slowly, never a spinner.
- Light leads: the room lights amber before the door finishes opening, and the lamp turns green only once it's open, as the workload is Ready before held requests pass through.
- Ease everything with `ease-calm`, cubic-bezier(.45,0,.2,1): 300 to 600 ms in interfaces (`duration-ui-short`, `duration-ui-long`), 3 to 6 s for ambient loops (`duration-ambient`). No bounce.
- The waking page's wedge breathes once every 2.8 s (`duration-breathe`), between opacity .55 and .3.
- He moves little: his lids, one arm. He never jumps.
- Under reduced motion, stop every loop and show the end state, still.

## Layout

- Flat: separate things with `line` and `surface`, not shadows. Shadows are for mock-ups of objects (`shadow-window`, `shadow-print`).
- Corners: `radius-md` (6 px) for buttons and terminal blocks, `radius-lg` (8 px) for cards and callouts, `radius-xl` (12 px) for cards on brand pages, `radius-sm` (4 px) for inline code. Doors are arches, never rounded rectangles.
- Spacing: `space-1` to `space-18` (4 to 72 px).

## Accessibility

- Text meets 4.5:1 on the grounds its token's note names, in both themes, apart from the three flagged pairs; text from 24 px, marks and focus rings meet 3:1.
- Never colour alone: every state carries its word and its door's shape, and the terminal adds a glyph and bold.
- Keyboard focus is `focus-ring`: a 2 px gap in the page colour, then 2 px of `action` (6.14:1 on light, 10.02:1 on dark).
- Every surface ships light and dark (logos, glyphs, icons, cards, the docs, the waking page) and follows `prefers-color-scheme`.
- Alt text says what the picture shows, in plain words: "The night porter holds the door of a waking room; the rooms on either side are asleep or awake."

## The files

| Where | What | Licence |
|---|---|---|
| [`../logo/`](../logo/) | The logo, wordmark, mark, avatar and favicons | [TRADEMARKS.md](../TRADEMARKS.md) |
| [`../illustrations/`](../illustrations/) | The porter's poses, door glyphs, UI icons, scenes and a sticker | [CC BY 4.0](../illustrations/LICENSE) |
| [`../tokens/`](../tokens/) | Every colour, type style, spacing step, radius, shadow and timing, as JSON and as CSS | CC BY 4.0, like the illustrations |
| [`logo-rules/`](logo-rules/) | Clear space, construction and misuse drawings | [TRADEMARKS.md](../TRADEMARKS.md) |
