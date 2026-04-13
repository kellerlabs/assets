# Assets

Shared image assets for [HomeRacker](https://github.com/kellerlabs/homeracker) projects.

Images are hosted here to keep source repositories lightweight — avoiding git history bloat from binary files.

## Structure

```text
homeracker/             # CC BY-SA 4.0
├── img/                # README + GitHub Pages images
└── models/             # MakerWorld description images
    └── <model>/makerworld/images/

homeracker-exclusive/   # Source-available
└── models/             # (reserved for future)
```

## Licensing

Each top-level folder has its own license:

- `homeracker/` — [CC BY-SA 4.0](homeracker/LICENSE)
- `homeracker-exclusive/` — [Source-available](homeracker-exclusive/LICENSE)

## Usage

Reference images via `raw.githubusercontent.com`:

```markdown
![alt](https://raw.githubusercontent.com/kellerlabs/assets/main/homeracker/img/example.png)
```

See [ADR-001](https://github.com/kellerlabs/homeracker/blob/main/docs/decisions/ADR-001-image-hosting-assets-repo.md) for design rationale.
