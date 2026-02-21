# Plan

## Overview

Planning

- [x] Write MOTIVATION.md
- [x] Write PLAN.md

## Acceptance

- [ ] Entire still working as is at https://secondrenaissance.net/
- [x] Entire site served from Flowershow
- [ ] Notified Sylvie and anyone else using framer

## Tasks

*Keep the old repo and Framer site untouched until the new site is clearly viable, then decommission deliberately.*

- [x] Flowershow Self-hosted to Cloud
- [x] Framer to Flowershow
- [ ] Repo reordering
- [ ] Deployment
  - [ ] Remove frontend proxy

### Flowershow Self-hosted to Cloud

* **Will not start with the ecosystem split**; treat it as already decided and out of scope for the first steps.
* **Create a new, clean repo for the FlowerShow Cloud site** and copy only the core Markdown content you intend to keep.
  * Rationale: reduces cognitive load, avoids legacy cruft, avoids risky force-pushes, and makes the new site feel intentional.
* First milestone:
  * Get FlowerShow self-hosted content deploying end-to-end on FlowerShow Cloud.

#### Tasks

- [x] Analyse what is in old site outside of ecosystem
- [x] Copy over base markdown **✅2026-01-20**
- [ ] Migrate nextjs style pages (two of them: index.jsx and map.jsx)
  - [ ] Copy over pages (next)
  - [ ] Convert those pages to markdown
- [ ] Add back in the map?

---

### Framer to Flowershow

- [x] What content is there
- [x] Analyse how to migrate a framer page (focus on art) **✅2026-01-20 this works quite well to just brute force with anti-gravity**
- [x] Cache framer html pages **✅2026-01-20 to `tmp/framer`**
- [ ] Migrate pages - first convert
  - [ ] `/` **will do by hand as flowershow self-hosted had this**
    - [x] Tweak hero text
    - [x] add video after hero **✅2026-01-24**
    - [x] Fix up calls to action at bottom
    - [x] Fix rendering on flowershow cloud **✅2026-01-20 now works**
    - [x] Fix button styling (here and everywhere ...?) **✅2026-01-24**
  - [x] `/art` **🚧2026-01-20 tailwind. ✅**
  - [x] `/art/exhibition` **🚧2026-01-20 tailwind✅**
  - [x] `/art/collective` **🚧2026-01-20 tailwind✅.**
    - [ ] Need to copy over hero image plus missing top text.
  - [x] `/art/residency` **🚧2026-01-20 tailwind✅**
  - [x] `/art/magazine` **🚧2026-01-20 tailwind✅**
  - [x] `/art/manifesto` **🚧2026-01-20 tailwind✅**
  - [x] `/art/magazine-submission` **✅2026-01-21 done as markdown by hand**
  - [x] `/course` **Already exists as markdown. Not much changed from original**
    - [ ] ❓ Add hero.
    - [ ] Check content for updates
  - [x] `/about` **✅2026-01-20 just go with markdown 😉. Updated content to latest. all done**
    - [ ] hero image ❓ (not sure really needed here?)
  - [ ] `/unconference` 🔽 **can use markdown.**
    - [x] migrate content **✅2026-01-21**
    - [ ] hero image
    - [ ] 🔽 images at bottom of orgs involved
  - [x] `/oasis` **Do in markdown by hand. Want nice hero?**
    - [ ] nice hero ...
  - [x] `/ecosystem`  **✅2026-01-25 migrated.**
    - [ ] need to fix links to go to new website ...
  - [x] `/paper` **Can probably do in markdown better** **✅2026-01-25 used html in the end as nicer for now.**

### Repo refactoring

Want to end up with 2 repos:

- One for ecosystem stuff as per https://github.com/life-itself/community/issues/1210
- This one for the website

What is currently in this repo should really go into ecosystem (and be refactored). Meanwhile we have the new website fairly clean.

Tasks

- [x] Create new repo for ecosystem **✅2026-01-23 at https://github.com/life-itself/2r-ecosystem**
- [x] Push this repo current content to that new repo
  - [x] Clean up branches here first
- [x] Force push the new repo content here from the new repo we have made **✅2026-01-23 https://github.com/life-itself/secondrenaissance is now the new clean version**

### Deploy new site

- [ ] Set up flowershow.app for that ...
- [ ] Switch over DNS
- [ ] Remove front end proxy


## Tidy-ups / themeing

🏆

- [ ] Set favicon
- [x] Flowershow supports nice heros **✅2026-01-21**
- [ ] Nice "2R" theme

# Inbox

- [ ] ➕2026-01-20 💤 split out the pip and cohere assets to their own subfolders so it is clean (rewrite markdown for this)
- [ ] ➕2026-01-20 work out what we do with old /wiki - kind of random and only standard thing is overview-mapping-efforts.md
  - [x] have moved overview-mapping-efforts to root
    - [ ] Create a redirect for this ...
