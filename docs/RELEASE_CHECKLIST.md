# Pre-release checklist

Do these in order and tick each box. Skipping any one of them costs at least a third of the conversion.

## Repo body
- [ ] `index.html` sits at the root, Pages serves it with no 404
- [ ] README first screen (before scrolling) has the one-line pitch and a hero image
- [ ] LICENSE is MIT and linked from the README footer
- [ ] About has the description (<=160 chars) and the Pages URL
- [ ] Topics added in the order given by `docs/TOPICS.md`

## Visual evidence (this drives most of the stars)
- [ ] Hero screenshot 1440x900 at `docs/screenshot.png`, placed after the first paragraph
- [ ] Phone screenshot 390x844 (proves the responsive claim)
- [ ] One shot of the block wall in hover state (proves interaction exists)
- [ ] Three clips, <=3 s each and <=2 MB: open a tool / click a square / swap the accent colour
- [ ] Social preview 1280x640 uploaded

## Credibility
- [ ] README states "no runtime network requests" and shows an empty DevTools Network panel
- [ ] The tool table matches the real `data-tool` count (30, no padding)
- [ ] No leftover lorem placeholder copy on the page

## Launch
- [ ] Tag `v1.0.0` with release notes: one-line pitch and the three clips
- [ ] First post: one line, hero image, link. No essay.
- [ ] Answer every issue/comment in the first 24 hours (stars track first-day engagement)

## Anti-patterns (these lose points)
- Never stack a wall of badges in the README
- Never write "blazing fast / supercharge / next-gen"
- No "Powered by AI" badge
- No empty issue templates
