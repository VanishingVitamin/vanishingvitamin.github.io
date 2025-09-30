# VanishingVitamin Website

This repository contains the source code for the VanishingVitamin website, which is published at `https://vanishingvitamin.github.io`.

The website is built using [Quarto](https://quarto.org) and automatically deployed to GitHub Pages using a GitHub Actions workflow.

---

## Website and Source Code
*   **Published Website:** `https://vanishingvitamin.github.io`
*   **Source Files:** The website content is written in Markdown (`.qmd`) and is located in the root of this repository.

## How to Contribute
Since the generated website files are handled by the GitHub Action, you only need to work with the source `.qmd` files.

### Prerequisites
1.  **Install Quarto:** To render and preview changes locally, you must [install Quarto](https://quarto.org/docs/get-started/).
2.  **Clone the Repository:**
    ```sh
    git clone https://github.com/vanishingvitamin/vanishingvitamin.github.io.git
    cd vanishingvitamin.github.io
    ```

### Workflow
1.  **Make your changes:** Create or edit `.qmd` files.
2.  **Preview locally:** Run `quarto preview` in your terminal to see your changes. If using RStudio, you can also run `quarto::quarto_render()` in the R Console.
3.  **Commit and Push:** Push your changes to the `main` branch.
    ```sh
    git add .
    git commit -m "Your descriptive commit message"
    git push origin main
    ```

## Project Structure
*   `_quarto.yml`: The main configuration file for the Quarto website. It defines the site's structure, navigation, and theme.
*   `index.qmd`: The source file for the home page. Other `.qmd` files contain text for other tabs.
*   `.github/workflows/deploy.yml`: The GitHub Actions workflow file that automates the build and deployment process.
*   `.gitignore`: Specifies files and folders to be ignored by Git, including the generated `_site/` folder.

### Automatic Deployment
A GitHub Actions workflow is automatically triggered after every push to `main`. 
The workflow renders the website and deploys the generated output to GitHub Pages, typically within a few minutes of pushing to `main`.
You can monitor the deployment's progress on the [**Actions**](https://github.com/VanishingVitamin/vanishingvitamin.github.io/actions) tab of this repository.

## Learn More
*   [**Quarto Website Documentation**](https://quarto.org/docs/websites/)
*   [**Quarto Publishing with Continuous Integration**](https://quarto.org/docs/publishing/ci.html)

---
*This `README.md` was last updated by Joe Zemmels, with help from Google Search AI.*
