# Maradona 1986 — World Cup analysis

Jupyter notebook behind the blog post
[One Man's Tournament: Maradona's 1986 coronation](https://shawnhdx0710.github.io/blogs/maradona-1986/maradona-1986/).

It rebuilds the visuals for Argentina's 1986 World Cup run using StatsBomb event data:

- QF vs England — match `3750191`
- SF vs Belgium — match `3889148`
- Final vs West Germany — match `3889149`

The notebook downloads the three matches from the public StatsBomb open-data repository at
runtime, then renders the formation, pass/shot maps, heatmap, and on-ball charts. The
`afa-badge.png` asset is used for the AFA badge on the formation graphic.

## Run

```bash
python3 -m venv .venv
.venv/bin/pip install -r requirements.txt
.venv/bin/jupyter notebook maradona-1986.ipynb
```

Run from the repository root so `afa-badge.png` resolves. Generated SVGs are ignored; the
versions used on the site live in the website's blog post directory.

StatsBomb Open Data is free for research/non-commercial use with attribution. Raw match
JSON is not committed.
