# 🏁 Getting Started

[← Back to the README](../README.md)

Do these steps once at the start of every assignment.

> [!TIP]
> **First assignment?** Do the [one-time WebStorm setup](WEBSTORM_SETUP.md) first.

## 1. Create your own repo from this template

- At the top of this repo on GitHub, click the green **Use this template** button. (If a
  menu opens, choose **Create a new repository**.)

  <img src="images/use-this-template.png" alt="The Use this template button at the top right of the repo page" width="600">

- Set **Owner** to your GitHub account.
- Give it a **Repository name** — use the assignment name, like `css-grid-introduction`.

  <img src="images/create-repo-name.png" alt="The Create a new repository form with Owner set to your username and the Repository name filled in" width="600">

- Set visibility to **Public** (GitHub Pages needs a public repo on a free account).

  <img src="images/create-repo-visibility.png" alt="The Choose visibility dropdown set to Public" width="600">

- Click **Create repository**. GitHub takes you to your new repo.

## 2. Clone your new repo in WebStorm

- On the WebStorm welcome screen, click **Clone Repository**. (If a project is already
  open, use **File** → **New** → **Project from Version Control…**)
- Click **GitHub** on the left. Pick `<your-username>/<repo-name>` from the list, not
  this template.
- Check the **Directory** it will save to, then click **Clone**.

  <img src="images/webstorm-clone-github.png" alt="The Clone Repository dialog on the GitHub tab with a repo selected, and the Clone into directory and Clone button highlighted" width="600">

- If WebStorm asks whether to trust the project, click **Trust Project**.

  <img src="images/webstorm-trust-project.png" alt="The Trust and Open Project dialog with the Trust Project button highlighted" width="500">

## 3. Create your `develop` branch

- Click the branch name (`main`) at the top left of the window, then **New Branch…**

  <img src="images/webstorm-new-branch-menu.png" alt="The branch widget menu open from main, with the branch widget and New Branch highlighted" width="500">

- Name it `develop`, leave **Checkout branch** checked, and click **Create**.

  <!-- SCREENSHOT: webstorm-new-branch.png — Create New Branch dialog with the name develop, Checkout branch checked, and Create highlighted -->

- The top left should now say `develop`. **Check this before your first commit.** Work
  committed to `main` can't go in your pull request.

## 4. Preview your page while you work

Open `index.html` and hover over the top right of the editor. Click the WebStorm icon for
the built-in preview, or a browser icon to open it in that browser. The page reloads every
time you save.

<img src="images/webstorm-preview-icons.png" alt="The browser icons in the top right of the editor, with the built-in WebStorm preview icon highlighted" width="600">

---

**Next:** [Publishing to GitHub Pages →](PUBLISHING.md)
