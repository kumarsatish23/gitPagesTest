# Hosting an Angular App on GitHub Pages

## Introduction

GitHub Pages is a free service by GitHub that allows developers to host static websites directly from their repositories. It's ideal for hosting single-page applications (SPAs) created with frameworks like Angular, React, Vue.js, etc.

## Prerequisites

1. **Basic Angular Knowledge**: Familiarity with Angular CLI.
2. **GitHub Account**: To create repositories and host your app.
3. **Node.js and npm**: Ensure both are installed.

## Steps to Host

1. **Create Angular App**:
   ```bash
   npm install -g @angular/cli
   ng new <app-name>
   cd <app-name>
   ng serve --open
   ```
2. **Push Code to GitHub**:
   ```bash
   git remote add origin https://github.com/<username>/<repository>.git
   git push -u origin master
   ```
3. **Deploy to GitHub Pages**:
   ```bash
   ng add angular-cli-ghpages
   ng deploy --base-href=/<repository-name>/
   ```
   The app will be hosted at `https://<username>.github.io/<repository-name>`.

## Limitations

- **1GB Size Limit**: For static content.
- **100GB Monthly Bandwidth**: Be mindful of high traffic.
- **10-Minute Deployment Time**: Longer deployments may fail.
- **10 Builds Per Hour**: Avoid frequent deployments.

GitHub Pages is best for static content, documentation, or showcasing projects.

---

For more details, visit the [full guide](https://www.angularminds.com/blog/host-an-angular-app-in-github-pages).
```
This `README.md` format organizes the steps clearly, providing a concise and structured guide for hosting an Angular app on GitHub Pages.
