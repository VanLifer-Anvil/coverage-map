# Open-Network SIM Coverage Map

Interactive map of 4G and 5G mobile data coverage across Great Britain, built for Anvil / VanLifers.

It shows what a customer gets on their current network compared with an open-network SIM that uses whichever of EE, O2, Three or Vodafone is strongest.

**Live map:** https://vanlifer-anvil.github.io/coverage-map/

## Views

- **Compare** – your current network on the left, the open-network SIM on the right, with a slider to drag between them.
- **Open SIM** – the best coverage available from any of the four networks.
- **Networks per area** – how many of the four networks reach each spot.
- **One network** – a single network's coverage.

There is also a postcode search and a "Use my location" button.

## Where the coverage comes from

The coverage is each network's own published predicted coverage map, for 4G and 5G combined. Snapshot dates:

| Network  | Map date        |
|----------|-----------------|
| EE       | 12 March 2025   |
| Vodafone | 10 February 2025|
| Three    | 6 December 2024 |
| O2       | archive v208    |

The copies were taken from the archive kept by mastdatabase.co.uk. Signal levels were read from each network's own map key: "good indoors and outdoors" or "outdoors only / limited".

The area covered is Great Britain, including the Hebrides, Orkney and the Isles of Scilly. Shetland and Northern Ireland are not included.

Detail is roughly 50 m per pixel. Zooming in further enlarges the same data.

Coverage is a prediction, not measured signal. Real-world signal varies with terrain, buildings, trees and vehicle bodywork.

## Files

- `index.html` – the map page
- `tiles/` – pre-built coverage layers: `any`, `count`, `ee`, `o2`, `three`, `vodafone`
- `lib/` – the Leaflet map library

The background map is © OpenStreetMap contributors. Postcode search uses postcodes.io (open data).
