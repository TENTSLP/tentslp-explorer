# TENT Token Explorer

A open source block explorer for TENT tokens based on the TENT Simple Ledger Protocol (TENTSLP).

![screenshot](public/img/screenshot.jpg)

## Translations

Please see [TRANSLATIONS.md](TRANSLATIONS.md).

## How to add Token Icon?

Open a PR at https://github.com/TENTSLP/tentslp-token-icons

## Token Verification

The explorer has a list of "verified" tokens in `public/verified_tokens.json`. This is to help reduce the chance of someone namesquatting to perform a con. You should always verify the token id yourself to be sure, but since most people are too lazy to do that there is a checkmark that will appear next to tokens in the search dropdown which shows if they are in the verified list.

If you would like your token to be considered verified open a PR adding the token id to the list and provide some proof you are the owner of the token.

## Building

You need `Make`, `curl`, `npm` installed. 

For running puppeteer you need additional libraries:

```
sudo apt install libx11-xcb-dev libxcb-dri3-dev libxcomposite-dev libxcursor-dev libxdamage-dev libxi-dev libxtst-dev libnss3-dev libcups2-dev libxss-dev libxrandr-dev libgbm-devlibasound2-dev libatk1.0-dev libatk-bridge2.0-dev libpangocairo-1.0-0 libgtk-3-dev
```

To actually build and start perform the following:

```
cp .env.example .env
npm i
make
npm start
```

## Credits

[ciripel](https://github.com/ciripel) ([TENTSLP](https://github.com/TENTSLP)), [blockparty-sh](https://github.com/blockparty-sh) for all the dev work, [James Cramer](https://github.com/jcramer) ([simpleledger](https://github.com/simpleledger)), [kosinusbch](https://github.com/kosinusbch) for stylesheet, and [Evan](https://twitter.com/evanluza) from bitcoin.com for original design files
