# Antigravity Catalogue

Official remote skills and plugins registry catalogue for **[Antigravity for Android](https://github.com/aazimameen1122/antigravity)**.

## Files

* [`skills.json`](./skills.json) — Curated agent skills index.
* [`plugins.json`](./plugins.json) — Curated plugins and tool integration index.

## Schema

Each item in `skills.json` and `plugins.json` follows the `SkillCatalogueItem` schema:

```json
{
  "id": "skill-id",
  "name": "skill-name",
  "description": "Accurate description matching the upstream repository.",
  "category": "Development | Architecture | UI & Visual | Testing | Security | Quality & Filter | Optimization | Developer Tools",
  "isPlugin": false,
  "repoUrl": "https://github.com/owner/repo.git",
  "subPath": "path/inside/repo"
}
```

## Contributing

To submit a new skill or plugin to the catalogue, open a Pull Request updating `skills.json` or `plugins.json`. Ensure:
1. The repository is public and accessible.
2. The description accurately reflects the upstream repository without hallucinated features.
3. If the repository contains multiple skills, specify `subPath` pointing to the exact directory containing `SKILL.md`.
