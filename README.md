# Laws

Two skill packs that bundle canonical laws, principles, and heuristics for software engineering and UX design. Each pack lives in its own folder with a `SKILL.md` manifest and a `laws/` directory of individual markdown files.


## Quickstart - both skills

```bash
npx skills add fmhall/software-laws
```

## Skills

### [engineering-laws/](engineering-laws/) — 56 laws of software engineering

Conway's Law, Brooks's Law, Hyrum's Law, YAGNI, DRY, SOLID, CAP theorem, and more. Scraped from [lawsofsoftwareengineering.com](https://lawsofsoftwareengineering.com/).

```bash
npx skills add fmhall/software-laws/engineering-laws
```

See [engineering-laws/README.md](engineering-laws/README.md) for the full categorized index.

### [ux-laws/](ux-laws/) — 30 laws of user experience

Hick's Law, Fitts's Law, Jakob's Law, Miller's Law, Peak-End Rule, the Gestalt principles, and more. Scraped from [lawsofux.com](https://lawsofux.com/).

```bash
npx skills add fmhall/software-laws/ux-laws
```

See [ux-laws/README.md](ux-laws/README.md) for the full categorized index.

## Usage

Once installed, both skills auto-trigger on relevant discussions (architecture trade-offs, UX decisions, etc.). You can also invoke them directly:

```
/software-laws         # pull the laws into context as a reference
/ux-laws               # pull the UX laws into context as a reference
```

Each skill ships an `audit` command that runs a full review of the current project against every law in the pack, with prioritized, location-specific recommendations:

```
/software-laws audit   # audit architecture, code quality, and team/process signals
/ux-laws audit         # audit interfaces, flows, and components
```

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
