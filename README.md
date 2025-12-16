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
| **Always create a new branch**                            | **Edit directly on the `main` branch**            |
| Ask the dev team if unsure                                | Guess formatting — it may break the layout        |

---

## 💾 How to Edit and Save Your Work (The Safe Way)

Follow these instructions exactly to safely update the website content.

> ⛔️ **CRITICAL RULE:** Never edit the `main` branch directly. **Always** create a new branch first.

### Phase 1: Create a New Branch (Start Here)

Do this **every time** you want to make changes.

1.  **Open the GitHub Desktop app** on your computer.
2.  **Select the Repository**: Make sure `Shridhan-content` is selected in the top-left corner.
3.  **Switch to Main**:
    *   Click the **Current Branch** button at the top.
    *   Select **`main`** from the list.
4.  **Get Latest Updates**:
    *   Click the **Fetch origin** button at the top right.
    *   If the button changes to **Pull origin**, click it again to download the latest files.
5.  **Create Your Branch**:
    *   Click the **Current Branch** button again.
    *   Click the **New Branch** button.
    *   **Name your branch**: Type a name like `updating-product-content` (lowercase, no spaces).
    *   Click **Create Branch**.
    *   Click **Publish Branch** to save it to the cloud.

> ✅ **Success!** You are now in your own safe lane.

### Phase 2: Make Your Changes

1.  **Open the Editor**:
    *   In GitHub Desktop, click the button that says **Open in Visual Studio Code**.
2.  **Find the File**:
    *   In VS Code, look at the file explorer on the left.
    *   Click the folder (e.g., `products/`) to expand it.
    *   Click the file you want to edit (e.g., `magnetic-level-indicators.md`).
3.  **Edit the File**:
    *   Make your text changes in the editor window.
4.  **Save the File**:
    *   Go to **File > Save** in the menu, or press `Ctrl + S`.

### Phase 3: Save and Upload (Commit & Push)

1.  **Return to GitHub Desktop**:
    *   Switch back to the GitHub Desktop app. You will see your changed file listed on the left.
2.  **Commit (Save) Your Changes**:
    *   Find the **Summary** box at the bottom left (it usually says "Summary (required)").
    *   Type a short description, e.g., "Updated description for MLI product".
    *   Click the blue **Commit to [your-branch-name]** button.
3.  **Push (Upload) Your Changes**:
    *   Click the **Push origin** button at the top right.
    *   *Note: This sends your changes to the internet so developers can see them.*
4.  **Finish**:
    *   Tell the developer team you have pushed your branch (e.g., "I pushed the `updating-product-content` branch").

### Phase 4: Cleaning Up

Once the developers have merged your changes:

1.  Switch back to the **`main`** branch in GitHub Desktop.
2.  Click **Branch > Delete...** in the top menu to remove your old branch.

To start a new task, go back to **Phase 1**.

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
