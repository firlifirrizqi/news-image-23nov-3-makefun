# The Daily World — 23 November 2026 (third entry)

[![make.fun bounty: news-image-20261123](https://img.shields.io/badge/make.fun-news--image--20261123-blue)](https://make.fun/bounty/news-image-20261123)
[![repo: firlifirrizqi/news-image-23nov-3-makefun](https://img.shields.io/badge/repo-firlifirrizqi%2Fnews--image--23nov--3--makefun-green)](https://github.com/firlifirrizqi/news-image-23nov-3-makefun)
[![referral: v8vnayfm](https://img.shields.io/badge/referral-v8vnayfm-orange)](https://make.fun?ref=v8vnayfm)

One newspaper front page that sums up **Monday 23 November 2026** in six
stories, drawn entirely in code as a single 1024×1024 PNG. Third entry for
make.fun's "Sum up 23 November's world news in one image" bounty
($100 in USDC, 50 paid places).

## The six stories

1. **Markets** — Asian shares plunge as AI fears spread: Nikkei falls
   5.06% and chipmakers slide; regulators rush to calm the markets.
2. **Health** — Ebola toll far higher than reported: hidden graves show
   Bunia's dead far exceed official counts in DR Congo.
3. **Middle East** — Iran claims 78 US drones downed: the IRGC tally
   counts 58 Reapers and 20 Predators; the US has not confirmed it.
4. **Sport** — LaLiga hit by a data breach: personal data stolen from a
   fan platform in a mid-November cyberattack.
5. **Labour** — Bangladesh wage talks stall: makers offer 15% as workers
   demand double; factories shut on Monday.
6. **Industry** — Vietnam starts a rare-earth plant: a $61m Haiphong
   plant to make 10,000 tonnes a year for magnets and EVs.

All six were first reported on 23 November 2026, and none of them appears
in the first or second entry for this bounty. Weekend follow-ups were left
out on purpose: the Sudan drone strikes, the Dymer rescue, the Istanbul
rally, the South Sudan raid, Bolsonaro's ICU stay and the penny law all
happened or were first reported on 20–22 November, not the 23rd.

## How it is made

`main.ts` (Node 22, standard library only) validates `entry.png` — PNG
signature, at most 1024×1024 pixels, at most 1 MiB — and copies it byte
for byte to the output directory. The image itself was drawn by the
accompanying Python script with PIL; running it twice produces identical
bytes.

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Licence

MIT — see [LICENSE](LICENSE).
