# Lab Organizer

Personal project organizer for organic chemistry lab work and project progress.

- **Projects** with tasks, ideas, literature, collaborations, FindMolecule links, progress log and characterization (compounds, structures, spectra)
- **Today / Daily work**: plans tasks from all projects to fit one workday (default 8 h)
- **Progress bars** and a health check for each project
- **Structure search**: substructure search by SMILES, or search by formula
- **Settings**: default time per activity type, plus custom activity types

## How it runs

`organizer.html` is a single-page app made to run as a Claude Artifact. Data is stored in the
artifact's private, owner-only database, and spectra are stored as artifact assets.
No data is kept in this repository.

## Local preview

Open `organizer.html` from `localhost` or `file://`. The page then runs in preview mode with
sample data and saves nothing.

```bash
python3 -m http.server 8765
```

Then open http://localhost:8765/organizer.html
