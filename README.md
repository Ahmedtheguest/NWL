# NWL / نَوْل — Everything Is Connected

**A bilingual, responsive brand concept website for NWL, built around Strategy × Enablement × Architecture.**

This repository is ready to deploy as a **static website on Vercel**. No frameworks, build tools, npm dependencies, API keys, or server are required.

> **Brand status:** NWL / نَوْل is a *working brand concept*, not a finalized company name or trademark.

## Features

- English / Arabic language switching with RTL support
- Responsive desktop and mobile layouts
- Animated brand visual, scroll reveals, and interactive diagrams
- Interactive methodology sections and a challenge-brief generator
- Local-only interaction: the brief is generated in the visitor's browser and copied to their clipboard
- Brand identity, mission, vision, target businesses, and future roadmap
- Search and social sharing metadata

## File structure

```text
/
├── index.html                 # Entire website (HTML, CSS, JavaScript)
├── vercel.json                # Vercel static-site settings
├── assets/
│   └── social-preview.png     # Preview for shared links
├── README.md                  # Project instructions
└── .gitignore
```

## Deploy from GitHub to Vercel

1. **Create a GitHub repository.** Visit GitHub → New repository. Give it a name such as `nwl-website`.
2. **Upload the project files.** Extract the ZIP. Upload **the contents of the folder** (including `index.html` and `vercel.json`) to the **root** of the GitHub repository. Don't upload only the ZIP.
3. **Import on Vercel.** Sign in at https://vercel.com/new, select **Import Git Repository**, authorize GitHub if needed, and choose your new repository.
4. **Confirm project settings.** Select **Framework Preset: Other**, set **Root Directory: `./`**, and leave **Build Command** disabled/empty. No environment variables are needed.
5. **Click Deploy.** Your project will receive a live `*.vercel.app` link. Future pushes to the GitHub repository trigger new deployments automatically.

### Deploy without GitHub (alternative)

Visit https://vercel.com/new or https://vercel.com/drop and upload the extracted project folder / ZIP directly. To keep automatic updates, connect GitHub afterward.

## Edit the website

- Content and all translations live in `index.html`.
- Theme colors are defined as CSS variables near the top of `<style>` (`--ink`, `--signal`, `--paper`, `--clay`, etc.).
- Language switching is handled by the `translations` object and `applyLanguage()` JavaScript function.
- The interactive challenge brief is intentionally **not a working contact form**; it doesn't transmit or store submitted content. To collect inquiries, you'll need a real email/contact service or backend and an appropriate privacy notice.
- If you choose a different official brand name, update both the visual text and page metadata before public launch.

## Local preview

Open `index.html` directly in a browser, or run a local server:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## ملاحظات النشر

الملفات جاهزة للرفع إلى GitHub ثم ربط المستودع بمنصة Vercel. لا تحتاج إلى إعداد Node.js أو عملية بناء (Build). الاسم «نَوْل» وهوية الموقع الحالية مبدئيان وقابلان للتعديل.
