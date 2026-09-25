# PROJECT KNOWLEDGE BASE

**Generated:** 2026-09-25
**Commit:** 5f229a9
**Branch:** main

## OVERVIEW
Public archive of Indrawan Lisanto's personal branding (**indrawandev**): master CV,
bios, portfolio case studies, social account registry and post records, brand assets.
Plain files only - Markdown for text, images for assets. No code, no build step, no
tooling. 18 tracked files, ~117 KB of source.

## STRUCTURE
```
my-personal-branding/
├── resume/       # cv-master.md (single source) + sent/ cover-letters/ certificates/
├── bio/          # one file per platform: linkedin.md, youtube.md, instagram.md
├── social/       # accounts.md registry + content/ post records + metrics/ monthly
├── brand/        # identity.md (colors/fonts/tagline) + headshots/ + logos/
├── portfolio/    # _template.md + one folder per project
├── testimonials/ # _template.md - quotes with source + permission flag
├── .agents/      # LOCAL ONLY (gitignored): upstream skill copies - see nested AGENTS.md
└── archive/      # outdated documents, scans, raw material
```

## WHERE TO LOOK
| Task | Location | Notes |
|------|----------|-------|
| Edit the CV | `resume/cv-master.md` | the single master, edited in place |
| Record a CV that was sent | `resume/sent/` | dated filename, never edited after |
| Bio for a specific platform | `bio/<platform>.md` | EN + ID, short + long tier, measured char count in each heading |
| About page / speaker bio | `bio/linkedin.md` (long tier) | the fullest form; YouTube's long tier doubles as channel copy |
| Add or verify a handle | `social/accounts.md` | 10-platform registry, keep current |
| Draft or record a post | `social/content/YYYY-MM-DD-<platform>-<slug>.md` | format in CONVENTIONS |
| Monthly follower snapshot | `social/metrics/YYYY-MM.md` | copy `social/metrics/_template.md` |
| Case study | `portfolio/<project>/case-study.md` | copy `portfolio/_template.md` |
| Headshots / logos | `brand/headshots/`, `brand/logos/` | one asset lives in one place |
| Colors, fonts, tagline | `brand/identity.md` | |
| Sensitive notes | `private*.md` (gitignored) | never commit |
| Social + branding playbooks | `.agents/skills/` | local only; see `.agents/skills/AGENTS.md` |

## CONVENTIONS
- Names: `kebab-case`; ISO dates (`2026-09-24`) when a date is needed. A leading `_` means template.
- **Master vs snapshot.** Living files (`cv-master.md`, `bio/`, `social/accounts.md`) are
  edited in place - git history is the versioning. Snapshots (`resume/sent/`, `social/metrics/`)
  are dated and never edited again.
- One asset lives in one place - never duplicate a headshot or logo across folders.
- **Post record format** (evidence: `social/content/2026-09-24-threads-react-blogger-api.md`):
  header block (Platform / Project / Links / Format), an EN and an ID variant, the
  measured character count in each section heading, posting notes at the end.
  Links go in the first reply/comment, never the post body (reach).
- **Lead title is fixed**: `AI-Native Full-Stack Engineer · Mobile-first` - identical in the
  CV header, every profile bio, and the website hero. Per-platform caps and tiers live in
  each `bio/<platform>.md`; the mobile-targeted and enterprise angles are labelled
  alternatives in `bio/linkedin.md`, not the lead.
- Empty directories are held by `.gitkeep` - that is why `git ls-files` shows files that
  appear to hold nothing.

## ANTI-PATTERNS (THIS PROJECT)
- **Never commit private material.** The repo is public and history is permanent - a
  fork keeps deleted files. Out of scope: phone number, home address, ID/tax numbers,
  references' personal contacts, anything under NDA. Those belong in `private*.md`.
- **No phone number in the CV** - public channels only (email, LinkedIn, GitHub, site).
- **Never edit `resume/sent/*`** - it records what was actually sent.
- **Never duplicate an asset** (headshot, logo) into a second folder.
- **Don't add tooling.** No generators, schemas, build steps, or package managers
  unless explicitly asked - this is an archive of plain files.

## COMMANDS
None - no build, test, lint, or package manager. The only routine operation is reading
`git diff` before `git push`: public history is permanent and unfixable by deletion.

## NOTES
- `.agents/`, `skills-lock.json` (`.gitignore` L12-13) and `.omo/` (L11) are gitignored, so they
  are ABSENT from a fresh clone and `README.md` does not mention them. All of `.agents/` is local;
  `.omo/init-deep.json` (the init-deep snapshot) is ignored the same way.
- Context files the two installed skills look for do not exist here:
  `.agents/product-marketing.md` (social) and `.agents/brand-context.md` (personal-brand).
  Both skills fall back to asking questions - expected, not a bug.
- Bio copy is per platform and per language: `bio/linkedin.md` (headline 220 / About 2,600),
  `bio/youtube.md` (channel description 1,000), `bio/instagram.md` (150) - each carries EN + ID
  and a short + long tier, and each heading states its measured char count. The former
  `bio/short.md` + `bio/long.md` were retired; every platform now has its own file -
  `linkedin.md`, `youtube.md`, `instagram.md`, `threads.md`, `x.md`, `dailydev.md`,
  `devto.md`, `github.md`, `facebook.md`, `tiktok.md` - every platform the old aggregates
  covered now has its own file.
- `LICENSE` is CC BY-NC-ND 4.0 (attribution, no commercial use, no derivatives) and at
  19 KB is the largest file in the repo; the written content is the licensed material.
