# 📄 CE7: CSS Grid Layout

Use CSS Grid to turn a page of stacked boxes into four multi-column layouts: two columns,
a row that spans both columns, a column that spans two rows, and a custom three-column grid
you build on your own.

**Points:** 10

## 🎯 Overview

In this coding exercise, you will start with a page that already has all of its HTML and
some basic styling. Every box on the page is stacked on top of the next one. Your job is to
write the CSS that arranges those boxes into grids.

Part 1 is a follow-along video that walks you through the first three layouts. Part 2 is
**on your own**: you will use what you learned to build the final three-column layout
without a step-by-step demonstration.

Almost all of your work happens in `grids.css`. You will only touch the HTML to add class
names and one new section.

> [!IMPORTANT]
> **The companion videos for this exercise are in Canvas**, on the assignment page. They
> walk you through Part 1 step by step, so watch them there instead of working from this
> file alone.

## 📋 Requirements

1. **Rename `grid-examples.html` to `index.html`.** This is required. GitHub Pages only
   serves `index.html` at your site's root URL, so any other name gives you a 404. Rename
   the existing file. Don't create a new `index.html` alongside it.
2. **Complete Part 1** by following the *Coding Exercise — Part 1* video to build the
   *2 Columns*, *2 Columns and a Row That Spans Both*, and *Right Column Spans 2 Rows*
   layouts.
3. **Complete Part 2 on your own** by following the four steps in the
   *Part 2 — On Your Own* section below, or in the
   [Part 2 PDF](.github/Part-2.pdf).
4. **Publish and submit** your page as described in the [README](README.md).

## 🧠 What You Will Learn

By completing this exercise, you will practice how to:

- Turn an element into a grid container with `display: grid`
- Define columns with `grid-template-columns` and the `fr` unit
- Make some columns wider or narrower than others
- Add space between grid items with `gap`
- Make a grid item span more than one column with `grid-column`
- Make a grid item span more than one row with `grid-row`
- Apply more than one class to a single HTML element
- Explain the difference between a grid **container** and the grid **items** inside it

## 🎬 Watch the Videos in Canvas and Follow Along

The screencast videos are on this assignment's page in **Canvas**, not in this repo. Watch
them **in order** and follow along in your code editor. Pause whenever you need time to
finish a step. It is normal to pause, rewind, and rewatch parts of a coding demonstration.

| Video | What you will do |
| --- | --- |
| **Coding Exercise — Part 1** | Follow along to build the first three layouts on the page: *2 Columns*, *2 Columns and a Row That Spans Both*, and *Right Column Spans 2 Rows*. |
| **Part 2 — On Your Own** | An introduction to the final *3 Columns* section, which you complete yourself using the four steps below. |

> [!NOTE]
> These are older videos. They show **Brackets** as the code editor, but you should use
> **Visual Studio Code**. The editor will look different, but your final code will be
> exactly the same.

> [!IMPORTANT]
> **A few steps in this repo are different from the videos.** Follow the videos for the
> CSS, and follow this repo for getting your files and submitting:
>
> - **Getting the starter files:** don't download `grids_start.zip`. Create your own repo
>   from this template and open it with GitHub Desktop, as described in the
>   [README](README.md#-getting-started).
> - **Naming your file:** rename `grid-examples.html` to **`index.html`**, whatever name
>   the video uses. GitHub Pages only serves `index.html` at your site's root URL; any
>   other name gives you a 404. Rename the file — don't create a second one.
> - **Submitting:** don't zip your folder or upload a file. Publish your page to GitHub
>   Pages and submit a pull request URL in Canvas, as described in the
>   [README](README.md#-submitting-the-assignment).

## ✍️ Part 2 — On Your Own

These steps come from the [Part 2 PDF](.github/Part-2.pdf) in Canvas, which shows a
screenshot of the section after each step. Open it to check your work as you go.

All four steps apply to the **same** section: the final *3 Columns* section at the bottom
of the page (`.container-3col`). They are not four separate sections to create. Each step
builds on the one before it.

1. **Make a grid that has 3 columns where the first and last columns are wider and the
   middle column is narrower.**
2. **Add a grid gap of `.5em`** so there is space between the columns.
3. **Add a fourth section to the grid.** Copy one of the existing `<section class="column">`
   blocks inside `.container-3col`, paste it as the last item, and give it different text.
   It will wrap onto a new row and fill only the first column.
4. **Make the bottom section span three columns** so the fourth section stretches across
   the full width of the grid.

When you are finished, the section should look roughly like this:

```
3 Columns
┌───────────────────┐ ┌──────┐ ┌───────────────────┐
│                   │ │      │ │                   │
│      wide         │ │narrow│ │      wide         │
│                   │ │      │ │                   │
└───────────────────┘ └──────┘ └───────────────────┘
┌───────────────────────────────────────────────────┐
│          fourth section spans all three           │
└───────────────────────────────────────────────────┘
```

## 📂 Starter Files

| File | Purpose |
| --- | --- |
| `grid-examples.html` | The page content. **Rename this to `index.html`.** Add class names and the fourth section here. |
| `grids.css` | Your grid styles. Fill in `.container-2col` and `.container-3col`, and write any new selectors under `/* add new selectors below */`. |
| `reset.css` | Removes default browser styles. **Don't edit this file.** |

Comments in the starter files point to where you will be working. For example, the
*Right Column Spans 2 Rows* section has an `<!-- add a second class -->` comment on the
section that needs a second class name. When an element has more than one class, put a
space between the class names:

```html
<section class="column span-vert">
```

> [!IMPORTANT]
> Open the entire project **folder** in VS Code, not a single HTML file. Keep `index.html`,
> `grids.css`, and `reset.css` together in the root folder so the stylesheet links keep
> working.

## 🧮 Grading Rubric

| Criteria | Full credit looks like | Points |
| --- | --- | --- |
| **Setup** | `grid-examples.html` is renamed to `index.html`. `index.html`, `grids.css`, and `reset.css` are in the root folder, and both stylesheets load on the live page. | 1 |
| **2 Columns** | The two sections in the first example sit side by side in two equal columns. | 1 |
| **Row That Spans Both** | The second example is a two-column grid, and one section stretches across both columns. | 1 |
| **Right Column Spans 2 Rows** | The third example is a two-column grid, and the right-hand section uses a second class to span two rows. | 1 |
| **Part 2, Step 1 — Wide / Narrow / Wide** | `.container-3col` is a grid with three columns. The first and last columns are wider than the middle column. | 1 |
| **Part 2, Step 2 — Gap** | The three-column grid has a gap of `.5em` between its items. | 1 |
| **Part 2, Step 3 — Fourth Section** | A fourth `section` with the `column` class has been added inside `.container-3col`. | 1 |
| **Part 2, Step 4 — Span Three Columns** | The fourth section spans all three columns of the grid. | 1 |
| **Code Quality** | Grid styles are written in `grids.css`, not inline in the HTML. `reset.css` is unchanged. The page's existing content and other styles are intact. | 1 |
| **Published & Submitted** | The page is live on GitHub Pages, and the pull request into `main` has every section of its template filled in. | 1 |
| | **Total** | **10** |

Each criterion is graded on the live GitHub Pages site. It earns its full point when it
matches the *Full credit looks like* column. Half credit may be given for a layout that is
close but not quite right, such as three columns that are all the same width in Step 1.

## ✅ Before You Submit

Check the following:

- [ ] `grid-examples.html` has been renamed to `index.html`
- [ ] `index.html`, `grids.css`, and `reset.css` are all in the root folder of the repo
- [ ] The *2 Columns* example shows two side-by-side columns
- [ ] The *2 Columns and a Row That Spans Both* example has one section spanning both columns
- [ ] The *Right Column Spans 2 Rows* example has its right column spanning two rows
- [ ] The *3 Columns* grid has wide, narrow, and wide columns
- [ ] The *3 Columns* grid has a `.5em` gap
- [ ] The *3 Columns* grid has a fourth section that spans all three columns
- [ ] You saved both `index.html` and `grids.css`
- [ ] The page is live on GitHub Pages and the URL is in your pull request

## 🛠️ Troubleshooting

If something is not working, check these common issues first:

- Did you save **both** files? It's easy to save the HTML and forget the CSS.
- Is the file named exactly `index.html`?
- Is `display: grid` on the **container** (the outer `section`), not on the columns inside it?
- Are the columns you want in a grid actually **inside** that container in the HTML?
- Does every class name in your HTML match the selector in your CSS exactly, including
  spelling and capitalization? Remember that CSS selectors for classes start with a `.`.
- When you added a second class, is there a **space** between the two class names?
- Did your new selectors end up inside another rule's curly braces? Check that every `{`
  has a matching `}`.
- Is every property followed by a colon and every value followed by a semicolon?

**Having problems with the videos?**

- **Getting a warning about third-party cookies?** Try using Chrome. Safari's default
  security settings may prevent embedded Canvas videos from playing unless those settings
  are changed.
- **Getting an "Access Denied" error?** Refresh your browser. In many cases, the videos
  will load correctly after the page reloads.

## 📚 Resources

- [Part 2 — On Your Own (PDF)](.github/Part-2.pdf) — the four Part 2 steps with screenshots
- [MDN — CSS grid layout](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout/Grids)
- [MDN — Basic concepts of grid layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout/Basic_concepts_of_grid_layout)
- [MDN — `grid-template-columns`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-template-columns)
- [MDN — `grid-column`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-column) and
  [`grid-row`](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-row)
- [CSS-Tricks — CSS Grid Layout Guide](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [Grid Garden](https://cssgridgarden.com/) — a game for practicing grid properties
- [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/#validate_by_input) —
  paste your CSS in to catch missing braces and semicolons

---

The AI policy and submission instructions are in the [README](README.md).
