# CF247 guides hub prototype

Design prototype for the "Car finance for your situation" hub on Car Finance 247 guides.

```
npm start
```

Opens on http://localhost:3000 (set `PORT` to change). No dependencies, Node 18+.

- `/` version switcher; `?view=v1` or `?view=v2` picks the starting version
- `/v1/` version 1 (frozen)
- `/v2/` version 2 (work in progress)
- Anything else (e.g. `/guide/...`) redirects to https://www.carfinance247.co.uk so links still work.
- `archive/` earlier rates-placement experiments (A/B/C), not served.

Edit files under `docs/`; changes show on refresh.

Mock-up for review only. Compliance text (representative example, broker statement) must be checked before anything goes live.

## GitHub Pages

Settings > Pages > Deploy from a branch > `main` / `/docs`. The switcher and both versions are static, so they work there (`?view=v1` / `?view=v2`). The redirect of `/guide/...` links to the live site only works on the local server; on Pages those links 404.
