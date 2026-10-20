# Daily Growth Tracker

1. Edit `index.html`: set `OWNER` to your GitHub username and `REPO` to the repository name; leave `BRANCH` as `main` if that is your default branch.
2. Upload `index.html` and `data/progress.csv` to the **same GitHub repository**. The path must be exactly `data/progress.csv` (case-sensitive).
3. Enable GitHub Pages under Settings → Pages → Deploy from a branch → `main` / (root).
4. Create a fine-grained personal access token limited to this repository with Contents: Read and write. Enter it when saving an entry. Never commit a token to your repo or share it.
5. Each successful Save updates `data/progress.csv` via the GitHub Contents API. The page reads the CSV and displays recent entries. The repository must be public for the unauthenticated history view in this version.

Note: GitHub Pages itself is static and does not provide a backend. The GitHub repository is the CSV data store. GitHub contribution graph credit is not guaranteed: author email attribution and other GitHub rules apply. This demo asks for a token in a browser prompt on each save; for a long-term solution, use GitHub OAuth with a backend or a trusted authenticated service.
