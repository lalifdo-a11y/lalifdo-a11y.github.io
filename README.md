This repository contains the complete codebase for a professional, minimalist, and responsive portfolio website designed specifically for free hosting on **GitHub Pages**.

---

## 📂 1. Directory Structure

To deploy or edit this portfolio locally, ensure the following file structure is maintained in your directory:

```text
[your-portfolio-folder]/
├── index.html   # Main page structure with semantic sections
├── styles.css   # Dark/Light theme system & responsive layouts
├── app.js       # Theme switcher and scroll highlighting logic
└── README.md    # Setup and deployment documentation (this file)
```

---

## 🚀 2. GitHub Pages Deployment Instructions

### Step 2.1: Create a GitHub Repository
1. Log in to your GitHub account (`lalifdo-a11y`).
2. Click **New** (or go to [github.com/new](https://github.com/new)).
3. Name your repository exactly:
   ```text
   lalifdo-a11y.github.io
   ```
   *Note: Using this exact format creates a "User Page" which will serve your website directly from the root URL: `https://lalifdo-a11y.github.io/`.*
4. Set the repository visibility to **Public** (required for hosting on GitHub Pages).
5. **Do not** initialize it with a README, `.gitignore`, or License (keep it empty). Click **Create repository**.

### Step 2.2: Push the Files to GitHub
Open your terminal/command prompt, navigate to the folder containing your portfolio files, and run the following commands:

```bash
# Initialize a local Git repository
git init -b main

# Stage and commit all files
git add .
git commit -m "Initial portfolio commit"

# Link your local repository to the GitHub remote
git remote add origin https://github.com/lalifdo-a11y/lalifdo-a11y.github.io.git

# Push the branch to GitHub
git push -u origin main
```

### Step 2.3: Verify GitHub Pages Activation
1. In your GitHub repository page, go to **Settings** (top navigation tab).
2. On the left sidebar, click **Pages** under the "Code and automation" section.
3. Under **Build and deployment**, ensure:
   - **Source** is set to `Deploy from a branch`.
   - **Branch** is set to `main` and the folder is set to `/ (root)`.
4. Click **Save**.
5. Wait 1–2 minutes. Your website will be live at:
   ```text
   https://lalifdo-a11y.github.io/
   ```

## 🎨 3. Customizing Your Portfolio

- **Profile Picture**: You can replace the SVG vector placeholder in the Hero section of `index.html` (under `<div class="hero-image-wrapper">`) with an `<img>` tag pointing to your custom profile picture:
  ```html
  <img src="assets/profile.jpg" alt="Yasuri Fernando" class="profile-img">
  ```
- **Social Media Links**: Look for the `social-links` block in `index.html` and replace the `#` links for LinkedIn, Instagram, Facebook, and YouTube with your actual profile URLs.
- **Projects & Research**: Add, delete, or rename project cards and interest summaries inside `index.html` to highlight your latest datasets and engineering milestones.
