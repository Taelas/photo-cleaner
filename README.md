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
