# Lab Organizer

Personal project organizer for organic chemistry lab work and project progress.

- **Projects** with tasks, ideas, literature, collaborations, FindMolecule links, progress log and characterization (compounds, structures, spectra)
- **Today / Daily work**: plans tasks from all projects to fit one workday (default 8 h)
- **Progress bars** and a health check for each project
- **Structure search**: substructure search by SMILES, or search by formula
- **Settings**: default time per activity type, plus custom activity types

## How it runs

The site is served by GitHub Pages from `index.html`. This repository holds only the code: no data.

Your data (projects, tasks, spectra) is saved in a separate **private** repository
(e.g. `lab-organizer-data`), through the GitHub API, with a fine-grained access token that is kept
only in your browser. The first time you open the site on a device, it asks for the repository and the token.

`organizer.html` is the same app without the page skeleton; it also runs as a Claude Artifact.

## Local preview

Open `organizer.html` from `localhost` or `file://`. The page then runs in preview mode with
sample data and saves nothing.

```bash
python3 -m http.server 8765
```

Then open http://localhost:8765/organizer.html (add `?github` to the address to test with GitHub storage).
