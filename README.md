# 📸 Photo Match & Clean

A lightweight, privacy-first, web-based duplicate photo finder. This tool allows you to select a local folder on your computer, scan it for identical or visually similar (edited/resized) photos, and safely review them before deletion—all without installing software or uploading a single pixel to the internet.

---

## ✨ Features

* **Visual Similarity Matching:** Uses Perceptual Hashing (aHash) to find photos that look the same, even if they have been renamed, resized, or slightly color-edited.
* **100% Private & Local:** Leverages the modern browser **File System Access API**. Your photos never leave your computer and are never uploaded to a server. 
* **Adjustable Sensitivity:** Use the sliding scale to look for exact digital duplicates or loose, "burst-mode" similarity matches.
* **Smart Organization:** Automatically groups duplicates together and marks the lower-resolution or modified copy for deletion while preserving your original.
* **Zero Installation:** Runs entirely inside modern web browsers as a single, lightweight web page.

---

## 🚀 How to Use

### Option 1: Run it Online (Recommended)
If you have hosted this repository on GitHub Pages, simply click your live link (e.g., `https://your-username.github.io/your-repo-name/`) to launch the app instantly.

### Option 2: Run it Locally
1. Download the `index.html` file from this repository to your computer.
2. Because web browsers require a secure environment to access local files, you cannot just double-click the file to open it. You must run a quick local server.
3. Open your terminal or command prompt in the folder where the file lives and run:
   ```bash
   python -m http.server 8000
## 📋 Step-by-Step Guide

1. **Adjust Strictness:** Set your preferred similarity threshold using the slider (the default setting is recommended for most users).
2. **Select Folder:** Click **"Select Photo Folder"** and grant the browser permission to view your chosen directory.
3. **Scan:** Wait a few moments while the background processor creates visual fingerprints for your images and groups them.
4. **Review & Clean:** Look through the generated duplicate groups. Click **"Delete Copy"** on any redundant files you want to remove from your device.

---

## 🌐 Browser Compatibility

This application relies on advanced local hardware integration via the **File System Access API**. 

* **Supported Browsers:** Google Chrome, Microsoft Edge, Opera, and Brave (Desktop versions).
* **Not Currently Supported:** Apple Safari and Mozilla Firefox do not yet fully support direct local directory management. Mobile browsers (iOS/Android) are also restricted by their mobile operating systems and cannot use this tool.

---

## 🔒 Privacy & Safety Note

* **Data Privacy:** This application runs entirely client-side (in your own browser window). There is no backend server, meaning zero tracking data or media data is ever collected, stored, or transmitted.
* **Safety Net:** To prevent accidental permanent data loss, please ensure you have a backup of important directories before executing massive bulk deletions.
