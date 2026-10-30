# You Don't Need Forge GUI

A Roblox development skill for AI coding assistants. It helps Roblox developers plan, build, debug, and polish games in Roblox Studio with clear Luau, deliberate UI, readable maps, and practical performance checks.

The skill is named `youdontneedforgegui` in its `SKILL.md` metadata. It guides an assistant through the work; it does not replace Roblox Studio or claim to run or test a project when those tools are unavailable.

## What it helps with

- Roblox Studio and Luau implementation, debugging, and code review
- Bright, cartoony UI with chunky outlined buttons, responsive layouts, proximity labels, and restrained screen transitions
- Map building, including classic stud-style terrain and low-poly scenery
- Figma-to-Roblox and Blender-to-Studio workflows, with practical Studio alternatives when those tools are not connected
- Performance work such as instance streaming, client-only decorative props, and checking part counts
- Careful inspection of user-provided `.rbxl` places before adapting their structure or behavior

The included button and shop-window designs are visual references. They do not ask the assistant to create a shop or copy a sample screen unless that is what the developer requested.

## Install

Install or import the **entire repository folder** using your assistant's skill installation method. Keep `SKILL.md`, `references/`, `assets/`, and `reference-projects/` together; the skill loads its guides and examples from those paths.

For Codex, clone the repository into your user skills directory:

```bash
git clone https://github.com/scamaltmancool/youdontneedforgeguiII.zip.git ~/.agents/skills/youdontneedforgegui
```


## Use

Ask for the Roblox task in your normal language. For example:

- “Build a small classic stud island map in my place.”
- “Review this LocalScript and fix the respawn bug.”
- “Adapt this Figma HUD for Roblox Studio and give me the import steps.”
- “Find why the map lags when players enter the forest.”

The skill checks the task, the available project files, and the relevant reference material before proposing changes. For implementation work, it calls for a Studio test checklist and distinguishes work that was actually tested from work that still needs testing.

## Repository contents

```text
SKILL.md
README.md
references/
  UI, map-building, lighting, modeling, performance, and code-quality guides
  Luau examples for buttons, proximity labels, decoration, and screen transitions
assets/
  icons/
reference-projects/
  README.md
  user-supplied .rbxl reference places
```

The reference places are source material, not audited or modified projects. The skill directs the assistant to inspect a copy in Studio before adapting it and to review scripts and assets before use.

## Asset notes

The asset IDs in `references/stud-map-and-vfx.md` are references, not verified assets. Check their type, availability, permissions, and contents in Roblox Studio before relying on them. Inspect models and remove scripts that are not needed before integrating them.

The bundled places and icons came from user-supplied materials. Review ownership and redistribution rights for every included place and asset before making the repository public. No license file is included in this package.

## Compatibility and limitations

The skill uses `SKILL.md` and lists Claude Code, Cursor, VS Code Copilot, Hermes, OpenHands, and OpenClaw as compatible Agent Skills environments. An assistant still needs access to Roblox Studio or a suitable project tool to inspect or test a place. It must say when it cannot do so and provide Studio steps instead of claiming a test ran.


## Screenshots of the UI
<img width="1200" height="633" alt="image" src="https://github.com/user-attachments/assets/0bc5227d-3ce9-41e3-bd9a-7f92017750e1" />
<img width="1204" height="639" alt="image" src="https://github.com/user-attachments/assets/bd293d39-bd29-4bba-8a22-7718d8c58eba" />

