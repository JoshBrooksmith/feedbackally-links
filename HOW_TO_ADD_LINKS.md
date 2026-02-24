# How to Add New Survey Links

This guide explains how to add, edit, or remove survey links from your FeedbackAlly links page.

---

## 📁 File to Edit

Edit this file: `index.html`

---

## ➕ Adding a New Link

### Step 1: Open the file

Open `feedbackally-links/index.html` in any text editor (Notepad, VS Code, etc.)

### Step 2: Find the links section

Look for the `<nav class="links">` section. You'll see existing links that look like this:

```html
<a href="https://feedbackally.walmart.com/survey/XXXXX/" class="link-button" target="_blank" rel="noopener">
    <span class="link-icon">📦</span>
    <span class="link-content">
        <span class="link-title">English Title Here</span>
        <span class="link-desc">Spanish Title Here</span>
    </span>
    <span class="link-arrow">›</span>
</a>
```

### Step 3: Copy and paste a new link

Copy one of the existing `<a>...</a>` blocks and paste it right after the last one (but before `</nav>`).

### Step 4: Update the new link

Change these 4 things:

| What to Change | Example |
|----------------|----------|
| `href="..."` | Your FeedbackAlly survey URL |
| `link-icon` | An emoji (📦 🛠️ 📋 🚛 ⚠️ 💬 ⭐ 📝) |
| `link-title` | English title |
| `link-desc` | Spanish title |

### Step 5: Save the file

---

## 📤 Push Changes to GitHub

After editing, run these commands in your terminal:

```bash
cd C:\Users\jbroo28\Documents\puppy_workspace\feedbackally-links
git add -A
git commit -m "Add new survey link"
git push
```

Changes will be live in ~30 seconds!

---

## 📋 Complete Example

Here's a full example of adding a "Safety Feedback" survey:

```html
<a href="https://feedbackally.walmart.com/survey/ABC123XYZ/" class="link-button" target="_blank" rel="noopener">
    <span class="link-icon">⚠️</span>
    <span class="link-content">
        <span class="link-title">Safety Feedback</span>
        <span class="link-desc">Comentarios de Seguridad</span>
    </span>
    <span class="link-arrow">›</span>
</a>
```

---

## 🎨 Available Emojis for Icons

| Emoji | Good For |
|-------|----------|
| 📦 | Profiling, Packages |
| 🛠️ | Equipment, Tools |
| 🚛 | Delivery, Trucks |
| ⚠️ | Safety |
| 📋 | General Surveys |
| 💬 | Feedback, Comments |
| ⭐ | Quality, Ratings |
| 📝 | Forms, Documentation |
| 👷 | Personnel, Workers |
| ⏰ | Time, Scheduling |

---

## ❌ Removing a Link

1. Open `index.html`
2. Find the `<a>...</a>` block for the link you want to remove
3. Delete the entire block (from `<a href=` to `</a>`)
4. Save and push to GitHub

---

## ✏️ Editing an Existing Link

1. Open `index.html`
2. Find the link you want to edit
3. Change the URL, title, description, or emoji
4. Save and push to GitHub

---

## 🆘 Need Help?

Ask Code Puppy! Just say:
> "Add a new survey link to my feedbackally page for [Survey Name] at [URL]"

🐕 Woof!
