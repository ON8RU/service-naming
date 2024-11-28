# 🦎 GENN - Command-Line Utility for Title and Slug Generation

GENN - is command-line utility to help you generate titles for services and aliases for this.

## Key Features:
1. Title Generation with Themes:
The `-of` flag allows you to choose between predefined themes for generating titles:

    - Animals: Titles inspired by the animal kingdom (e.g., "Berserk Boomslang", "Slow Dachsador").
    - Space: Titles inspired by space exploration and celestial bodies (e.g., "Mature Astarte", "Fantastic Bryanhoran").
    - Professions : Names inspired by people's professions and their deeds (e.g., "Resonant Gofer", "Damaging Cook").

2. Slug Generation (-slugify):
The -slugify flag converts any string or title into a clean, SEO-friendly slug. This is ideal for generating readable, hyphenated URL strings that are compatible with web standards and search engines.

    - Animals: Titles inspired by the animal kingdom (e.g., "loving-lizard", "rich-sturgeon").
    - Space: Titles inspired by space exploration and celestial bodies (e.g., "hallowed-bunsen", "rural-charton").
    - Professions : Names inspired by people's professions and their deeds (e.g., "cumbersome-flautist", "adamant-tutor").

## Istallation

```bash
sudo wget https://raw.githubusercontent.com/ON8RU/service-naming/refs/heads/master/genn.sh -O /usr/bin/genn
```

```bash
sudo chmod +x /usr/bin/genn
```

## Usage Examples

### Generate a Themed Title (Animals):
To generate a title using the "animals" theme:

```bash
genn
```
or

```bash
genn -of animals
```

Output: `Plucky Siamese`

### Generate a Themed Title (Space):
To generate a title using the "space" theme:

```bash
genn -of space
```

Output: `Known Trinculo`

### Generate a Themed Title (Professions):
To generate a title using the "professions" theme:

```bash
genn -of professions
```

Output: `Ablaze Ethologist`

### Generate a Slug:
To generate an SEO-friendly slug from a string:

```bash
genn -slugify
```
Output: `handsomely-gecko`

or

```bash
genn -of animals -slugify
```

Output: `crimson-earthworm`

or

```bash
genn -of space -slugify
```

Output: `young-eurybates`

or

```bash
genn -of professions -slugify
```

Output: `vacuous-fishmonger`
