# Contributing to the Wiki

Thank you for taking the time to contribute! This wiki is powered by [MkDocs](https://www.mkdocs.org/) and [GitHub Pages](https://pages.github.com/). We rely on Pull Requests (PRs) to update our documentation.

## How to Contribute (Quickest Method)

1. **Navigate to the page** you want to update on the live wiki.
2. Click the **pencil icon** ("Edit this page") in the top right corner.
3. If you do not have write access, GitHub will automatically create a fork of this repository for you.
4. Make your edits directly in the browser using Markdown formatting.
5. Scroll down, add a short title explaining your change, and click **Propose changes**.
6. Click **Create pull request**.

## How to Add a New Page

If you want to create a brand-new page from scratch rather than editing an existing one:

1. Fork this repository and clone it to your local machine.
2. Create a new `.md` file inside the `docs/` directory (e.g., `docs/getting-started.md`).
3. Write your content using standard Markdown syntax.
4. Open the `mkdocs.yml` file in the root directory.
5. Add your new page to the `nav` section to make sure it appears in the navigation sidebar:
   ```yaml
   nav:
     - Home: index.md
     - Getting Started: getting-started.md
   ```
6. Commit your changes, push to your fork, and submit a **Pull Request** to the `main` branch.

Once a maintainer reviews and merges your pull request, a GitHub Action will automatically build and publish your updates to the live site.
