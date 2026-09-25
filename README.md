# my-personal-branding

Personal archive for branding documents: CV/resume, portfolio case studies,
social media records, brand assets, bios, and testimonials.

Everything here is plain files - Markdown for text, PDF (or whatever format the
recipient asked for) for anything sent out, images for assets. No build step,
no tooling.

This archive is **public**: it holds only material meant to be seen, and the CV
carries public contact channels only. What is deliberately kept out is listed
under [Public scope](#public-scope).

## Layout

| Path | What lives here |
| --- | --- |
| `resume/cv-master.md` | The single master CV - always edited here |
| `resume/tailored/` | Role-targeted CV variants, one file per position (living, edited in place) |
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
| `bio/` | Copy-paste bios - one file per platform (`linkedin.md`, `youtube.md`, `instagram.md`, `threads.md`, `x.md`, `dailydev.md`, `devto.md`, `github.md`, `facebook.md`, `tiktok.md`), each with EN + ID and a short + long tier |
| `testimonials/` | Quotes with source and permission flag |
| `archive/` | Outdated documents, scans, raw material |

## Conventions

- File names: `kebab-case`; ISO dates (`2026-09-20`) when a date is needed.
- Files starting with `_` are templates.
- **Master vs archive**: living files (`cv-master.md`, `resume/tailored/`, `bio/`,
  `social/accounts.md`) are edited in place - git keeps their history. Anything sent out
  (`resume/sent/`) or captured as a snapshot (`social/metrics/`) is dated and
  never edited again.
- One asset lives in one place - never duplicate headshots or logos across folders.

## Public scope

This repository is **public** - everything committed here is meant to be seen.

- Deliberately excluded: home address, ID/tax numbers, references' personal
  contacts, and anything under NDA. Notes like that belong in `private*.md`,
  which is git-ignored.
- Pushing is effectively permanent: a commit stays in the history, and a public
  repo can be forked, so deleting a file later does not unpublish it. Read the
  diff before every push.
- Contact channels in the CV stay public: email, LinkedIn, GitHub, website. No
  phone number.

## License

The written content (CV, bios, portfolio, brand notes) is licensed under
[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) - share it
with attribution, no commercial use, no derivatives. Full text: [LICENSE](LICENSE).
