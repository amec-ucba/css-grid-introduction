# 💻 Assignment Boilerplate

A starting point for assignment and exercise repos. It includes submission instructions, editor and Git configuration, and a pull request template so every assignment works the same way.

> [!NOTE]
> `.editorconfig`, `.gitattributes`, `.gitignore`, `.noai`, and the `.github` folder are
> setup files that keep assignments consistent. Leave them alone.

## 📋 Assignment Requirements

> [!IMPORTANT]
> **Start here: [read ASSIGNMENT.md →](ASSIGNMENT.md)**

It has the requirements, grading criteria, and due date. Read it before you start, and check it again before you submit. This `README` only covers how to publish and submit your work.

## 🏁 Getting Started

1. **Create your own repo from this template.**
   - At the top of this repo on GitHub, click the green **Use this template** button. (If a
     menu opens, choose **Create a new repository**.)

     <img src=".github/images/use-this-template.png" alt="The Use this template button at the top right of the repo page" width="600">
   - Set **Owner** to your GitHub account.
   - Give it a **Repository name** — use the assignment name, like `assignment-1`.

     <img src=".github/images/create-repo-name.png" alt="The Create a new repository form with Owner set to your username and the Repository name filled in" width="600">
   - Set visibility to **Public** (GitHub Pages needs a public repo on a free account).

     <img src=".github/images/create-repo-visibility.png" alt="The Choose visibility dropdown set to Public" width="600">
   - Click **Create repository**. GitHub takes you to your new repo.
2. **Open your new repo in GitHub Desktop.**
   - Check that the repo name at the top of the page is `<your-username>/<repo-name>`, not
     this template.
   - Click the green **Code** button → **Open with GitHub Desktop**.
   - GitHub Desktop opens and asks where to save the repo. Pick a folder on your computer
     and click **Clone**.

   <img src=".github/images/code-open-with-github-desktop.png" alt="The Code menu with Open with GitHub Desktop near the bottom" width="600">

   <img src=".github/images/github-desktop-clone.png" alt="GitHub Desktop's Clone a Repository dialog with the repo URL and Local Path filled in, and the Clone button highlighted" width="600">
3. In GitHub Desktop, create your assignment branch: **Current Branch** → **New Branch** and name it `develop`.
4. Click **Open in \<editor\>** to open the folder in your code editor and start working.

## 📂 Where Your Files Go

Create your files in the **root folder** of this repo — the same folder as this README.
GitHub Pages publishes from the root, so `index.html` has to live there or your site will 404. Group your assets into subfolders:

```
index.html
css/style.css
js/script.js
images/photo.jpg
```

## 🤖 AI Policy

Work on this assignment must be your own. Do not use AI coding assistants — including
GitHub Copilot, Cursor, ChatGPT, Claude, or JetBrains AI Assistant — to generate,
complete, or rewrite your code.

You should be able to explain any line of your submission. You may be asked to do so.

This repo includes a `.noai` file, which disables JetBrains AI Assistant for the project
in IDEs like WebStorm. Leave it in place. It is a reminder of the policy above, not a
substitute for it — following the policy is still your responsibility.

## 🚀 Publishing to GitHub Pages

Your work has to be live on the web before you can submit it.

1. **Commit your work in GitHub Desktop.**
   - Make sure **Current Branch** says `develop`.
   - Enter a summary in the bottom-left box, like `Create index.html`, and click
     **Commit to develop**.

   <img src=".github/images/github-desktop-commit.png" alt="GitHub Desktop's Changes tab with the Current Branch dropdown showing develop, a commit summary entered, and the Commit to develop button highlighted" width="600">
2. **Push your work to GitHub.**
   - The first time, click **Publish branch** at the top. This creates your `develop`
     branch on GitHub.
   - After that, the same button says **Push origin**. Click it after every commit.

   <img src=".github/images/github-desktop-publish-branch.png" alt="GitHub Desktop toolbar with the Publish branch button highlighted" width="600">
3. **Turn on GitHub Pages.**
   - On GitHub, open **your** repo (the one you created from the template) and go to
     **Settings** → **Pages**.
   - Under **Branch**, click the **None** dropdown and pick `develop`.

     <img src=".github/images/pages-select-branch.png" alt="The Pages branch dropdown open with develop highlighted" width="600">
   - Make sure **Source** is *Deploy from a branch* and the folder is `/ (root)`, then click
     **Save**.

     <img src=".github/images/pages-source-and-branch.png" alt="Pages settings with Source set to Deploy from a branch, and develop, / (root), and Save highlighted" width="600">
4. **Open your live site.** The first deploy takes a minute or two. Reload the Pages
   settings screen until it says **Your site is live at**, then click the URL:
   ```
   https://<your-username>.github.io/<repo-name>/
   ```

   <img src=".github/images/pages-site-live.png" alt="The Your site is live at banner with the site URL highlighted" width="600">

   Confirm the page loads correctly — the right content, no missing images, no broken styles.

**🛠️ Troubleshooting**

- **404 page:** make sure an `index.html` exists in the root of the branch you selected, and that the filename is lowercase.
- **Old version showing:** Pages caches aggressively. Wait a minute, then hard refresh (<kbd>Cmd</kbd>/<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>R</kbd>).
- **Nothing deployed:** check the **Actions** tab for a failed `pages build and deployment` run.

## 📬 Submitting the Assignment

Submission has two parts: publish the site, then submit a pull request URL in Canvas.

1. **Publish to GitHub Pages** using the steps above. Do this first.
2. **Open a pull request into `main`.**
   - In **GitHub Desktop**, with `develop` selected, click **Preview Pull Request**, then
     **Create pull request**. (You can also use **Branch** → **Create Pull Request**.) The
     pull request form opens in your browser.

     <img src=".github/images/github-desktop-preview-pr.png" alt="GitHub Desktop with the Preview Pull Request button highlighted" width="600">
   - Confirm **base** is `main` and **compare** is `develop`, and title it with the
     assignment name.

     <img src=".github/images/pr-base-compare-title.png" alt="The Open a pull request form with base main, compare develop, and the title highlighted" width="600">
   - The description is pre-filled with a template. Fill in every section: paste your live
     GitHub Pages URL under **Live GitHub Pages URL**, write a short **Summary**, check off
     the **Checklist** by changing each `[ ]` to `[x]`, and answer the **Reflection**.
     **Notes for your instructor** is optional. Leave the `<!-- -->` hint lines as they are;
     they're hidden once the pull request is created.

     <img src=".github/images/pr-description.png" alt="The pull request description template filled in, with the GitHub Pages URL highlighted" width="600">
   - Click **Create pull request**.

     <img src=".github/images/pr-create-button.png" alt="The Create pull request button highlighted" width="600">
   - Your pull request opens. It should say **Open** and show it merging `develop` into
     `main`. Don't merge it.

     <img src=".github/images/pr-opened.png" alt="An open pull request merging develop into main, with the Open status highlighted" width="600">
3. **Submit the pull request URL in Canvas.**
   - Copy the pull request URL from your browser's address bar. It looks like
     `https://github.com/<your-username>/<repo-name>/pull/1`.
   - Open the matching assignment in Canvas and click the red **Start Assignment** button.
     The page scrolls down to the submission form.

     <img src=".github/images/canvas-start-assignment.png" alt="The Canvas assignment page with the Start Assignment button highlighted" width="600">
   - On the **Website URL** tab, paste your **pull request URL** into the **Website URL**
     field. Don't paste your GitHub Pages URL here; that goes in the pull request.
   - Optional: add a note for your instructor in **Comments**.
   - Click the red **Submit Assignment** button.

     <img src=".github/images/canvas-submit-url.png" alt="The Canvas Website URL form with a pull request URL entered, a comment for the instructor, and the Submit Assignment button highlighted" width="600">

> [!CAUTION]
> Late or missing submissions are graded on what is in the pull request at the deadline, so push your final commits before you submit.
