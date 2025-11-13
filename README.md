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

## 💾 How to Edit and Save Your Work (The Safe Way)

This guide uses the GitHub Desktop app. The process is designed to be safe, so you can't accidentally break the website. Think of it like suggesting changes to a document, rather than editing the master copy directly.

### Step 1: Start a New Editing Session

Do this **every time** you start a new task (e.g., updating a product page, adding an event).

1.  **Open GitHub Desktop** and make sure your current repository is `Shridhan-content`.
2.  **Get the latest master draft**:
    *   Click `Current Branch` at the top and select the **`main`** branch.
    *   Click the **`Fetch origin`** button to check for new updates. If it changes to say **`Pull origin`**, click it again.
3.  **Create your personal copy for editing**:
    *   Click `Current Branch` again and click the **`New Branch`** button.
    *   Name your copy based on your task (e.g., `update-expo-page`, `fix-typo`). Use lowercase and hyphens.
    *   Click **`Create Branch`**, then click the **`Publish branch`** button.

> ✅ **You are now in a safe editing space!** Any changes you make here won't affect the main website until they are approved.

### Step 2: Make Your Edits
1.  In GitHub Desktop, click **`Open in Visual Studio Code`** to open the project.
2.  Find the file you want to edit in the folders on the left.
3.  Make your changes to the text and save the file in VS Code (`Ctrl+S`).

### Step 3: Save and Submit Your Work for Approval

Once you're happy with your edits, follow these steps to submit them.

1.  **Return to GitHub Desktop**. You'll see your changed files listed on the left.
2.  **Describe your change**: In the **Summary** box at the bottom-left, write a short note about what you did.
    *   *Example*: `Updated the text on the Automation Expo page`
3.  **Save your changes**: Click the blue **`Commit to...`** button. This saves a snapshot of your work to your personal copy.
4.  **Send for review**: Click the **`Push origin`** button at the top. This uploads your saved changes.
5.  **Ask for approval**: A new section will appear. Click the **`Create Pull Request`** button. This will open a page in your web browser. Just click the final **`Create Pull Request`** button on that page.

> ✅ **All done!** You have successfully submitted your changes. The tech team will now review them and merge them into the website.

### Step 4: Clean Up Before Your Next Task

After the tech team confirms your changes are merged, you can delete your old personal copy.

1.  In GitHub Desktop, switch back to the **`main`** branch and make sure it's updated (`Fetch`/`Pull`).
2.  Go to the menu bar at the top and click `Branch > Delete...`.
3.  Select your old branch (e.g., `update-expo-page`) and click **`Delete`**.

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
