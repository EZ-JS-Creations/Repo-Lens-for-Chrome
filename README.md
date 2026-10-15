# RepoLens

RepoLens is a Chrome extension that adds an interactive repository explorer to GitHub repository pages.

## Features

- Browse repository files in an interactive tree.
- Search repository files.
- Preview supported files from the repository interface.
- Quickly navigate to repository content on GitHub.
- A compact toolbar with repository actions.

> RepoLens is a community project and is not affiliated with or endorsed by GitHub.

## Install in Chrome (developer mode)

1. Download or clone this repository.
2. Open `chrome://extensions` in Chrome.
3. Enable **Developer mode**.
4. Click **Load unpacked**.
5. Select the folder containing `manifest.json`.
6. Open or refresh a GitHub repository page.

## Development

This is a Manifest V3 Chrome extension. The main files are:

- `manifest.json` — extension metadata, permissions, and entry points.
- `content.js` / `content.css` — GitHub page integration.
- `tree.html`, `tree.js`, `tree.css` — repository tree interface.
- `popup.html`, `popup.js`, `popup.css` — extension popup.
- `background.js` — extension service worker.
- `icons/` — extension icons.

After changing files, return to `chrome://extensions`, click **Reload** for RepoLens, and refresh the GitHub page to test the update.

## Permissions and access

The manifest requests the `storage` permission and access to `github.com` and `api.github.com`. These are used by the extension to integrate with repository pages and retrieve repository data. Review the source code before installing if you want to inspect exactly how data is handled.

## Contributing

Bug reports and pull requests are welcome. Please include reproduction steps and your Chrome version when reporting a problem.

## License

No license has been specified yet. Unless a license is added, standard copyright restrictions apply; please ask the repository owner before redistributing or reusing this code.
