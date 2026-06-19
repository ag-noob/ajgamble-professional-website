here is the GitHub repo you will be working with: 
https://github.com/ag-noob/ajgamble-professional-website

here is the handoff instructions from Claude chat who took over the site build after i had been working with Gemini on the build for a couple of days.  Gemini was way too hands on for my liking.  :
Project Hand-off Summary

Tech Stack: Astro (Static Site Generator), deployed via Cloudflare Pages.
Repository: [paste your new public GitHub URL here]

Current State (as of last working session, verify against actual repo —
this summary wasn't generated from inspecting the live code):
- Structure: Migrated from a blog-only setup to a professional portfolio.
  Key pages: /index (Home), /experience (Portfolio), /about.
- Layouts: Consolidated into BlogPost.astro — CSS/layout logic modified
  to support static pages without date requirements, plus a "banner"
  style header. Known issue: this layout is doing double duty for all
  page types; may be worth splitting into PageLayout.astro and
  PostLayout.astro for maintainability if the site grows.
- Navigation: Header.astro cleaned up to Home / Experience / About,
  default "Blog" nav link removed.
- Content: /experience page has three styled sections — McKissick
  Products (Turnaround), The Crosby Group (Scaling), Industrial
  Splicing (Operational Excellence).
- Design: Minimalist, professional aesthetic. Custom hero banner image
  at /public/header-bg.jpg. Header image uses a fixed aspect-ratio in
  CSS — if the image changes shape, aspect-ratio/object-position in
  BlogPost.astro will need adjusting to keep framing right.

Deployment: Repo was just migrated from GitLab to GitHub (public repo).
Cloudflare Pages deployment source [is being / has been] repointed to
the new GitHub repo — confirm this is actually wired up and building
correctly before making changes.

Ask: Pick up where this left off — confirm current build status first,
then I'll direct specific changes from here.
