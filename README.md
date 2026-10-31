# Publish RuKaiKai on GitHub Pages

This package is already built for:

**https://curiousavery.github.io/rukaikai/**

You do not need Node.js, Ollama, or a terminal to publish it. Ollama is only
needed by people who download and run the separate local edition.

GitHub cannot publish the ZIP file itself. Extract it first, then upload the
files inside the extracted folder as described below.

## Before you upload

The GitHub repository must be named **`rukaikai`** exactly. GitHub Pages paths
are case-sensitive, and this build expects `/rukaikai/` in every asset URL.
Do not use this package for a root-level `curiousavery.github.io` repository;
that kind of site requires a separate build whose base path is `/`.

After extracting `rukaikai-github-pages.zip`, open the
`rukaikai-github-pages` folder. Its top level should contain `index.html`,
`assets`, `brand`, `downloads`, and this `README.md`. Upload these items to the
repository root. Do not upload the enclosing `rukaikai-github-pages` folder as
one extra directory.

## First-time setup using the GitHub website

1. Sign in to the **curiousavery** account at [github.com](https://github.com/).
2. Select **New repository** from the **+** menu.
3. Enter **`rukaikai`** as the repository name.
4. Choose **Public**. Leave the optional README, `.gitignore`, and license boxes
   unchecked, then select **Create repository**.
5. On the empty repository page, choose **uploading an existing file**. If the
   repository already exists, choose **Add file → Upload files** instead.
6. Drag everything *inside* the extracted `rukaikai-github-pages` folder into
   the upload area. The repository root must contain `index.html` directly.
7. Enter a message such as `Deploy RuKaiKai site`, then select
   **Commit changes**.
8. Open **Settings → Pages**.
9. Under **Build and deployment**, choose **Deploy from a branch**.
10. Select the repository's default branch (usually **main**) and the
    **/(root)** folder, then select **Save**.
11. Allow up to 10 minutes for the first deployment. GitHub will show the public
    address when it is complete. Open
    **https://curiousavery.github.io/rukaikai/**.

The hidden `.nojekyll` file is included in the package. If Finder does not show
it during a manual upload, this particular build will still work because none
of its required folders begins with an underscore.

## Updating the site later

Generate a fresh package, extract it, and upload its contents to the same
repository root. Replace files with matching names and commit the update. The
generated JavaScript and CSS filenames may change between releases; old files
can remain temporarily, but only the files referenced by the new `index.html`
are used.

## Quick checks after publishing

- The RuKaiKai logo appears in the header and introduction.
- The status says **Online source demo**.
- Selecting `qiladju sa kilangda.` shows `Sit back and listen.`.
- **Download the local starter kit** downloads a ZIP file.
- The browser address begins with
  `https://curiousavery.github.io/rukaikai/`.

## If something looks wrong

- **404 page:** confirm the repository is public, Pages uses the branch that
  contains `index.html` and `/(root)`, and allow up to 10 minutes.
- **Page has no styling or images:** confirm the repository is named exactly
  `rukaikai` and that `index.html` is at the repository root.
- **The URL contains an extra folder:** the enclosing
  `rukaikai-github-pages` folder was uploaded instead of its contents. Move its
  contents to the repository root.
- **Pages is using an old GitHub Actions setup:** in **Settings → Pages**, switch
  the source to **Deploy from a branch** for this ready-built package.

## Package integrity

The `.sha256` file beside the downloadable package contains its SHA-256
checksum. Checking it is optional, but it can confirm that the ZIP was copied
without damage.
