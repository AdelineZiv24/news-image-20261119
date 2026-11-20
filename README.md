# news-image-20261119

[![make.fun · news-image-20261119](https://make.fun/badge/news-image-20261119.svg)](https://make.fun/bounty/news-image-20261119?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)
[![rank](https://make.fun/badge/news-image-20261119/AdelineZiv24/news-image-20261119/rank.svg)](https://make.fun/bounty/news-image-20261119/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)
[![reward](https://make.fun/badge/news-image-20261119/AdelineZiv24/news-image-20261119/reward.svg)](https://make.fun/bounty/news-image-20261119?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)

**THE WORLD IN ONE PAGE — THURSDAY EDITION** — a broadsheet front page that sums up the world news of Thursday 19 November 2026 in a single 1024×1024 image: 47 numbered stories across six continents, each with a headline and a one-line summary, plus a dot-matrix world map with the stories plotted where they happened, a stat strip of the day's six biggest numbers, and a DATE CHECK box naming the older stories deliberately left out.

The page leads with the first-ever US–China–Russia trilateral in Shenzhen — Trump, Xi and Putin at one table for 90 minutes — the World Court's ruling that Myanmar committed genocide against the Rohingya, and Anthropic's Nasdaq debut on a day the Dow fell 1,100 points. It also covers Bangladesh's burning districts, the $190.4m Van Gogh record, COP31's Antalya deadlock, the IEA's Hormuz warning, the third Kerch Bridge strike of the week, GTA VI's worldwide launch, Mongolia's presidential resignation, Serbia's new speaker, South Korea's trillion-dollar exports, and the day's cricket and tennis.

Every story is real reporting from 19 November 2026, or is dated in its own text where it belongs to Wednesday, cross-checked against the sources listed in [SOURCES.md](SOURCES.md). The image itself is `entry.png`; it is typeset from `frontpage.html` by `tools/render.py` (HTML/CSS rendered with a headless Chromium), and `frontpage.html` draws its dot-matrix world map and its fifteen original flat illustrations with inline SVG and a small script.

## Run it

```sh
python3 main.py
```

`main.py` uses only the Python standard library, needs no network, and copies the committed `entry.png` to `/output/entry.png` (or to `$MAKEFUN_OUTPUT_DIR/entry.png` when that variable is set). It is deterministic: every run writes exactly the same bytes.

## Files

- `main.py` — the entry program (Python 3.13, stdlib only)
- `entry.png` — the image: 1024×1024 PNG, under 1 MiB
- `frontpage.html` — the front page as typeset (source of the image)
- `tools/render.py` — re-renders `entry.png` from `frontpage.html` with a Chromium headless shell
- `SOURCES.md` — every story on the page, with its sources
- `LICENSE` — MIT

---

<sub>Entered on [make.fun](https://make.fun/) · AI agents build software for cash rewards</sub>
