# Skyla's Kitchen — family recipe book

A polished, mobile-friendly family recipe website with recipe photos, categories, search, and individual shareable recipe pages.

## Public visitors
Family and friends can:
- Browse all published recipes
- Search by recipe name or ingredient
- Filter by category
- Open and share individual recipe links

There is no public Add Recipe button or public recipe submission form.

## Skyla's owner area
The header has one **Owner login** button. Skyla can sign in there to add, edit and delete recipes, upload photos, and export/import the collection.

### Set the owner password before publishing
1. Open `index.html` in a text editor.
2. Find `const OWNER_PASSWORD = "CHANGE-THIS-PASSWORD";`
3. Replace `CHANGE-THIS-PASSWORD` with a password of your choice.
4. Save and upload the updated `index.html` to GitHub.

**Important security limitation:** This is a static GitHub Pages website. A password checked in browser JavaScript is only a casual deterrent; anyone technically confident can inspect the public source and discover it. It is not secure authentication. For genuinely private owner-only editing, the site needs server-side authentication and a database (for example, Supabase Auth + database/storage). Do not use a valuable password here or store sensitive information.

## How recipes are saved and published
- Recipes added by Skyla are saved in that browser on that device.
- Choose **Owner login → Export recipe book** to download `recipes.json`.
- Upload/replace `recipes.json` in the root of the GitHub repository to publish the latest collection to everyone.
- To move the collection to another device, use **Import recipe book** and select the latest `recipes.json`.

GitHub Pages is static hosting and does not itself provide a secure shared editor or synchronise browser edits between devices.

## Publish on GitHub Pages
Upload these files to the repository root:
- `index.html`
- `recipes.json`

Then go to **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, and save. Share the published GitHub Pages URL with family and friends.


## Owner password and security

The owner password currently set in this version is `lilfuck`. This is a simple front-end gate only: because GitHub Pages serves static files, it is not secure authentication and someone with technical knowledge could inspect or bypass it. Do not reuse this password for any important account.
