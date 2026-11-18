<div align="center">
  <img src="docs/logo.png" width="96" alt="Osta logo">
  <h1>Osta</h1>
  <p>Add your persona, global rules and language style to your messages in any AI chat.<br>Free, private, open source. Chrome and Firefox.</p>
</div>

## What it does
Osta adds visible context (persona, Globals, Language & Style) to your message at the moment you send it. It is plain text in your message, not a hidden system prompt. Nothing is sent anywhere except the chat you were already typing in.

- 97 expert personas, including **Osta**, one persona for any field
- Globals and Snippets, with drag and drop ordering
- Reply language, dialect, length and tone
- Dark, light or auto theme, RTL support, optional persona compression
- No account, no tracking, no network calls of its own

## Install
Download the latest files from [Releases](../../releases/latest).

**Chrome / Edge / Brave:** unzip `osta-chrome.zip`, open `chrome://extensions`, turn on Developer mode, click **Load unpacked** and pick the folder.

**Firefox:** open `about:addons`, click the gear, **Install Add-on From File**, and choose `osta-firefox.xpi`. Builds are unsigned, so use Firefox Developer Edition or Nightly with `xpinstall.signatures.required` set to `false`.

Store listings (Chrome Web Store, Firefox Add-ons) are coming soon.

## Develop
```bash
cd extension
npm install      # test dependency (jsdom)
npm test         # node:test suite
```
Load `extension/` as an unpacked extension in Chrome to try changes.

### Build release files
```bash
python3 scripts/build.py     # writes dist/osta-chrome.zip and dist/osta-firefox.xpi
```
The build minifies nothing by default. Pass `--minify` to run terser (`npm i -g terser`) on the JavaScript.

## Support
Star the repo, share it, open an issue, or [buy me a coffee](https://buymeacoffee.com/YOUR_NAME).

## License
MIT, see [LICENSE](LICENSE).
