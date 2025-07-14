# 🗂️ QuickNote

QuickNote is a simple, responsive note-taking web app that lets you quickly jot down notes, categorize them with emojis, and sort/search your content. Your notes are stored in the browser's `localStorage`, so they persist between sessions.

> ✍️ Built as a personal solution for quickly taking notes while watching online videos—no need to switch tabs or open another app

## Demo

<https://quicknote1.netlify.app/>

## Features

- 🆕 Add notes with `title`, `body`, `date` and `category` (emoji)
- 📝 Edit existing notes in-place
- 🗑 Delete notes individually
- 💾 Save and persist notes using `localStorage`
- 🔎 Search notes by keyword (title, body)
- 🔃 Sort notes by:
  - 📅 Date
  - 🔤 Title
  - 📂 Category
- 🧼 Clear all notes (via double-click for safety)

## 🖥️ Technologies Used

| Technology     | Purpose                         |
| -------------- | ------------------------------- |
| HTML5 + CSS3   | Structure and styling           |
| JavaScript     | Functionality and interactivity |
| `localStorage` | Persistent data storage         |

## 🚀 How to Use

1. Open the app in your browser.

2. Type in a note title, body, and select a category.

3. Click Add to save the note.

4. Use the Search bar to filter notes.

5. Use the Sort dropdown to organize them.

6. Click 📝 to edit and 💾 to save a note.

7. Click 🗑 to delete a note.

8. Double-click Clear All Notes to remove everything.

## 🧠 JavaScript Concepts Practiced

| Concept              | Usage                               |
| -------------------- | ----------------------------------- |
| `forEach()`          | Render each note                    |
| `filter()`           | Search notes                        |
| `sort()`             | Sort by date/title/category         |
| `Set`                | Avoid duplicate dates during render |
| `localStorage`       | Save and retrieve note data         |
| `RegExp`             | Perform keyword-based search        |
| `readonly` attribute | Enable/disable editing              |
| DOM manipulation     | Build notes dynamically             |

## ⚙️Internal Notes

- noteSections.innerHTML = ""
  → Clears previous content before re-rendering. Prevents note duplication in UI.

- uniqueDate = new Set()
  → Tracks which dates have already been rendered so each date appears only once (for grouped views).

## 💡 Why I Made This App

While watching JavaScript tutorials online, I found it slow to switch to another tab (like a note-taking app) to jot down notes and then return to the video. So, I created QuickNote as a lightweight, fast note-taking tool. Later, I extended it into a Chrome Extension and a deployable web app with sorting and filtering capabilities.

## ✅ Future Ideas

- 🌓 Dark mode

- 🖇️ Tagging or multi-category support

- 🔐 Optional password or pin lock
