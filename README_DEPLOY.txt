WEAPON EVOLUTION: THE ABSOLUTE — 2.5D CINEMATIC BUILD

WHAT THIS PACKAGE DOES
- Runs immediately in a browser with fallback weapon visuals.
- Becomes photorealistic when you add transparent WebP weapon images and cinematic WebP backgrounds.
- Keeps the hardened input/game-loop architecture designed for iPad Safari.
- Uses no paid hosting and no paid database.

RECOMMENDED HOST: GITHUB PAGES
Why: static WebP/PNG/audio assets are served directly and cached well. This is better for an asset-heavy game than Google Apps Script.

FILES TO ADD
Weapons:
  assets/weapons/w01.webp ... w50.webp
Use transparent background. Recommended source size: 1024x1536 or 1024x1024.
Try to keep each exported WebP around 100-400 KB.

Backgrounds:
  assets/backgrounds/bg01_forest.webp
  assets/backgrounds/bg02_fortress.webp
  assets/backgrounds/bg03_battlefield.webp
  assets/backgrounds/bg04_elemental.webp
  assets/backgrounds/bg05_futurecity.webp
  assets/backgrounds/bg06_planetary.webp
  assets/backgrounds/bg07_space.webp
  assets/backgrounds/bg08_nebula.webp
  assets/backgrounds/bg09_reality.webp
  assets/backgrounds/bg10_absolute.webp
Recommended source size: 1920x1080, WebP quality 70-82, ideally 200-700 KB.

LEVELS
01. Stick -> assets/weapons/w01.webp
02. Bone Stick -> assets/weapons/w02.webp
03. Cardboard Sword -> assets/weapons/w03.webp
04. Wooden Sword -> assets/weapons/w04.webp
05. Stone Sword -> assets/weapons/w05.webp
06. Copper Sword -> assets/weapons/w06.webp
07. Iron Sword -> assets/weapons/w07.webp
08. Frost Iron Sword -> assets/weapons/w08.webp
09. Flame Iron Sword -> assets/weapons/w09.webp
10. Iron Sword v3 -> assets/weapons/w10.webp
11. Iron Sword v4 -> assets/weapons/w11.webp
12. Iron Sword v5 -> assets/weapons/w12.webp
13. Iron Sword v6 -> assets/weapons/w13.webp
14. Iron Sword v7 -> assets/weapons/w14.webp
15. Iron Sword v8 -> assets/weapons/w15.webp
16. Iron Sword v9 -> assets/weapons/w16.webp
17. Super Iron Sword -> assets/weapons/w17.webp
18. Ultra Iron Sword -> assets/weapons/w18.webp
19. Platinum Sword -> assets/weapons/w19.webp
20. Diamond Sword -> assets/weapons/w20.webp
21. Diamond Sword v2.4 -> assets/weapons/w21.webp
22. Diamond Sword v3.1 -> assets/weapons/w22.webp
23. Diamond Sword v4 -> assets/weapons/w23.webp
24. Diamond Sword v5 -> assets/weapons/w24.webp
25. Diamond Sword v6 -> assets/weapons/w25.webp
26. Diamond Sword v7 -> assets/weapons/w26.webp
27. Diamond Sword v8 -> assets/weapons/w27.webp
28. Diamond Sword v9 -> assets/weapons/w28.webp
29. Diamond Sword Supra -> assets/weapons/w29.webp
30. Netherite Sword -> assets/weapons/w30.webp
31. Netherite Sword v2.6 -> assets/weapons/w31.webp
32. Netherite Sword v3.3 -> assets/weapons/w32.webp
33. Netherite Sword v4 -> assets/weapons/w33.webp
34. Netherite Sword v5 -> assets/weapons/w34.webp
35. Netherite Sword v6 -> assets/weapons/w35.webp
36. Netherite Sword v7 -> assets/weapons/w36.webp
37. Netherite Sword v8 -> assets/weapons/w37.webp
38. Netherite Sword v9 -> assets/weapons/w38.webp
39. Netherstar Sword -> assets/weapons/w39.webp
40. Brain Sword -> assets/weapons/w40.webp
41. Brain Sword Supra -> assets/weapons/w41.webp
42. Sword of the Cosmos -> assets/weapons/w42.webp
43. Sword of the Mutants -> assets/weapons/w43.webp
44. Sword of the Titans -> assets/weapons/w44.webp
45. Godstar Sword -> assets/weapons/w45.webp
46. Ultra Godstar Sword -> assets/weapons/w46.webp
47. Ultrastar Sword -> assets/weapons/w47.webp
48. Dark Ultrastar Sword -> assets/weapons/w48.webp
49. Darkgod Sword -> assets/weapons/w49.webp
50. Extreme Darkgod Sword -> assets/weapons/w50.webp
FREE DEPLOYMENT — GITHUB PAGES
1. Create a free GitHub account if you do not already have one.
2. Create a new public repository, for example: weapon-evolution.
3. Upload EVERYTHING inside this package while preserving the folder structure.
4. Open the repository Settings.
5. Click Pages.
6. Under Build and deployment, choose Deploy from a branch.
7. Branch: main. Folder: /(root).
8. Save.
9. GitHub will display the live website address after deployment.
10. Open the site in Safari on the iPad.
11. Use Safari Share > Add to Home Screen for an app-like icon.

IMPORTANT
- Do not rename index.html.
- Keep assets/weapons and assets/backgrounds exactly as shown.
- GitHub Pages is case-sensitive.
- Replacing an image does NOT require modifying the game JavaScript.
- After replacing images, allow GitHub Pages a short refresh cycle, then reload the browser.

SAVE SYSTEM
Progress is stored in localStorage on the current browser/device.
No database is required.

OPTIONAL LATER
If you need one profile shared across multiple devices, keep GitHub Pages for hosting and add a tiny Google Apps Script + Google Sheets save API later.

ASSET CREATION WORKFLOW
For each weapon:
1. Create/generate a photorealistic weapon on a transparent background.
2. Remove any remaining background.
3. Crop with some transparent breathing room around the weapon.
4. Export as WebP.
5. Rename exactly w01.webp, w02.webp, etc.
6. Put it in assets/weapons.

For each environment:
1. Create a cinematic 16:9 background.
2. Keep the central/lower area reasonably clear so targets remain readable.
3. Export as WebP.
4. Rename using the exact background filenames above.
5. Put it in assets/backgrounds.

PERFORMANCE TARGET
Total site target: roughly 15-35 MB.
Only the active weapon/background is requested by the browser.
This is far safer on iPad than 50 live high-poly 3D models.
