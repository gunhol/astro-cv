# CV / Portfolio Website

A minimalist, high-performance personal CV website built with **Astro** and **TailwindCSS**.
Designed to be hosted on **GitHub Pages** with zero configuration.

## 🚀 Quick Start (Run Locally)

Prerequisites: Node.js (v18+)

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Start development server:**
   ```bash
   npm run dev
   ```
   Open [http://localhost:4321](http://localhost:4321) to view it.

3. **Build for production:**
   ```bash
   npm run build
   ```

## 📝 How to Edit Content

You don't need to touch the HTML code to update your CV. All data is stored in a structured file.

1. Open **`src/data/cv.ts`**.
2. Update the fields in the `cvData` object:
   ```typescript
   export const cvData = {
     personal: {
       name: "Your Name",
       role: "Your Role",
       // ...
     },
     experience: [
       // Add or remove experience items here
     ],
     // ...
   }
   ```
3. Save the file. If the dev server is running, the changes will appear instantly.

## 🌍 Deployment (GitHub Pages)

This project is pre-configured with a GitHub Actions workflow for automatic deployment.

### 1. Push to GitHub
Create a new repository on GitHub and push this code:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

### 2. Configure Settings
1. Go to your repository on GitHub.
2. Navigate to **Settings** > **Pages**.
3. Under **Build and deployment**, select **Source: GitHub Actions**.

### 3. Custom Domain (Optional)
If you want to use a custom domain (like `hollander.one`):
1. Update `public/CNAME` with your domain.
2. Update `site` in `astro.config.mjs` with your full URL (e.g., `https://hollander.one`).
3. Configure your DNS provider to point to GitHub Pages.

## 🛠️ Tech Stack
- **[Astro](https://astro.build)**: Zero-JS frontend framework (super fast).
- **[TailwindCSS](https://tailwindcss.com)**: Utility-first styling.
- **TypeScript**: Type-safe data structure.
- **GitHub Actions**: Automated deployment.
