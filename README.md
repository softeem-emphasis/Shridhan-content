# Shridhan Website - Content Editing

This repository contains all the content for the Shridhan website.

## Folder Structure

### Content Folders
*   `products/` - Product information and descriptions
*   `events/` - Event details and information
*   `services/` - Service descriptions
*   `images/` - All images organized by type
    *   `images/events/` - Event images
    *   `images/products/` - Product images
    *   `images/services/` - Service images

---

## ✍️ How to Edit Content

Every content file (e.g., `bilge-alarm-systems.md`) has two parts:

1.  **Frontmatter**: The data at the very top between the `---` lines. This holds key information like the title, summary, and image list.
2.  **Body**: The main description text that appears *below* the second `---`.

### Example File: `magnetic-level-indicators.md`
```markdown
---
title: Magnetic Level Indicators (MLIs)
collection: Level Instrumentation
images:
  - magnetic-level-indicators-mlis.webp
summary: Provides clear and reliable visual indication of liquid levels...
sku: LI-MLI-100
---

This is the main body content. You can write multiple paragraphs here.

This is a second paragraph.
```

### Editing a Page
1.  Navigate to the correct folder (e.g., `products/`).
2.  Find and open the `.md` file you want to edit.
3.  **To edit the summary**, change the text after `summary:`.
4.  **To edit the main description**, change the text in the body section below the `---`.
5.  Save the file.

### ⭐ Golden Rules for Editing
*   ✅ **DO** keep the `---` lines at the top and bottom of the frontmatter.
*   ✅ **DO** pay attention to the spacing (indentation) for lists like `images`.
*   ❌ **DO NOT** change the `sku:` value of an existing product. This is a unique ID.
*   ❌ **DO NOT** use complex HTML. Stick to plain text.

---

## 🚀 When You Make Changes

**IMPORTANT**: After making any changes:

1. Commit your changes with a clear message
2. **Notify the developers** by:
   - Creating a GitHub issue titled "Content Update - [what you changed]"
   - OR sending an email with details about what was updated

## 🏷️ File Naming
- Use lowercase letters
- Use hyphens instead of spaces
- Example: `bilge-alarm-systems.md`

## ❓ Need Help?
Contact the development team if you have questions!
