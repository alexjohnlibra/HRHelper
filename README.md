<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/drive/1rcKDHocMJydMCBea0k6wPv5UHuv3yOkt

## Run Locally

**Prerequisites:**  Node.js

1. Install dependencies:
   ```bash
   npm install
   ```
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key (if applicable)
3. Run the app:
   ```bash
   npm run dev
   ```

## Build for Production

To create a production build:
```bash
npm run build
```
 
## Setup & Deployment Operations

This project has been fully configured for a seamless development and deployment experience:

### 1. Project Initialization & Dependencies
- Configured `package.json` with React, Vite, and necessary UI libraries.
- Run `npm install` to download dependencies.
- Run `npm run dev` to spin up the local dev server.

### 2. GitHub Actions Deployment
- A GitHub Action (`.github/workflows/deploy.yml`) is set up to automatically build and deploy your app to **GitHub Pages** whenever you push to the `main` branch.
- **To enable:**
  1. Go to your repository **Settings** -> **Pages**.
  2. Under "Build and deployment", set **Source** to **GitHub Actions**.

### 3. Version Control (`.gitignore`)
- A comprehensive `.gitignore` ensures that build outputs (`dist/`), dependencies (`node_modules/`), system files (`.DS_Store`), and sensitive privacy variables (`.env`, `.env.local`) are securely ignored and kept out of your public repository.

指令集修改
 1. 設定 package.json 並安裝套件
 2. 確認專案可以正常運行
 3. 設計 GitHub Action 部署腳本
 4. 設計 .gitignore，確保不需上傳檔案已被忽略
 5. 將操作記錄到 README.md
 6. 需要询问AI如何部署的步骤（deployment）的详细步骤即可