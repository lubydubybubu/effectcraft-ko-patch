# effectcraft-ko-patch

Korean (한국어) interface patch for **[EffectCraft](https://github.com/storytold/effectcraft)** (After Effects-class motion graphics), upstream tag `v0.9.2`.
This repository contains **only the patch**, not EffectCraft's source code. See `BASE.txt` for the exact upstream commit.

## Apply
```bash
git clone --branch v0.9.2 https://github.com/storytold/effectcraft.git && cd effectcraft
git apply ../effectcraft-ko-patch/patches/effectcraft-v0.9.2-ko.patch
```
Then build as upstream documents. Windows build without MSVC: [artcraft-ko-toolkit](https://github.com/lubydubybubu/artcraft-ko-toolkit).

## What it changes
New Korean catalog (624 menu + 506 panel rows, 1,130/1,130 of the most complete catalog) with Korean After Effects terminology; Hangul probed first (Malgun Gothic on Windows); Settings ▸ General ▸ Language ▸ 한국어.
Changed files: `CHANGED-FILES.txt`.

## Verified
14 Korean tests RED→GREEN, 64 i18n/theme/menu/settings tests; Windows headless render follows ko-KR: Korean menus, no tofu.

## Known limits
Dock tab titles, timeline column headers and workspace names are hard-coded English upstream (no language translates them yet).

Translations are AI-assisted (Claude Opus 5.5) and not reviewed by a professional translator.
Licence: MIT OR Apache-2.0, same as EffectCraft; upstream contributions credited above.
