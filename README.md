# Hildegard Craft

Craft skills for serious creative work: writing, web and interface design, photo and video editing, recording cleanup, 3D models and parts to print drawn in code, and a make, check, refine loop. Instructions only.

These are skills for Claude: plain instructions and a few small helper scripts that Claude reads when your request
matches. They teach the habits of a careful maker: interview before drafting, look at the real thing, check it
against measurements and a rubric, and refine until it passes. The plugin has no server, hook or background process,
and its own scripts open no network connection.

## What is in it

- **hildegard**: the method for serious work in any form: a short interview, research, drafts, contact sheets, blind critique and checks. Covers writing (fiction, essays, papers in APA, Chicago or MLA), storyboards, image and video editing, color, dialogue cleanup, and music and sound made in code.
- **hildegard-3d**: models for screens and for printing, built in code and checked view by view for size and watertight meshes.
- **hildegard-craft**: the bar every other skill holds: brief, lint the prompt, review against a rubric, decide whether the work is fit to hand over.
- **hildegard-loop**: draft, render, critique, refine: how to keep improving a piece in rounds until it passes its own checks.
- **hildegard-openscad**: exact, parametric parts in OpenSCAD code (brackets, enclosures, knobs, clips, gears, threads), checked and measured.
- **hildegard-photo-edit**: professional photo editing with ImageMagick: straighten, white balance, exposure, color, sharpen, export.
- **hildegard-print**: working parts to 3D print: sized from a photo or listing, fits checked, sliced, handed over with a print sheet.
- **hildegard-video-edit**: professional video editing with FFmpeg: cut, trim, grade, caption, reframe, mix and finish, then check the result.
- **hildegard-web**: websites and app screens as real HTML and CSS, checked at phone, tablet and desktop width in light and dark, with eight finished templates.

## How to use it

Install the plugin from Claude's directory, or in Claude Code:

```text
/plugin marketplace add baney75/hildegard-plugin
/plugin install hildegard-craft@hildegard-craft
```

Then ask for the work in plain words. Claude loads the skill that fits:

- "Edit my photo: straighten the horizon, fix the white balance, export for the web."
- "Cut these clips into a 30-second teaser with captions and check the audio levels."
- "Design a replacement knob I can 3D print, 40 mm wide, and check it fits."
- "Build a one-page site for my bakery at phone and desktop width, light and dark."
- "Draft a five-page essay in APA, then critique it as a hostile reader would."

To name a skill yourself, type its name after the plugin's, such as `/hildegard-craft:hildegard-web`.

## Good to know

- The skills work on their own. Some mention Hildegard, a separate free open-source app that runs on your own
  computers. It is not part of this plugin and nothing here needs it; where a skill names one of its tools, use your own.
- A few skills use programs you may already have, such as FFmpeg, ImageMagick, OpenSCAD or Blender. They are not
  included. One helper script (cutout.py) needs the rembg library (from pypi.org), which downloads its own model from
  github.com the first time you run it. A few skills suggest installing other Python packages and fonts the same way.
  Everything that can reach the network is listed at https://dbaney.com/hildegard/privacy/. Claude runs commands only with the permission you have set.
- Privacy: https://dbaney.com/hildegard/privacy/. Terms: https://dbaney.com/hildegard/terms/. Support and bug reports: https://github.com/baney75/hildegard/issues.

## License

AGPL-3.0-only (see LICENSE). The site templates inside hildegard-web are Apache-2.0 (LICENSE-APACHE).
Source: https://github.com/baney75/hildegard (skills/ there is what this plugin carries).
