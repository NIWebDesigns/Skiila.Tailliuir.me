# Skii-la's Kitchen

A simple static family recipe website for GitHub Pages.

## Website files

- `index.html` — the website and owner editing area
- `recipes.json` — the complete published recipe collection
- `photos/1.jpg`, `photos/2.jpg`, etc. — recipe pictures, with numbers matching recipe IDs

The recipe cards are shown newest first (highest recipe number first).

## Simple steps for Skii-la

1. **Start fresh:** tap **Step 1 — Load the current website**. This clears the saved working copy on that phone and loads the recipes currently online. Do this before editing.
2. **Make changes:** add a recipe, or open an existing recipe and choose **Edit recipe**.
3. **Send the update:** tap **Step 3 — Download my update**, then send the downloaded ZIP file to Matthew in your usual messages. Do not open the ZIP.
4. **Reset after Matthew confirms:** only after Matthew says the update is online, tap **Step 4 — Clear my updates and reload the website**. This replaces the phone's saved working copy with the newly published recipes.

Important: Step 1 and Step 4 replace the saved recipes on that phone with the live `recipes.json`. Any edits not yet sent to Matthew will be lost. If the live website cannot be reached, the saved copy is left untouched.

## Steps for Matthew to publish an update

1. Open the ZIP sent by Skii-la.
2. Upload/replace `recipes.json` at the website root.
3. Upload/replace each photo listed in `changes.txt`, keeping it inside the `photos` folder. A changed old photo keeps its number, so `photos/2.jpg` replaces the old `photos/2.jpg`.
4. Do not delete any other photos. Old unused photos can safely be left in place.
5. After confirming the live website has updated, tell Skii-la she can tap **Step 4 — Clear my updates and reload the website**. This replaces her phone’s local working copy with the newly published recipes.

The ZIP always contains the complete updated `recipes.json` and only new or changed photos. If it is exported again before the changes are marked as published, changed photos are included again intentionally, so a missed upload is not silently forgotten.

Deleted recipes disappear from `recipes.json`. Their old image files can be left on GitHub; they are harmless unused files and do not need to be deleted manually.

## Important note about owner login

The password gate is a convenience only. Because this is a static website, the password is visible in the website source and is not secure server-side authentication. Do not use it to protect sensitive information.
