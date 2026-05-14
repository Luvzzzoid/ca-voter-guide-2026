# California Voter Guide 2026

An interactive, nonpartisan voter guide for California's 2026 primary election. Enter your address, see only the elections on your ballot, get consolidated candidate profiles covering policy stances, endorsements, and funding sources, and save your favorites, all in one place.

**Live demo:** [luvzzzoid.github.io/ca-voter-guide-2026](https://luvzzzoid.github.io/ca-voter-guide-2026)

---

## Why this exists

The current voting experience can feel overwhelming, confusing, or too time-consuming. It's difficult for voters to navigate aspects such as figuring out what district they're in, what offices they need to research, what information is actually relevant for them, how to remember their picks, and more - causing many to skip the polls entirely. This guide attempts to fix that by combining everything into one visual, address-first experience.

---

## Features

- **Address lookup:** enter any California address to identify your congressional, state senate, and assembly districts via the U.S. Census Bureau Geocoding API. See only the elections on your specific ballot.
- **Visual district map:** highlights your district in blue across Congressional, State Senate, and Assembly views. Zoomable and pannable.
- **Candidate profiles:** summarized policy stances, endorsements, and a breakdown of top funding sources.
- **Office explainers:** plain-language one-liners for every office on your ballot (e.g. what does the State Assemblymember actually do?).
- **Election quick-nav:** jump to any election without scrolling through everything.
- **Browse all elections:** explore all 12 California statewide and district elections with the top navigation, independent of the address lookup.
- **Starred picks:** star candidates you like. Saved to your browser (localStorage). Persists across sessions on the same device.
- **Shareable ballot link:** generates a URL encoding your picks so you can send your ballot to friends and family. No server or account needed, everything is in the URL.
- **Printable cheat sheet:** print a summary of your candidate picks to bring to the polls.

---

## Data notice

**This is a prototype.** All candidate data currently shown is illustrative sample data for demonstration purposes only. In a production version, candidate data would be sourced from:

- [FPPC campaign finance filings](https://www.fppc.ca.gov/) (California)
- [FEC filings](https://www.fec.gov/) (federal races)
- Candidate official websites
- Nonpartisan journalism (e.g. CalMatters)

No editorial stance is taken on any candidate.

---

## Tech stack

- HTML, CSS, and JavaScript
- [D3.js](https://d3js.org/) for the district map
- U.S. Census Bureau [Geocoding API](https://geocoding.geo.census.gov/geocoder/) for address-to-district lookup, using JSONP to support browser-based requests without a backend
- GitHub Pages for hosting

---

## Contributing

This is an independent civic project with no commercial interest. If you have candidate data corrections, design suggestions, or want to contribute real district GeoJSON, open an issue or pull request.

---

## Content and attribution

Candidate information in the live version will be sourced from publicly available records and nonpartisan journalism, with full attribution. If you represent a news organization and are interested in a content partnership or data collaboration, please reach out via [Email](mailto:luvneetk@berkeley.edu) or [GitHub Issues](https://github.com/luvzzzoid/ca-voter-guide-2026/issues).

---

## License

MIT License. Free to use, adapt, and redistribute with attribution.

---

*Built by a California voter who thinks the system can be improved.*
