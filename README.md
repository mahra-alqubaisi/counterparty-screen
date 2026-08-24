# Counterparty Screen

Check an Ethereum wallet for sanctions, scams and suspicious connections.

Paste an address and the tool pulls live Ethereum activity, checks the wallets it interacted with against public watchlists, and shows the evidence behind any match.

Live demo: https://counterparty-screen.netlify.app

## Checks

- U.S. Treasury / OFAC sanctions
- Israel NBCTF seizure orders
- FBI Lazarus theft advisory
- ScamSniffer
- MyEtherWallet darklist
- Optional indirect screening through wallets it interacted with

NBCTF and FBI data via OpenSanctions. Chain data from Blockscout. No API keys required.

## How it works

- Known exchanges and routers are skipped during indirect screening to avoid noisy results.
- Results show how much transaction history was actually checked.
- Direct sanctions matches are shown separately from indirect exposure.
- Watchlists are refreshed rather than hardcoded.

## Limitations

The tool only checks Ethereum addresses and Ethereum transactions. Indirect screening checks selected connected wallets, not the entire transaction network. This is a learning project, not a compliance product.

## Licence

MIT for the code.
OpenSanctions data is licensed for non-commercial use under CC BY-NC 4.0.
