# stattstrack

Weekly leaderboard tracker for Maze of Gains: live table, the frozen end-of-week snapshot, the combined "snapshot + new week" ranking, activity windows and wallet balances.

- `index.html` is a static page. It reads `data.json`, `activity.json` and `wallets.json` from the `data` branch of this repository (raw.githubusercontent.com), which a local collector updates every couple of minutes.
- No build step. Deploy the `main` branch as a static site (Vercel: framework "Other", no build command). `vercel.json` disables deployments for the `data` branch.
