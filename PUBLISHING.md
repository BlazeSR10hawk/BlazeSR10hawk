# Publish BlazeSR10hawk as a GitHub profile README

This folder is ready for the **special GitHub profile repository**.

## Website upload — no command line required

1. Sign in to `https://github.com/BlazeSR10hawk`.
2. Open `https://github.com/new`.
3. Set **Repository name** to exactly `BlazeSR10hawk` (same spelling and case as the username).
4. Set it to **Public**. Click **Create repository**. A README auto-initialization is optional; if you check it, replace its default README with the one in this folder.
5. Open **Add file → Upload files** (or **uploading an existing file** in the empty repository).
6. Upload `README.md`, `PUBLISHING.md`, and the entire `assets` directory so that the directory paths are preserved. If your browser loses the folder structure, create the `assets` folder through the web editor or use the git commands below.
7. Commit the changes to `main`.
8. Visit `https://github.com/BlazeSR10hawk` — the profile README should appear on the profile page.

**Important:** The README must be at the root of `BlazeSR10hawk/BlazeSR10hawk`, and `assets/` must remain next to it.

## Git command-line upload

From this folder, after creating the empty public GitHub repository:

```bash
git init
git branch -M main
git add README.md PUBLISHING.md assets/
git commit -m "feat: launch animated BlazeHawk profile README"
git remote add origin https://github.com/BlazeSR10hawk/BlazeSR10hawk.git
git push -u origin main
```

If GitHub created a README during repository setup, clone that repo first, replace its README, add `assets/` and `PUBLISHING.md`, then commit and push normally.

## Asset notes

- `assets/blazehawk-banner.jpg` — static, cinematic hero image.
- `assets/blazehawk-flight.gif` — autoplay loop visible directly in GitHub Markdown.
- `assets/blazehawk-flight.mp4` — original **10-second** video; clicking the GIF opens the video file.
- `assets/blazehawk-avatar.jpg` — user's source GitHub avatar, preserved as an asset.

GitHub does **not** consistently support directly embedded playable MP4 videos in repository README Markdown. The **GIF + MP4 link** approach is the reliable fallback.

No personal access token or secret is required in the README. Do not commit tokens.
