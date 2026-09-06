# spain-2026

A static scoreboard for a shared holiday kitty: what was spent, what each
person's share is, and the shortest set of payments that squares everyone up.

Live at <https://mikozyz.dev/spain-2026/>.

Everything here is generated. The ledger itself lives in a private repository,
one file per receipt, and a build step renders these two files from it:

| File | What it is |
| --- | --- |
| `index.html` | The page. Self-contained — the data is embedded in it. |
| `data.json` | The same numbers, if you would rather read them raw. |

People appear as initials only. Receipt photos, the original messages and the
names behind the initials stay in the private repository and are never
published; the build refuses to run if any of them would reach these files.

Don't edit `index.html` or `data.json` by hand — the next build overwrites them.
