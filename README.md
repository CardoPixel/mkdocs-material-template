# Welcome to MkDocs-material-template

This template repository is made to jumpstart the creation of a documentation site for any type of project.

It uses [Material Theme for MkDocs](https://squidfunk.github.io/mkdocs-material/), to render an awesome-looking site that can be easely edited using any markdown-compatible text editor, even with the native Markdown editor of Github itself!.

For full documentation about the components of this repo, visit [mkdocs.org](https://www.mkdocs.org/getting-started/), [mkdocs-material](https://squidfunk.github.io/mkdocs-material/getting-started/), [drawio](https://www.drawio.com/doc/), [mkdocs-drawio-file](https://github.com/onixpro/mkdocs-drawio-file), [mkdocs-git-revision-date-localized-plugin](https://timvink.github.io/mkdocs-git-revision-date-localized-plugin/index.html) and [mkdocs-git-authors-plugin](https://timvink.github.io/mkdocs-git-authors-plugin/).

## Commands

- Install he dependancies of this project.

FIRST:

```bash
npm install
```

OR

```bash
yarn install
```

OR

```bash
bun install
```

AND THEN:

```bash
pip install -r requirements.txt
```

- Start the live-reloading docs server.

```bash
mkdocs serve
```

OR

```bash
npm run serve
```

- Build the documentation site.

```bash
mkdocs build
```

OR

```bash
npm run build
```

- Make automatic Release, using the conventional commits to generate a CHANGELOG (ensure to this after the workflow CI finish to generate the .png files from the drawio files).

```bash
npm run release-it
```

## Project layout

```bash
    .github/                    # GitHub related files (README, Issue Templates, Actions, etc).
    .husky/commit-msg           # Configuration file to handle the commit msg for commitlint.
    .gitattributes              # Git Configuration file to handle various types of files.
    .gitignore                  # Git Configuration file for git to ignore files or folders.
    package.json                # Manage node.js dependencies, scripts, versioning, config and modules.
    requeriments.txt            # pip requeriments files to handle python dependencies.
    mkdocs.yml                  # The configuration file.
    docs/                       # Main folder for the documentation, each sub-directory will be a section
        index.md                # The documentation homepage.
        assets/                 # Assets for the documentation site (favicon, logo, drawio files, etc).
            stylesheets/        # Stylesheets to add custom color palettes.
                extra.css       # Sample on an stylesheet to override the theme.
            drawio-assets/      # Redered versions of the diagram in the drawio files (.png images by default).
        sample/                 # Sample section.
            sample-section.md   # Main markdown of a sample section.
        ...                     # Other markdown pages, images and other files.
```
