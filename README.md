# Leader age charts

Interactive charts on the age of national leaders, built to be embedded with an iframe.

Open `index.html` (or the published site's home page) to see every chart with a "Copy iframe code" button.

| File | Chart |
|---|---|
| `leader-age-gap-dotplot.html` | Which countries have the largest age gap between leader and the population? |
| `leader-age-swarm.html` | Leader age, by region (or political regime) |
| `leader-age-range.html` | How old are leaders in each region? (youngest, median, oldest) |
| `leaders-vs-population-scatter.html` | Do older populations have older leaders? |
| `leaders-gantt-world.html` | How old are the world's leaders, and how long have they led? |
| `leader-age-gap-map.html` | How far apart in age are leaders and the people they lead? |

Each page is a single self-contained HTML file. Leader ages are calculated in the browser from birth dates, so they update on their own; the list of leaders itself is a snapshot from 7 October 2026.

URL options (add to the end of a chart's address): `embed=1`, `title=1`, `controls=0`, `theme=light|dark`, plus `view=`, `group=`, `highlight=` and `compact=1` on the charts that support them.

## Data sources

- Leader birth dates and terms: Wikipedia and Wikidata.
- Median age of the population: UN World Population Prospects (2024), via Our World in Data.
- Political regimes: V-Dem, Regimes of the World (Democracy Report v16, 2026), via Our World in Data.
- Map borders: Natural Earth, via the `world-atlas` package.

Check each source for its own licence and attribution terms before reusing the data.
