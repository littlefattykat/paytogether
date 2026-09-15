# TripSplit Pro

A mobile-first, installable trip expense splitter with multi-currency settlement, natural-language entry, receipt capture, offline support, and local-first privacy.

## Features

- Multiple trips and travellers
- Natural-language prefilling such as `Thao paid 120 SGD for dinner for everyone`
- Equal or selected-member expense allocation
- Per-member paid, owed, and net balances
- Minimized debtor-to-creditor settlements
- Multi-currency expenses and settlement currency selection
- Date-specific exchange-rate lookup with Google verification fallback
- Categories, receipt capture, expense editing, and deletion
- JSON backup and restore
- Native share sheet and iPhone home-screen installation
- Offline app-shell caching

## Run locally

Requirements: Node.js 20 or newer.

```bash
npm install
npm run dev
```

Open the local address shown by Vite. To test the production output:

```bash
npm run build
npm run preview
```

## Publish with GitHub Pages

1. Create an empty GitHub repository.
2. Extract the release ZIP.
3. Upload all extracted files and folders to the repository root. Do not upload the outer `TripSplit-Pro-Repository` folder.
4. Commit to `main`.
5. Open repository **Settings > Pages**.
6. Under **Build and deployment**, choose **GitHub Actions**.
7. The included workflow builds and deploys the app after a push to `main`.

If dotfiles are hidden by your operating system, this package also contains `UPLOAD-NOTES.txt` explaining which ones are optional and how to create them through GitHub.

## iPhone installation

Open the published app in Safari, tap Share, and select **Add to Home Screen**.

## Privacy and limitations

Data and receipt images are stored in the current browser. Export a JSON backup before clearing browser data or changing devices. This is an expense-recording utility, not a payment processor. Automatic exchange lookup depends on an external public endpoint and unsupported currencies require manual entry.

## License

MIT
