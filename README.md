# Laws

Two skill packs that bundle canonical laws, principles, and heuristics for software engineering and UX design. Each pack lives in its own folder with a `SKILL.md` manifest and a `laws/` directory of individual markdown files.

## Skills

### [engineering-laws/](engineering-laws/) — 56 laws of software engineering

Conway's Law, Brooks's Law, Hyrum's Law, YAGNI, DRY, SOLID, CAP theorem, and more. Scraped from [lawsofsoftwareengineering.com](https://lawsofsoftwareengineering.com/).

```bash
npx skills add fmhall/software-laws
```

See [engineering-laws/README.md](engineering-laws/README.md) for the full categorized index.

### [ux-laws/](ux-laws/) — 30 laws of user experience

Hick's Law, Fitts's Law, Jakob's Law, Miller's Law, Peak-End Rule, the Gestalt principles, and more. Scraped from [lawsofux.com](https://lawsofux.com/).

```bash
npx skills add fmhall/ux-laws
```

See [ux-laws/README.md](ux-laws/README.md) for the full categorized index.

## Structure

```
engineering-laws/
  SKILL.md          # skill manifest + quick reference
  README.md         # categorized index
  laws/             # 56 individual law files
ux-laws/
  SKILL.md          # skill manifest + quick reference
  README.md         # categorized index
  laws/             # 30 individual law files
```

Each law file has frontmatter (`title`, `slug`, `category`, `summary`, `source`) and sections for Takeaways, Overview, and Origins.
