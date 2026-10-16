# Install the DEVPLAY GitHub profile

These files are made for the special profile repository:

`https://github.com/shahdelbary/shahdelbary`

## Upload the files

Keep the folders exactly as shown:

```text
shahdelbary/
├── README.md
├── assets/
│   ├── cyber-header.svg
│   └── neon-divider.svg
└── .github/
    └── workflows/
        └── snake.yml
```

1. Open the `shahdelbary` repository on GitHub.
2. Replace the existing `README.md` with the included one.
3. Upload the `assets` folder and its two SVG files.
4. Upload `.github/workflows/snake.yml`.
5. Commit all files to the `main` branch.

## Start the snake animation

1. Open the repository's **Actions** tab.
2. If GitHub asks, click **I understand my workflows, go ahead and enable them**.
3. Select **Generate contribution snake**.
4. Click **Run workflow** → **Run workflow**.
5. Wait for the green check. The workflow creates an `output` branch automatically.
6. Refresh the profile. GitHub's image cache may take a few minutes to update.

## If the workflow cannot push

Open **Settings → Actions → General → Workflow permissions**, select
**Read and write permissions**, then save and run the workflow again.

## Compatibility notes

- The header and divider are self-contained SVG files; no JavaScript is used.
- The typing line, badges, stats, streak, and view counter are remote images. If one provider is temporarily down, the rest of the profile still works.
- The snake appears only after the workflow has successfully created the `output` branch.
- DEVPLAY Edu and DEVPLAY Boost intentionally have no repository links because no verified public repository URL was supplied.
- If the default branch is not named `main`, update the branch name in `snake.yml` under `push.branches`.

