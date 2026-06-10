# My Worldbuilding Wiki

A self-hosted worldbuilding wiki — public-facing site on GitHub Pages, private editor on your own computer.

---

## Files

| File | Purpose |
|---|---|
| `index.html` | Public website (goes on GitHub Pages) |
| `wiki.json` | Your wiki data (also committed to GitHub) |
| `editor.html` | **Private** — open locally to write and edit. Never needs to go on GitHub. |

---

## First-time setup

### 1. Create a GitHub account
Go to https://github.com and sign up if you don't have an account.

### 2. Create a new repository
- Click the **+** in the top-right → **New repository**
- Name it anything (e.g. `my-world`)
- Set it to **Public**
- Click **Create repository**

### 3. Upload your files
- On the repository page, click **Add file → Upload files**
- Upload `index.html` and `wiki.json` (not `editor.html` — that stays on your computer)
- Click **Commit changes**

### 4. Enable GitHub Pages
- Go to your repository **Settings** tab
- Click **Pages** in the left sidebar
- Under **Source**, select **Deploy from a branch**
- Set branch to `main`, folder to `/ (root)`
- Click **Save**
- After a minute or two, your site will be live at:
  `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

---

## Your writing workflow (after setup)

Every time you want to add or edit content:

1. **Open `editor.html`** — double-click it on your computer, it opens in your browser
2. **Write your pages** — changes save automatically to your browser
3. When ready to publish, click **↑ Publish wiki.json** in the bottom-left
4. A `wiki.json` file downloads to your computer
5. **Upload the new `wiki.json` to GitHub:**
   - Go to your repository on github.com
   - Click `wiki.json` in the file list
   - Click the **pencil icon** (Edit) in the top-right
   - You'll see "You are editing a file..." — but instead, click **Cancel**
   - Back on the file, click the **...** menu → **Upload a file** won't work here
   - Easier: go back to the main repo page → **Add file → Upload files**
   - Upload your new `wiki.json` and click **Commit changes**
6. Wait ~1 minute, then refresh your public site — it's updated!

> **Tip:** If you get comfortable with GitHub Desktop (https://desktop.github.com), the upload step becomes "drag file into folder, then click Sync" — much faster.

---

## Notes

- `editor.html` stores your notes in your **browser's local storage**. This is tied to that browser on that computer. Don't clear your browser data for that file. The `wiki.json` you publish is your backup.
- Images you attach in the editor are embedded as base64 inside `wiki.json`. Large images will make the file big — keep attached images under ~1MB each.
- The public site has no login, no tracking, no cookies.

---

## Customising your site title

In `editor.html`, click **⚙ Site settings** to change the title and subtitle. These are saved into `wiki.json` when you publish.
