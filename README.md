# Assets

Shared image assets for [HomeRacker](https://github.com/kellerlabs/homeracker) projects.

Images are hosted here to keep source repositories lightweight — avoiding git history bloat from binary files.

## Structure

```text
common/                 # Shared across projects
└── makerworld/images/  # Shared MakerWorld banners & logos

homeracker/             # CC BY-SA 4.0
├── img/                # README + GitHub Pages images
└── models/             # MakerWorld description images
    └── <model>/makerworld/images/

homeracker-exclusive/   # Source-available
└── models/             # MakerWorld description images
    └── <model>/makerworld/images/
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

See [image-hosting-assets-repo](https://github.com/kellerlabs/homeracker/blob/main/docs/decisions/image-hosting-assets-repo.md) for design rationale.

## 🚀 Quick Start

This repo enforces [pre-commit](https://pre-commit.com/) hooks to auto-optimize images on commit.

**Prerequisites**: Python 3.x

```bash
python3 -m venv .venv

# Windows (Git Bash):
source .venv/Scripts/activate
# macOS/Linux:
source .venv/bin/activate

pip install -r requirements.txt

# Install the git hooks
pre-commit install --install-hooks -t commit-msg -t pre-commit
```

Now pre-commit will automatically run on `git commit`. To manually run hooks on all files:

```bash
pre-commit run --all-files
```
