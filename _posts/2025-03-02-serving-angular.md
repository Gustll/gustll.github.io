---
title: Serving Angular on Github Pages
date: 2025-03-26
categories: []
tags: [angular] # TAG names should always be lowercase
description: >-
  This tutorial will guide you how to set up an Angular project & host it on GitHub Pages.
---

## ✏️ Prerequisites

- Git
- GitHub
- Angular project created via Angular CLI

## 🚀 Quick Start (local development)

1. Install the latest version of the Angular CLI globally and create a new Angular project.

    ```console
    npm install -g @angular/cli
    ng new your-angular-project --defaults
    cd your-angular-project
    ```

2. Next we should create a public repository on GitHub with our <repo_name>
By default Angular CLI initializes a Git repo, so now we add a remote for GitHub using the git remote add commang:

    ```console
    git remote add origin https://github.com/<username>/<repo_name>.git
    ```

3. To build our Angular project to github pages will will use angular-cli-ghpages in our project.

    ```console
    ng add angular-cli-ghpages
    ```

4. Now we can deploy out project to GitHub pages with all default settings.

    ```console
    ng deploy --base-href=/<repo_name>/
    ```

5. Our project should now be available at `https://<username>.github.io/<repo_name>`

6. [Example](https://gustll.github.io/animations-playground/)
