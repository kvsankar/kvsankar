# Repository instructions

## Purpose

This is the source repository for the `kvsankar` GitHub profile. GitHub renders
`README.md` on the profile page.

Keep this profile focused on public GitHub projects and the work behind them.
Use Sankara.net as the broader home for career history, personal interests, and
long-form material. The profile may link to those surfaces without duplicating
their full content.

## Repository structure

- `README.md` is the single-page profile source.
- `images/` contains profile artwork referenced from the README.
- Do not introduce subpages or a navigation tree unless explicitly requested.
- Keep `AGENTS.md` and `CLAUDE.md` identical so agents receive the same guidance.

## README conventions

- Use one H1 for the introduction, H2 headings for peer sections, and H3
  headings for projects within a section.
- Keep the Explore table compact and link it to sections on the same page.
- Describe GitHub-backed projects in useful detail; hand broader personal
  material off through the compact Beyond GitHub section.
- Keep AI and DevEx entries text-only. Images may remain in astronomy and
  outreach sections where they materially show the work.
- Prefer concise descriptions followed by explicit `Live`, `Source`, or
  destination links.
- Verify claims against the linked project or live page. Do not fabricate or
  infer documentation content.
- Preserve existing local image files unless their removal is explicitly in
  scope, even when a README reference is removed.

## Validation

There is no application build or test suite. For README changes:

1. Run `git diff --check`.
2. Render with Pandoc when available:
   `pandoc --from=gfm --to=html --standalone --output=/tmp/kvsankar-profile-preview.html README.md`.
3. Confirm internal anchors and newly added external links.
4. Inspect the final diff and live README after a push.

## Git safety

- Stage only files intended for the current change; do not use `git add -A` in
  a mixed worktree.
- Use the configured SSH remote for fetch and push.
- Do not rewrite history, force-push, skip hooks, or work around validation
  failures without explicit permission.
- If hooks or checks fail, fix the underlying issue.
- Commit and push only when requested.
- If two approaches fail for the same problem, stop and present options rather
  than trying repeated speculative fixes.
