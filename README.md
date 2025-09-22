# Sacred Spaces — Mining Tourism Innovation Summit 2025 (Group 13)

This repository hosts Group 13's sprint workspace for the 2025 Mining Tourism Innovation Summit. We are prototyping respectful visitor experiences for post-mining landscapes that hold cultural significance, weaving community knowledge with spatial data, quick-turn analytics, and storytelling assets.

**Using this template?** Keep [TEMPLATE_GUIDE.md](TEMPLATE_GUIDE.md) handy—it's the checklist we followed to swap in the new project name, links, and navigation.

---

## 1) Understanding the repository

Treat this space like a shared online studio. Everything your team needs for the sprint lives here:

* **README.md** — You are here. It explains how the project is organized and how to contribute quickly.
* **code/** — Python/R notebooks, scripts, and utilities that support analyses or visualizations.
* **docs/** — Markdown content that powers the public website at [`https://cu-esiil.github.io/sacred-spaces-mining-tourism-innovation-summit-2025__13/`](https://cu-esiil.github.io/sacred-spaces-mining-tourism-innovation-summit-2025__13/).
* **documentation/** — Longer-form internal notes (meeting summaries, brainstorming logs, etc.). Summarize highlights on the public site when ready.
* **containers/** — Optional recipes for reproducible environments if you need them later in the sprint.

### Storage quick reference

- **Code (`code/`)** — Keep filenames descriptive and add short docstrings or README snippets so others can rerun work.
- **Documentation (`docs/` & `documentation/`)** — Public storytelling lives in `docs/`; private or in-progress details go in `documentation/`.
- **Data (`data/`)** — Only small, shareable datasets belong here. Use CyVerse (see persistent-storage instructions) for larger assets.

---

## 2) How to update the website

Every page on the site corresponds to a Markdown file in `docs/`. When you edit these files on `main`, GitHub Actions rebuilds and deploys the MkDocs site automatically.

### Make a quick update

1. Open the [`docs/`](docs/) folder in GitHub.
2. Click `index.md` (the homepage) or another page you want to edit.
3. Use the pencil icon (✏️) to open the editor.
4. Adjust the text, swap images (upload to `docs/assets/` first), or update links.
5. Write a short commit message like `update day 1 brainstorm`.
6. Choose **Commit directly to the `main` branch** and click **Commit changes**.

> Tip: Need a new section? Create a Markdown file in `docs/`, then add it to the navigation in `mkdocs.yml` if you want it in the top menu.

### Enable/verify publishing

If the site has not been published yet:

1. Go to **Settings → Pages**.
2. Under **Build and deployment**, confirm **Source** is set to **GitHub Actions**.
3. Trigger the "Deploy site (MkDocs)" workflow from the **Actions** tab if a build hasn't run yet.

---

## 3) How to share code

All sprint code should live in the `code/` directory. Create subfolders by topic if it helps (e.g., `code/analysis/`, `code/viz/`).

### Browser upload or edit

1. Open the [`code/`](code/) folder.
2. Click **Add file → Create new file** or **Upload files**.
3. Name the file clearly (e.g., `community_layers.ipynb`, `tourism_scenarios.py`).
4. Add a short header describing inputs/outputs.
5. Commit with a message like `add visitation scenario notebook`.

### Local workflow (optional)

If you prefer working locally or inside CyVerse JupyterLab:

```bash
# Clone once (replace with your fork if needed)
git clone https://github.com/CU-ESIIL/sacred-spaces-mining-tourism-innovation-summit-2025__13.git
cd sacred-spaces-mining-tourism-innovation-summit-2025__13

# Regular workflow
git pull origin main
# ...edit files...
git add code/my_script.py docs/index.md
git commit -m "Add baseline map and update homepage"
git push origin main
```

---

## 4) Common tasks

* **Add a new webpage:** Create a `.md` file in `docs/` (for example, `docs/methods.md`) and add it to `mkdocs.yml`.
* **Highlight data sources:** Update `docs/data.md` with links, access notes, and contacts.
* **Update the team section:** Edit `docs/team.md` (or the "Team" section on the homepage) with names, roles, and preferred contact info.
* **Embed visuals:** Place images in `docs/assets/` and reference them in Markdown with `![caption](assets/filename.png)`.

---

## 5) Tips for beginners

* Version history is your safety net—small commits are welcome.
* Write commit messages that help "future you" remember what changed.
* Keep large files (over ~50 MB) out of GitHub. Use the CyVerse persistent storage link in the site navigation instead.
* When in doubt, leave notes in `documentation/group-notes.md` so teammates know what you tried.

---

## 6) Learn more

* [MkDocs Material documentation](https://squidfunk.github.io/mkdocs-material/)
* [GitHub Pages + MkDocs guide](https://www.mkdocs.org/user-guide/deploying-your-docs/#github-pages)
* [Editing files on GitHub](https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files)

---

## 7) First things to try

1. Update `docs/index.md` with your project one-liner and Day 1 notes.
2. Add your name and role to the team table.
3. Drop your first notebook or script into `code/` and link it from the **Code** page.
4. Post a visual (photo, map, plot) so the homepage tells your story at a glance.

---

## Beginner mode: build the site without the command line

This walkthrough is for teammates who prefer working entirely in the browser.

### What you need

* A GitHub account (free). Sign up at [github.com](https://github.com/).
* Access to this repository: [`https://github.com/CU-ESIIL/sacred-spaces-mining-tourism-innovation-summit-2025__13`](https://github.com/CU-ESIIL/sacred-spaces-mining-tourism-innovation-summit-2025__13).

### Step 1 — Accept your invite

1. Open the invitation link sent by email or via GitHub notifications.
2. Click **Accept invitation** so you can edit the project files.

### Step 2 — Browse the repository

1. Visit the repository link above.
2. Explore folders like `docs/`, `code/`, and `documentation/` to see what's inside.

### Step 3 — Publish (or verify) the website

1. Click **Settings** → **Pages**.
2. Ensure **Source** is set to **GitHub Actions** (this repository ships with an action that builds MkDocs).
3. Once a deploy finishes, your site will live at [`https://cu-esiil.github.io/sacred-spaces-mining-tourism-innovation-summit-2025__13/`](https://cu-esiil.github.io/sacred-spaces-mining-tourism-innovation-summit-2025__13/).

### Step 4 — Edit the homepage

1. Return to the **Code** tab → open `docs/` → click `index.md`.
2. Hit the pencil icon to edit.
3. Replace the placeholder hero text with your own summary.
4. Add at least one visual by uploading an image to `docs/assets/` and referencing it.
5. Commit the changes with a clear message.

### Step 5 — See your updates online

1. Go back to **Settings → Pages** and open the deployed site.
2. Refresh after a minute or two if the changes are not visible yet (builds usually finish quickly).

### Step 6 — Add another page

1. From the **Code** tab choose **Add file → Create new file**.
2. Name it something like `docs/community.md` and add a short outline.
3. Commit the file, then open `mkdocs.yml` to add it under the navigation if you want it in the menu.

### Step 7 — Add an image or downloadable asset

1. Upload your asset to `docs/assets/`.
2. Reference it in Markdown, for example `![Adit entrance](assets/adit.jpg)` or `[Download the brief](assets/brief.pdf)`.

Congratulations—you just shipped updates to the Sacred Spaces sprint site without leaving your browser!
