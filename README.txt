CENES Designer — Bilingual (English + Hindi) Ready Package (AI + 3D)
==================================================================

What's inside:
- electron-app/  -> Desktop UI (Electron) with language toggle (English/Hindi).
- backend/       -> Node.js server that proxies to Stable Diffusion WebUI for AI image generation.
- assets/        -> 5 sample designs for offline use.
- .github/workflows/ -> optional cloud build workflow.

Quick start (Windows 10):
1) Download & extract this ZIP to a folder (e.g., C:\CENES).
2) Install Node.js LTS from https://nodejs.org and restart your PC if prompted.
3) Start backend (in PowerShell):
   cd C:\CENES\backend
   npm install
   npm start
   You should see: CENES backend running on http://localhost:5000
   (Optional) To enable AI: run Stable Diffusion WebUI (Automatic1111) at http://127.0.0.1:7860
4) Start app (in another PowerShell):
   cd C:\CENES\electron-app
   npm install
   npm start
   The app UI has a language toggle button (top-right) to switch between English and Hindi.

Offline mode:
- You can use sample designs without internet. 3D preview works offline.
Online mode (AI):
- For AI generation, run Stable Diffusion WebUI locally and ensure backend is running. Then use the 'Generate with AI' button.

Build installer (optional):
- To create a Windows installer (.exe), run in electron-app:
   npm run dist
  The installer will appear in electron-app/dist.

If you want, I can now:
- A) Build the .exe for you in the cloud (GitHub Actions) if you create a GitHub repo and push this project.
- B) Or guide you step-by-step to build on your laptop.
