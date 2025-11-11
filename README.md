# 📝 Shridhan Website – Content Editing Guide

Welcome! 👋
This guide helps you **edit and update website content** stored in Markdown (`.md`) files on GitHub — even if you’ve never coded before.

---

## 🗂️ Repository Overview

All content for the **Shridhan website** is organized into folders:

| Folder      | What it Contains                           | Example                                          |
| ----------- | ------------------------------------------ | ------------------------------------------------ |
| `products/` | Product descriptions, specs, and summaries | `products/magnetic-level-indicators.md`          |
| `events/`   | Event details and write-ups                | `events/annual-conference-2025.md`               |
| `services/` | Descriptions of offered services           | `services/installation-support.md`               |
| `images/`   | Images grouped by category                 | `images/products/magnetic-level-indicators.webp` |

---

## ✍️ Understanding Markdown Files

Each `.md` file has **two main parts**:

1. **Frontmatter** – The data at the top between `---` lines (metadata used by the site).
2. **Body** – The actual text that appears on the website (below the frontmatter).

### Example file

```markdown
---
title: Magnetic Level Indicators (MLIs)
collection: Level Instrumentation
images:
  - magnetic-level-indicators-mlis.webp
summary: Provides clear and reliable visual indication of liquid levels.
sku: LI-MLI-100
---

This is the main body content. You can write multiple paragraphs here.

Here’s another paragraph with more details or examples.
```

> 💡 **Tip:** Frontmatter is metadata — it tells the site how to display title, summary, images, etc.

---

## 🧩 Frontmatter Fields Explained

|         Field | Description                                      | Example                                                           |
| ------------: | ------------------------------------------------ | ----------------------------------------------------------------- |
|      `title:` | Page or product title (appears on the site)      | `Magnetic Level Indicators (MLIs)`                                |
| `collection:` | Content category or group                        | `Level Instrumentation`                                           |
|     `images:` | One or more image filenames from `/images/...`   | `- magnetic-level-indicators-mlis.webp`                           |
|    `summary:` | A short one-line summary                         | `Provides clear and reliable visual indication of liquid levels.` |
|        `sku:` | A unique ID (for products) — **never edit this** | `LI-MLI-100`                                                      |

---

## ✏️ How to Edit a Page (Step-by-Step)

1. **Navigate** to the correct folder (e.g., `products/`).
2. **Open** the `.md` file you want to edit (e.g., `products/magnetic-level-indicators.md`).
3. **Edit** the content:

   * Update the `summary:` line to change the short description.
   * Edit the **main description** in the body (below the second `---`) for long-form content.
4. **Preserve formatting**:

   * Keep the `---` lines exactly as they are.
   * Maintain proper indentation (2 spaces for list items such as `images:`).

✅ Correct indentation example:

```yaml
images:
  - image-one.webp
  - image-two.webp
```

❌ Incorrect indentation example:

```yaml
images:
- image-one.webp
- image-two.webp
```

> ⚠️ Wrong spacing can cause display errors. Always align list items under their heading with two spaces.

---

## 🌟 Golden Rules

| ✅ DO                                                      | ❌ DON’T                                           |
| --------------------------------------------------------- | ------------------------------------------------- |
| Keep the `---` lines at the top and bottom of frontmatter | Delete or move them                               |
| Follow exact indentation (2 spaces for lists)             | Mix tabs and spaces                               |
| Use plain text or simple Markdown                         | Paste formatted text from Word without cleaning   |
| Add images to the correct `/images/...` folder            | Upload images in random folders                   |
| Use lowercase filenames with hyphens                      | Use spaces, underscores, or capitals in filenames |
| Ask the dev team if unsure                                | Guess formatting — it may break the layout        |

---

## 💾 How to Save and Sync Changes with GitHub Desktop

This guide shows you how to use the GitHub Desktop app to save and upload your changes.

### Part 1: Before You Start (Get Latest Updates)

Always sync your local files *before* making new edits. This prevents conflicts.

1.  **Open GitHub Desktop** and make sure your current repository is `Shridhan-content`.
2.  **Switch to the `dev` branch**. At the top, click `Current Branch` and select `dev`.
3.  **Fetch and Pull**. Click the **`Fetch origin`** button. If it changes to say **`Pull origin`**, click it again to download the latest changes to your computer.

### Part 2: Edit Content in VS Code

1.  In GitHub Desktop, click **`Open in Visual Studio Code`** to open the project.
2.  Navigate to the correct folder (`products/`, `services/`, etc.) and edit the `.md` files as needed.
3.  **Save your changes** in VS Code (`Ctrl+S` or `Cmd+S`).

### Part 3: Save and Upload Your Changes

After saving your files, return to GitHub Desktop to upload them.

1.  **Review Your Changes**: On the left, you will see a list of all the files you modified.
2.  **Write a Commit Message**: In the bottom-left corner:
    *   In the **Summary (required)** field, write a brief, clear description of what you changed.
    *   *Example*: `Update summary for Magnetic Level Indicators`
3.  **Commit Your Changes**: Click the blue **`Commit to dev`** button. This saves a snapshot of your work on your computer.
4.  **Push to GitHub**: Finally, click the **`Push origin`** button at the top of the window. This uploads your committed changes to the `dev` branch on GitHub for the development team to see.

> ✅ **That's it!** Once you've pushed your changes, the development team will be able to see them and merge them into the live site.

---

## 🏷️ File Naming Rules

When creating new files, follow these rules:

* Use **lowercase** letters only
* Use **hyphens (-)** instead of spaces

Examples:

```
✅ bilge-alarm-systems.md
❌ Bilge Alarm Systems.md
❌ bilge_alarm_systems.md
```

> 💡 Consistent filenames help generate clean URLs and keep the site organized.

---

## 🧬 Optional: Learn Markdown (Beginner-Friendly)

If you'd like to learn more, these guides are helpful:

* Markdown Basics: [https://www.markdownguide.org/basic-syntax/](https://www.markdownguide.org/basic-syntax/)
* YAML Frontmatter: [https://jekyllrb.com/docs/front-matter/](https://jekyllrb.com/docs/front-matter/)
* Edit files on GitHub: [https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files](https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files)

---

## 🦘 Need Help?

If something is confusing:

* 📧 Email: `support@softeem.ca`
* 💬 Open a GitHub Issue and title it: `Help with Content Editing`

We’re here to help. Everything is versioned — you can’t permanently break the site. 💪
