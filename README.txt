BBJ777x TOKEN — Cloudflare Pages deployment

CONTENTS
- index.html: responsive landing page
- styles.css / script.js: animation, live clocks, interaction and live order-book chart
- assets/bbj777x-logo.png: token logo
- assets/aircraft.png: aircraft visual used in the flight animation
- .well-known/stellar.toml: Stellar asset metadata
- stellar.toml: copy of the metadata file for convenience

DEPLOY
1. In Cloudflare Dashboard, open Workers & Pages and select the Pages project for bbj777xlm.pages.dev.
2. Upload/deploy the contents of the bbj777x-site folder (not the parent folder) as the static site assets, or connect this folder through your Git workflow.
3. Confirm that https://bbj777xlm.pages.dev/.well-known/stellar.toml and https://bbj777xlm.pages.dev/assets/bbj777x-logo.png load publicly.
4. Ensure the Stellar account's home_domain is set to bbj777xlm.pages.dev if you want Stellar wallets/explorers to discover this metadata.

NOTES
- The world clocks use the visitor's browser Intl time-zone database.
- The bottom chart requests the public Stellar Horizon order book for BBJ777x/XLM. If there are no offers or no liquidity, the chart reports that rather than fabricating price history.
- The Trade button currently links to StellarTerm's exchange landing page. Select/verify the exact BBJ777x issuer asset there before trading.
- The aircraft is a high-detail generated visual animated along a CSS flight path, not a real-time 3D simulation.
- Stellar.toml metadata and token logo URLs become live only after deployment.
