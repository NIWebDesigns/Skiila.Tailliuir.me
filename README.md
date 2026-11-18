# Skyla’s Kitchen — family recipe book

A mobile-friendly family recipe website with photos, categories, search, and shareable recipe links.

## For family and friends
Visitors can browse, search, open, and share recipes. The Edit recipe control is only shown after the owner has logged in.

## Skyla’s simple editing steps
1. Open the family website.
2. Tap **Owner login** at the top and enter the owner password.
3. Tap **Add a new recipe** (or open an existing recipe to edit it).
4. Add a photo, ingredients and directions, then tap **Save recipe**.
5. When finished, tap **Download recipe updates** and send the downloaded `recipes.json` file to the person who manages the website.

The website currently saves edits in the browser and device where Skyla made them. They do not automatically appear on the public family website or sync to another phone/computer. The downloaded `recipes.json` file must replace the old one in the GitHub Pages website before everyone sees the updates.

## Important security and ease-of-use note
This website is hosted as a static GitHub Pages site. Its password check is only a basic front-end screen, not secure authentication: a technically confident visitor could inspect or bypass it. Do not reuse this password for important accounts. Also, because the current version stores edits in one browser, it is not yet a true shared online recipe editor.

For the genuinely easiest setup for a non-technical owner, the next step is to connect a private sign-in and shared online database. Then Skyla could log in from her phone, add or edit a recipe, and tap Save — with no downloads, file transfers, or GitHub steps.

## Publish on GitHub Pages
Keep `index.html`, `recipes.json`, and the recipe photo file together in the repository root. In GitHub, open **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
