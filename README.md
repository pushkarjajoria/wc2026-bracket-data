# wc2026-bracket-data

Data store for the [World Cup 2026 Bracket Predictor](https://github.com/<owner>/wc2026-bracket).

This repo holds a single file:

- **`predictions.json`** — everyone's submitted brackets.

It is written from the browser by the bracket app using the GitHub Contents API and a
fine-grained Personal Access Token that is scoped to **this repo only** (Contents:
read/write). Keeping submissions here means a leaked token can't affect the app code or
any other repository.

You normally never edit this file by hand. If you ever need to remove a bad entry,
edit `predictions.json` on GitHub.com and commit — the app reads the latest version on
each load.

```json
{
  "version": 1,
  "submissions": []
}
```
