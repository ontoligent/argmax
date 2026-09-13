# Contributing to the Wiki

Thank you for helping maintain and expand our collective knowledge base! We use **Zensical**, a high-performance static site generator, to build and maintain our documentation repository.

Please follow this step-by-step workflow to propose wiki updates.

## 🛠️ Prerequisites & Installation

To preview your changes locally before submitting a Pull Request, you need Python installed on your machine.

1. **Install Zensical:** Open your terminal and run:
   ```bash
   pip install zensical
   ```

## 🔄 Step-by-Step Contribution Workflow

### 1. Edit a Page
* **Quick Web Edits:** If you are fixing a small typo, click the **"Edit this page"** button (pencil icon) on the top right of the live wiki site. GitHub will automatically guide you to create a fork and edit the Markdown directly in your browser.
* **Complex Edits / New Pages:** Clone this repository locally and open the project directory in your code editor (such as Visual Studio Code, Cursor, or Zed).

### 2. Run the Local Live Preview Server
Before pushing your changes, always test how they look in the browser. 
1. Open your terminal in the root repository directory.
2. Run the Zensical development server:
   ```bash
   zensical serve
   ```
3. Open your browser and navigate to `http://127.0.0.1:8000`. The page will automatically refresh every time you save edits to your Markdown files.

### 3. Check for Broken Links (Zensical Workspace Diagnostics)
Zensical automatically tracks internal anchors and files across the entire workspace. Before opening a Pull Request, look at your terminal output or open your editor's **Workspace Diagnostics/Problems** panel (if using a supported editor). 
* Zensical will alert you if you accidently link to a non-existent markdown file or use a broken cross-reference.
* Fix any warnings or errors before pushing!

### 4. Update the Navigation Map (If adding a new page)
If you create a completely new `.md` file inside the `docs/` folder, you must add it to the custom navigation layout. Open `mkdocs.yml` (or `zensical.toml`) and append your page path under the `nav:` block.

### 5. Submit Your Pull Request
Commit your changes to a new branch and push it to GitHub. Open a **Pull Request** matching your branch against our `main` branch. 

Once our automated GitHub Action workspace checks pass and a maintainer reviews the text, your PR will be merged, and the live wiki will automatically update within a couple of minutes!
