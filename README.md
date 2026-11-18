# Skii-la's Kitchen

A simple static family recipe website for GitHub Pages.

## Website files

- `index.html` — the website and owner editing area
- `recipes.json` — the complete published recipe collection
- `photos/1.jpg`, `photos/2.jpg`, etc. — recipe pictures, with numbers matching recipe IDs

The recipe cards are shown newest first (highest recipe number first).

## Sending updates from Skii-la's phone

1. Skii-la logs in and edits/adds recipes as usual.
2. Tap **Download to send to your sweet boy**.
3. The ZIP contains the complete updated `recipes.json`, a `changes.txt` guide, and only photos that are new or have been replaced since the last confirmed publish.
4. Matthew uploads/replaces `recipes.json` at the website root and uploads/replaces any included files inside the existing `photos` folder. A changed old photo keeps its number, so uploading `photos/2.jpg` replaces the old `photos/2.jpg`.
5. After the upload is confirmed, Skii-la taps **I've uploaded the changes** on her phone. This marks the exported photo changes as published so they will not be sent again next time.

If the ZIP is exported again before the changes are marked as published, the changed photos are included again. This is intentional, so a missed upload is not silently forgotten.

Deleted recipes disappear from `recipes.json`. Their old image files can be left on GitHub; they are harmless unused files and do not need to be deleted manually.

## Refreshing a device

**Use the live website recipes** downloads the current public `recipes.json` and replaces the recipes saved on that device. It discards local edits that have not been exported, so export first.

## Important note about owner login

The password gate is a convenience only. Because this is a static website, the password is visible in the website source and is not secure server-side authentication. Do not use it to protect sensitive information.
