# California Voter Guide 2026

An interactive, nonpartisan voter guide for California's June 2, 2026 primary election. Enter your address, see the elections likely on your ballot based on estimated district data, review consolidated candidate profiles covering policy stances, endorsements, and funding sources, save your favorites, and share your picks - all in one place, with no account or app required.

**Live:** 
- Cloudflare: [cavote.pages.dev](https://cavote.pages.dev/)
- GitHub Pages: [luvzzzoid.github.io/ca-voter-guide-2026](https://luvzzzoid.github.io/ca-voter-guide-2026)

---

## Why this exists

The current voting experience can feel overwhelming, confusing, or too time-consuming. Figuring out what district you're in, which offices you need to research, what candidates actually stand for, how to remember your picks, etc. It all ends up being a lot to navigate. This guide attempts to fix that by combining everything into one visual, address-first experience to lower that barrier.

---

## Features

- **Address lookup:** enter any California address to identify your congressional, state senate, assembly, and Board of Equalization districts via the U.S. Census Bureau Geocoding API. Only the races likely on your ballot are shown based on estimated districts. Verify your districts before relying on results. 
- **Visual district map:** highlights your district in blue across Congressional, State Senate, Assembly, and BOE views. Zoomable and pannable.
- **Candidate profiles:** summarized policy stances, endorsements, and a breakdown of top funding sources, sourced from public records and nonpartisan journalism.
- **Full candidate roster:** for statewide races, leading candidates have full profile cards with stances, endorsements, and funding. For U.S. House, State Senate, and Assembly races, full cards are limited, and candidates in those races are listed in the roster. All other candidates on any ballot appear in the roster below each race. 
- **Office explainers:** plain-language one-liners for every office on your ballot (e.g. what does the State Assemblymember actually do?).
- **Election quick-nav:** jump to any office without scrolling through everything.
- **Browse all elections:** explore all California statewide and district elections with the top navigation, independent of the address lookup.
- **Starred picks:** star candidates you like. Saved to your browser only (localStorage); never sent anywhere. Persists across sessions on the same device.
- **Shareable ballot link:** generates a URL encoding your picks so you can send your ballot to friends and family. No server or account needed, everything is in the URL.
- **Shareable ballot image** creates a downloadable image of your picks to post to social media or anywhere you like. Generated entirely in your browser. 
- **Printable cheat sheet:** print a clean summary of your starred candidate picks to bring to the polls.

---

## Data sources

Candidate and election data in this guide is drawn from publicly available sources:

- [California Secretary of State](https://www.sos.ca.gov/elections) - official candidate filings and district maps
- [CalMatters 2026 Voter Guide](https://calmatters.org/california-voter-guide-2026/) - nonpartisan candidate coverage
- [TransparencyUSA](https://www.transparencyusa.org/) - campaign finance data (may not reflect the most recent filings)
- [U.S. Census Bureau Geocoding API](https://geocoding.geo.census.gov/geocoder/) - address-to-district lookup
- Candidate official campaign websites (linked on each card)

No editorial stance is taken on any candidate.

---

## Disclaimers

**This guide is independent and not affiliated with the California Secretary of State, any government agency, any political party, or any campaign.**

- Data is drawn from public sources and may be incomplete, outdated, or subject to change. It does not represent the entirety of any candidate's record, positions, or qualifications.
- Campaign finance figures reflect data available at the time of publication and may not include recent filings.
- District assignments are estimated using the U.S. Census Bureau geocoder and may not perfectly reflect final adopted redistricting lines. Verify your district at [We Draw the Lines California](https://wedrawthelines.ca.gov/final-maps/).
- Your actual ballot may differ. Ballot contents are determined by your county elections office.
- This guide does not endorse any candidate, party, or ballot measure.
- You cannot cast a vote with this tool.

Verify all information independently before making voting decisions.

---

## Tech stack

- HTML, CSS, and JavaScript
- [D3.js](https://d3js.org/) for the district map
- U.S. Census Bureau [Geocoding API](https://geocoding.geo.census.gov/geocoder/) for address-to-district lookup, using JSONP to support browser-based requests without a backend
- GitHub Pages for hosting

---

## Contributing

This is an independent civic project with no commercial interest. If you have candidate data corrections, design suggestions, or want to contribute, open an issue or pull request on GitHub. You can also reach out via [Email](mailto:luvneetk@berkeley.edu).

---

## Embed this guide

Anyone can embed this guide on their website using a standard iframe.

```
<iframe 
  src="https://cavote.pages.dev/"
  width="100%" 
  height="800px" 
  frameborder="0"
  title="California Voter Guide 2026">
</iframe>
```

The guide is fully self-contained and runs client-side. No data is collected from your visitors. If you embed it, attribution is appreciated but not required under the MIT license.

---

## License

MIT License. Free to use, adapt, and redistribute with attribution.

---

*Built by a California voter who thinks the system can be improved.*
