BBJ777x TOKEN — Cloudflare Pages site

DEPLOY
1. Upload the contents of this folder to a Cloudflare Pages project (Direct Upload), or connect this folder through Git.
2. The site is static: no build command is required. Set the output directory to the project root if your setup asks for one.
3. After deployment, check:
   https://bbj777xlm.pages.dev/
   https://bbj777xlm.pages.dev/.well-known/stellar.toml
   https://bbj777xlm.pages.dev/assets/bbj777x-logo.png

IMPORTANT
- The trading button currently opens StellarTerm (https://stellarterm.org/), a Stellar DEX interface. It is not a pre-filtered BBJ777x order book. Confirm the asset and issuer inside the exchange before trading.
- Stellar.toml uses the provided issuer and asset code BBJ777x. Make sure this issuer actually issued that exact asset code on Stellar mainnet.
- Stellar asset metadata is discovered by wallets when the issuing account has the home domain set to bbj777xlm.pages.dev. Set the account's home_domain to bbj777xlm.pages.dev using a wallet or Stellar tooling; simply uploading this file does not set the issuer's home domain.
- The logo URL is the deployed /assets/bbj777x-logo.png path.
- Replace the generic token description with your final official project description if needed.

FILES
index.html, styles.css, script.js, assets/, .well-known/stellar.toml, _headers
