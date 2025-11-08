# Astro Claude Skill

This repository contains the **Astro Builder** Claude skill plus all of the docs you need to download it, bundle it into a `.skill` file, and start using it immediately.

## Repository Structure

- `README.md` – quick-start instructions (this file)
- `ASTRO-SKILL-GUIDE.md` – detailed feature guide you can link to visitors
- `astro-builder/` – the actual Claude skill payload (packaged into `astro-builder.skill`)

## Download The Files

- **Clone with Git:** `git clone https://github.com/<you>/astro-claude-skill.git`
- **Or download ZIP:** use GitHub’s “Code → Download ZIP”, then extract locally.

## Build The `.skill` Archive

1. Move into the skill directory:
   ```bash
   cd astro-claude-skill/astro-builder
   ```
2. Zip everything inside to create the distributable:
   ```bash
   zip -r ../astro-builder.skill .
   ```
3. The file `astro-builder.skill` will appear in the repo root, ready for upload.

## Upload And Use With Claude

1. Open Claude → Settings → Skills → Upload Skill.
2. Select `astro-builder.skill` and enable it for conversations where you want Astro help.
3. Keep `ASTRO-SKILL-GUIDE.md` nearby (or link to it in your repo) so collaborators instantly understand the skill’s capabilities and workflows.

Need more detail on what’s inside the skill bundle? Check `astro-builder/README.md` for a breakdown of the instructions, references, and helper scripts that ship with the package.
