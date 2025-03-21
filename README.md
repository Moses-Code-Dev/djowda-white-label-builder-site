Djowda White Label Builder Site Repository

🚀 Purpose

This repository (djowda-white-label-builder-site) hosts the production-ready static files (HTML, CSS, JS) for the Djowda White Label Builder's official website. It is the deployed site powered by GitHub Pages.

Note: All development and source code contributions must occur in the main frontend repository: djowda-white-label-builder-frontend

📁 Repository Structure

|-- index.html
|-- static/
|-- favicon.ico
|-- manifest.json
|-- robots.txt
|-- ...other production assets

📌 Rules & Contribution Guidelines

NO direct development in this repo.

No editing or adding of JS, CSS, React, or development files.

All functional and design changes happen in the main repo.

Production Builds Only:

Files in this repo are exclusively the output from npm run build in the frontend repo.

Pull Requests Requirements:

PRs must include ONLY built files (index.html, static assets, etc.).

PR description must reference:

Date of build

Link to the commit or PR in the main frontend repo

Branch Policy:

main branch only.

No dev or feature branches are maintained here.

Deployment:

GitHub Pages automatically deploys from the main branch.

Automation:

(Optional Future Plan) Automate build + push workflow via GitHub Actions triggered by changes in the main frontend repo.

🛠️ Example Update Workflow

# Clone the frontend repo
$ git clone https://github.com/YOUR-ORG/djowda-white-label-builder-frontend.git
$ cd djowda-white-label-builder-frontend

# Install dependencies and build
$ npm install
$ npm run build

# Copy the build files
$ cp -r build/* ../djowda-white-label-builder-site/

# Commit & Push to site repo
$ cd ../djowda-white-label-builder-site
$ git add .
$ git commit -m "Deploy build from frontend repo commit abc123 (YYYY-MM-DD)"
$ git push origin main


