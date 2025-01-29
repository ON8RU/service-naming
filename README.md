# 🦎 GENN - Command-Line Utility for Title and Slug Generation

GENN — a utility for generating creative titles and SEO-friendly slugs.

## Features
1. **Title Generation** (`-of`):  
   Generate names in specific themes:
   - `animals` (Example: "Plucky Siamese")
   - `space` (Example: "Mature Astarte")
   - `professions` (Example: "Ablaze Engineer")

2. **Slug Conversion** (`-slug`):  
   Converts the generated title to **kebab-case** (e.g., `plucky-siamese`).  
   *Two modes:*
   - `genn -of [theme]` → Returns a title.
   - `genn -of [theme] -slug` → Returns the title as a slug.

## Installation
```bash
sudo wget https://raw.githubusercontent.com/ON8RU/service-naming/refs/heads/master/genn.sh -O /usr/bin/genn
sudo chmod +x /usr/bin/genn
```

**Dependencies**:  
- Bash ≥4.0
- `wget` (for installation only)

## Usage
### Generate a Title
```bash
genn                  # Random theme → "Adamant Tutor"
genn -of animals      # "Plucky Siamese"
genn -of space        # "Known Trinculo"
```

### Convert Title to Slug
```bash
genn -of animals -slug      # plucky-siamese
genn -of space -slug        # mature-astarte
genn -slug -of professions  # ablaze-engineer (order-insensitive)
```

### Batch Generation
```bash
# 5 space-themed titles
for i in {1..5}; do genn -of space; done

# 3 animal-themed slugs
for i in {1..3}; do genn -of animals -slug; done
```

---

## Collaboration
🚀 **Want to contribute?** I’d love to collaborate! Here’s how you can help:
- **Report bugs** or suggest features in [Issues](https://github.com/ON8RU/service-naming/issues).
- **Submit Pull Requests** for fixes or improvements.
- **Propose new themes** (e.g., `tech`, `mythology`, `food`).

---

## Development
License: [MIT](https://choosealicense.com/licenses/mit/).  
For setup details, check the [repository](https://github.com/ON8RU/service-naming).

---

✨ **Pro Tip**: Add `alias genn="bash /usr/bin/genn"` to your `.bashrc`/`.zshrc` for quick access!