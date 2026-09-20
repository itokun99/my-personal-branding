# my-personal-branding

Personal archive for branding documents: CV/resume, portfolio case studies,
social media records, brand assets, bios, and testimonials.

Everything here is plain files - Markdown for text, PDF (or whatever format the
recipient asked for) for anything sent out, images for assets. No build step,
no tooling.

## Layout

| Path | What lives here |
| --- | --- |
| `resume/cv-master.md` | The single master CV - always edited here |
| `resume/sent/` | Archive of CVs actually sent (dated names, never edited after) |
| `resume/cover-letters/` | Cover letter drafts and sent versions |
| `resume/certificates/` | Certificates and awards (pdf/png) |
| `portfolio/_template.md` | Template for new case studies |
| `portfolio/<project>/` | One folder per project: `case-study.md` + `assets/` |
| `social/accounts.md` | Registry of all social accounts |
| `social/content/` | Post drafts and published records (dated names) |
| `social/metrics/` | Monthly follower/engagement snapshots |
| `brand/headshots/` | Public photos |
| `brand/logos/` | Logo and favicon files |
| `brand/identity.md` | Colors, fonts, tagline |
| `bio/short.md`, `bio/long.md` | Copy-paste bios |
| `testimonials/` | Quotes with source and permission flag |
| `archive/` | Outdated documents, scans, raw material |

## Conventions

- File names: `kebab-case`; ISO dates (`2026-09-20`) when a date is needed.
- Files starting with `_` are templates.
- **Master vs archive**: living files (`cv-master.md`, `bio/`, `social/accounts.md`)
  are edited in place - git keeps their history. Anything sent out
  (`resume/sent/`) or captured as a snapshot (`social/metrics/`) is dated and
  never edited again.
- One asset lives in one place - never duplicate headshots or logos across folders.

## Privacy

- Keep this repository **private** - it aggregates personal data.
- Never commit what you do not want public: home address, ID numbers,
  references' personal contacts. Keep notes like that in `private*.md`
  (git-ignored).
