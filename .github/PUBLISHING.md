# 🚀 Publishing to GitHub Pages

[← Back to the README](../README.md)

Your work has to be live on the web before you can submit it. Commit and push as you
work, then turn on GitHub Pages once.

## 1. Commit your work in WebStorm

- Make sure the branch name at the top left says `develop`.
- Press <kbd>Cmd</kbd> + <kbd>K</kbd> to open the **Commit** panel. Check the files you
  want to include.
- Type a short message describing the change, like `Create index.html`, and click **Commit**.

  <img src="images/webstorm-commit.png" alt="The Commit tool window with index.html, style.css, and photo.jpg checked, a commit message entered, and the Commit button highlighted; the branch widget shows develop" width="600">

- **First commit only:** WebStorm asks for your **Name** and **Email**. Use your **UC email** (the one on your
  GitHub account) so your commits show up as yours. Leave **Set properties globally** checked and click **Set and
  Commit**. It won't ask again.

  <img src="images/webstorm-git-identity.png" alt="The Git User Name Is Not Defined dialog with the Name and E-mail fields and the Set and Commit button highlighted" width="400">

- **If WebStorm says it found problems:** before each commit, WebStorm checks your code.
  If it finds errors or warnings, it stops and asks what to do.
    - Click **Review** to see the list. Double-click a problem to jump to it. Common ones
      are a misspelled image path, a missing `alt`, or a typo in a CSS property.
    - Fix what you can, then commit again.
    - If you've checked and want to commit anyway (for example, to save work in
      progress), click **Commit Anyway**. Your commit still goes through.

  <img src="images/webstorm-commit-checks.png" alt="The Commit contains problems notification with the Review code analysis and Ignore links highlighted" width="500">

- Commit often: every time you finish a piece of the page, not once at the end.

## 2. Push your work to GitHub

- Press <kbd>Cmd</kbd> + <kbd>Shift</kbd> + <kbd>K</kbd>. The **Push** dialog shows
  `develop → origin : develop` and the commits that will be sent.
- Click **Push**. The first push creates your `develop` branch on GitHub.

  <img src="images/webstorm-push.png" alt="The Push dialog showing develop → origin : develop with the Push button highlighted" width="600">

- Push after every commit (or click **Commit and Push** in the Commit panel to do both
  at once).

## 3. Turn on GitHub Pages

- On GitHub, open **your** repo (the one you created from the template) and go to **Settings** → **Pages**.
- Under **Branch**, click the **None** dropdown and pick `develop`.

  <img src="images/pages-select-branch.png" alt="The Pages branch dropdown open with develop highlighted" width="600">

- Make sure **Source** is *Deploy from a branch* and the folder is `/ (root)`, then click **Save**.

  <img src="images/pages-source-and-branch.png" alt="Pages settings with Source set to Deploy from a branch, and develop, / (root), and Save highlighted" width="600">

## 4. Open your live site

The first deploy takes a minute or two. Reload the Pages settings screen until it says
**Your site is live at**, then click the URL:

```
https://<your-username>.github.io/<repo-name>/
```

<img src="images/pages-site-live.png" alt="The Your site is live at banner with the site URL highlighted" width="600">

Confirm the page loads correctly — the right content, no missing images, no broken styles.

## 🛠️ Troubleshooting

- **404 page:** make sure an `index.html` exists in the root of the branch you selected, and that the filename is
  lowercase.
- **Old version showing:** Pages caches aggressively. Wait a minute, then hard refresh
  (<kbd>Cmd</kbd>/<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>R</kbd>).
- **Nothing deployed:** check the **Actions** tab for a failed `pages build and deployment` run.

---

**Next:** [Submitting the Assignment →](SUBMITTING.md)
