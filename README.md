# Simple Web Project - GitHub Actions CI/CD

## 📋 Project Overview
This is a simple static web project designed to demonstrate a CI/CD pipeline using **GitHub Actions**. The project automates testing, building, and (optionally) deploying the site to **GitHub Pages** upon every push to the `main` branch.

---

##  CI/CD Workflow Breakdown

### **Trigger:**
- The workflows are triggered **on every push to the `main` branch**.

### **test.yml** (Testing & Build Pipeline)
Steps:
1. **Checkout Code** – Pulls the latest code from GitHub.
2. **Setup Node.js Environment** – Uses Node.js v16.x.
3. **Install Dependencies** – Runs `npm install` to fetch dependencies.
4. **Run Tests** – Executes `npm test` (currently mocked as placeholder).
5. **Build Project** – Runs `npm run build` to generate production build.

### **deploy.yml** (Optional Deployment to GitHub Pages)
Steps:
1. **Checkout Code**
2. **Build Project**
3. **Deploy to GitHub Pages** using `peaceiris/actions-gh-pages`.

>  Note: The deployment step is configured but **static site content needs to be provided in the `/src` folder** for the GitHub Pages URL to be live.

---

## 🖥️ Local Development Setup

### Prerequisites:
- Node.js >= v18.x
- NPM (Node Package Manager)

### Steps:
```bash
# Clone the repository
git clone https://github.com/ChallaDevOps/assignment-GHA-cicd
cd assignment-GHA-cicd

# Install dependencies
npm install

# Run Tests
npm test

# Build Project
npm run build






CICD:
=====

Push code to main branch.

GitHub Actions will automatically deploy the site if it is generated correctly.

Currently, the GitHub Pages deployment workflow is configured but the live URL is not active because placeholder content is used.

Expected URL
https://ChallaDevOps.github.io/assignment-GHA-cicd/

