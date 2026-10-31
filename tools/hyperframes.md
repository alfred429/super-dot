# Hyperframes — video and presentations

Version: 1.0.0 · 2026-10-31

Reuse Hyperframes' existing authoring skills, templates and render pipeline on the Mac.
Start with [the official project](https://github.com/heygen-com/hyperframes) and its current
[CLI reference](https://github.com/heygen-com/hyperframes/blob/main/docs/packages/cli.mdx).
Check the installed version/help before following commands; don't replace a working pipeline.

## Set up once

Reuse an existing installation. With permission, prepare the documented prerequisites (currently
Node.js 22+ and FFmpeg for the CLI route). Native [Hyperframes Studio](https://hyperframes.heygen.com/)
is another supported entrypoint. Choose the route already suitable for the person's Mac.

The upstream project currently documents `npx hyperframes skills update` for its core authoring
skills. Installation changes the user's machine, so get the appropriate authorisation first.
Add specialised presentation/media skills only when that output needs them.

## Create something small

Use a creative project under the relevant life area. In its chosen working directory, the documented
CLI starting point is `npx hyperframes init my-video`. Read the installed Hyperframes skills, reuse
a suitable composition and preview it with `npx hyperframes preview` from that composition directory.

Follow the installed version's lint/layout checks and render guidance. `npx hyperframes render`
creates video; use its documented single-worker option where supported and render one job at a time.
Inspect the actual output before calling it finished. Presentation decks use the upstream slideshow
workflow; an interactive deck is distinct from an MP4.

Keep inputs, compositions and finished outputs in the personal project's assets. For narration,
reuse upstream media/transcription timing rather than estimating speech from character counts.
Recheck synchronisation after audio changes. Mac-dependent work waits when the Mac is unavailable;
preserve completed assets and resume the existing project. Public publishing is a separate choice.
