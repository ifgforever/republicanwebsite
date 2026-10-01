# Republican Unified Voters

A volunteer voter guide for the Illinois general election on Tuesday, November 3, 2026.

The site lists every statewide, congressional and Cook County race, the Republican running in each, and a non-Democrat choice where no Republican is on the ballot. Visitors mark their picks and copy the list to send to friends.

## How it works

The whole site is one file, `index.html`. There is no build step. Open it in a browser to preview it.

Visitors' picks, district and plan are saved in their own browser only (localStorage). Nothing is sent to a server.

## Updating candidates and dates

The data is in the `<script>` near the bottom of `index.html`:

- `STATEWIDE`: Governor, U.S. Senate, Attorney General, Secretary of State, Comptroller, Treasurer
- `HOUSE`: all 17 U.S. House districts
- `COOK_REP`: Cook County races with Republicans (Water Reclamation District)
- `COOK_ALT`: Cook County races with no Republican, where a non-Democrat can be marked instead
- `DATES`: the City of Chicago key dates

The "Only a Democrat is running" list and the page text are plain HTML above the script.

## Putting it online

Any static host works. Two easy options:

- **GitHub Pages:** Settings → Pages → Source: "Deploy from a branch" → Branch: `main`, folder `/ (root)`.
- **Cloudflare Pages:** connect this repository, leave the build command empty, and set the output directory to `/`.

## Sources

Candidates were checked on October 1, 2026 against:

- [Illinois State Board of Elections](https://www.elections.il.gov) candidate list for the November 3, 2026 general election
- [Chicago Board of Elections](https://chicagoelections.gov)
- [Cook County Clerk](https://www.cookcountyclerkil.gov), including the November write-in candidate list
- [Evanston RoundTable ballot guide](https://evanstonroundtable.com/2026/09/30/2026-midterm-ballot-guide-english/) (September 30, 2026)
- [Ballotpedia](https://ballotpedia.org) and Wikipedia's 2026 Illinois election pages

Each voter's official sample ballot is the final word.

## Disclaimer

Republican Unified Voters is a volunteer voter guide. It is not affiliated with the Illinois Republican Party, the Republican National Committee, or any candidate or campaign. If money is spent promoting this site, Illinois "paid for by" disclaimer rules may apply.
