# Pure OLED Rainbow

Pure black and pure white Obsidian surfaces with colourful folders, menus and note headings.

**Status: planning only. No theme code has been written.**

Plan date: 13 November 2026. This repository currently contains this planning README only. The name is a descriptive working name; Community name availability must be checked before any future submission.

Search keywords: Obsidian theme, OLED, AMOLED, pure black, pure white, rainbow folders, colourful file explorer.

## Who this is for

People who want the Pure OLED Black White foundation with much richer navigation and document colours.

## User need and evidence

Rahul requested this additional theme on 13 November 2026: keep pure black and pure white backgrounds, add at least 20 folder colours, vary colours through every nesting level, and colour menus and actual headings.

- [Existing Pure OLED Black White foundation](https://github.com/tutivsoft-com/pure-oled-black-white)

The Reddit links come from the preceding idea research and represent qualitative demand, not a market-size estimate or proof that existing themes do not solve the problem. For Pure OLED Rainbow, the additional requirement comes directly from the owner. Other themes and snippets may already address parts of these needs.

## Planned appearance and features

- Keep primary editor, file explorer, sidebars, panels, menus and dialog surfaces exactly #000000 in dark mode and #FFFFFF in light mode.
- Use separate colour palettes for dark and light modes so coloured text remains readable on each background. Pure white is a light appearance choice, not an OLED power-saving claim.
- Provide at least 20 distinct folder accent colours per mode, arranged so adjacent visible siblings have clearly different colours. Rotate after the palette is exhausted.
- Apply colours to folder labels, folder icons and disclosure arrows where available. Keep filenames readable; related file accents may complement their folder without erasing distinctions.
- Apply colour variation at every supported nesting depth, including children, grandchildren and deeper folders. Children must not all inherit one parent colour.
- Aim for a varied, random-looking order within each folder, with a different starting offset or order at deeper levels. Keep assignment stable during ordinary browsing and redraws.
- Avoid immediate parent/child colour repeats and adjacent sibling repeats where the tree structure and palette allow. Do not claim every folder in an unlimited vault has a globally unique colour.
- Use colour in navigation icons, tabs, menu icons or labels, settings sections, properties, callouts, links and status indicators while retaining clear semantic meanings.
- Colour the actual H1-H6 heading text, with strong size and weight hierarchy. Coordinate bold, italic, highlights, code syntax, internal links and external links.
- Keep selection, hover, search matches and keyboard focus unmistakable. Use coloured borders, underlines or markers where useful while keeping ordinary surfaces pure black or pure white.
- Preserve Obsidian navigation, layout and folder operations. Keep the original Pure OLED Black White theme and its releases separate.

## Mode scope

Both modes are required: pure black dark mode and pure white light mode.

## Folder colour feasibility to resolve before coding

This is a theme plan, not a promise that plain CSS can provide true random or path-stable colours. First inspect the current file explorer structure and supported selectors. Evaluate repeating sibling palettes and depth-based offsets for a stable, random-looking result. Check collapsed and virtualised tree behaviour before choosing an approach.

A theme stylesheet cannot perform arbitrary path hashing or generate persistent random assignments. If the exact nested behaviour cannot be delivered reliably through theme CSS, explain the specific gap to Rahul before changing scope or proposing a companion plugin. The required outcome remains 20 or more rotating colours, variation within nested folders and clear neighbouring distinctions. Do not silently reduce this to colouring top-level folders only.

## Future implementation and release plan

1. Confirm the final palette and layout against the requirements above.
2. Build the theme only after Rahul authorises implementation. Prefer supported Obsidian CSS variables and keep source readable.
3. Test representative notes, navigation, tabs, properties, menus, settings, search, Canvas and Bases where applicable. Include focus, selection, hover and error states.
4. Run the theme-specific checks below and record the actual Obsidian versions, devices and modes tested.
5. Prepare the root manifest, stylesheet, licence and real screenshots. Decide the first release version and minimum app version from actual testing.
6. Follow the current Obsidian submission guidance when a release is separately authorised. Commit source and screenshots, tag the intended revision, attach matching release assets and verify the published listing.

Keep assets offline, respect font and third-party licences, and avoid required plugins for the core appearance. Do not configure GitHub Actions or automatic deployment.

Official references for later implementation:

- [Build a theme](https://docs.obsidian.md/Themes/App%20themes/Build%20a%20theme)
- [Submit a theme](https://docs.obsidian.md/Themes/App%20themes/Submit%20your%20theme)
- [Developer policies](https://docs.obsidian.md/community-directory/developer-policies)

These are future work items. No release, installation instructions, compatibility certification or Community listing is being claimed by this planning repository.

## Acceptance checklist for later implementation

- [ ] Build a sample tree with at least 45 sibling folders, mixed files, empty folders and at least 8 nested levels; test palette rotation and deeper variation.
- [ ] Check adjacent visible folders and immediate parent/child pairs for easily distinguishable colours. Twenty colours cannot guarantee that every possible pair has high mutual contrast; review perceptual separation as well as text/background contrast.
- [ ] Collapse and expand folders, scroll, sort, rename, move, create and delete sample folders; check that colour behaviour is predictable and does not flicker.
- [ ] Measure coloured text against #000000 and #FFFFFF independently; do not simply reuse bright dark-mode colours on white.
- [ ] Check desktop and mobile navigation, menus, actual heading text and selected states.
- [ ] Verify pure surface colours in core views. Record third-party plugins that override surfaces rather than claiming control of every plugin.
- [ ] Confirm every claimed feature has been implemented and tested before replacing the planning-only status.
- [ ] Review screenshots for private information and verify all published documentation and asset paths.
- [ ] Verify the default branch, release revision and uploaded assets before calling any future release complete.

## Current boundary

Only repository creation and this Markdown plan are authorised in this task. Do not add theme CSS, manifests, screenshots, release tags or submissions as part of this planning work. Future work stays on this repository's verified primary branch.
