# House-hunt map

A map of Kevin's Funda favorites, published with GitHub Pages. The page (`index.html`) reads `favorites.json` and shows each house as a pin on a PDOK or OpenStreetMap map. Each visitor's browser looks up the exact address through PDOK, and falls back to the postcode centre in `postcodes.json` if no address is found.

## Updating

Only `favorites.json` changes day to day. Set `updated` to today's date and list every current favorite:

| Field | Meaning |
|---|---|
| `u` | Funda listing URL |
| `a` | Street address, e.g. `Aegirstraat 1` |
| `pc` | 4-digit postcode, e.g. `1363` |
| `t` | Town |
| `price` | Asking price in euros (number) |
| `liv` | Living area in m² |
| `plot` | Plot area in m² |
| `beds` | Bedrooms |
| `lab` | Energy label, or empty if none is listed |
| `yard` | `yes` (back yard 100 m² or more), `likely` (garden all round on a big plot), `no` (under 100 m²), `unknown` (listing doesn't say), or `nc` (not checked yet) |
| `bg` | Back-yard size in m² if known, otherwise `null` |

Keep the yard details from the previous version for houses that are still favorites, and drop houses that are no longer favorites.

Browse Funda politely: one page at a time, at least 10 seconds apart, at most about 20–25 page loads an hour and 40 a day, and stop at the first sign of blocking (403, "Access Denied" or a CAPTCHA).
