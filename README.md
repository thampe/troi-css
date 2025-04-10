# TROI Improved

A Chrome extension that enhances TROI Software usability by adding clear German button labels.

## Purpose

The sole purpose of this extension is to make the TROI Software interface more intuitive. This is achieved by:
- Adding German text labels to buttons
- Improving spacing between buttons
- Automatic application on all TROI pages

## Installation

1. Download this extension
2. Open Chrome and navigate to `chrome://extensions/`
3. Enable "Developer mode" in the top right corner
4. Click "Load unpacked"
5. Select the directory containing the extension files

## How it Works

The extension:
- Automatically adds CSS styles to TROI pages
- Requires no additional permissions
- Works immediately after installation
- Improves button visibility and clarity

## Development

To modify the CSS styles:
1. Edit the `troi.css` file
2. Reload the extension in `chrome://extensions/`

## Automatic Publishing

The extension is automatically updated in the Chrome Web Store when a new version is released.

### Setting up Automatic Publishing

1. Create a new project in the [Google Cloud Console](https://console.cloud.google.com/)
2. Enable the Chrome Web Store API
3. Create OAuth 2.0 credentials
4. Generate a refresh token
5. Add the following secrets to your GitHub repository:
   - `EXTENSION_ID`: Your Chrome extension ID
   - `CLIENT_ID`: Your OAuth 2.0 Client ID
   - `CLIENT_SECRET`: Your OAuth 2.0 Client Secret
   - `REFRESH_TOKEN`: Your OAuth 2.0 Refresh Token

### Publishing a New Version

1. Update the version in `package.json`
2. Create and push a new tag:
   ```bash
   git tag v1.0.0
   git push origin v1.0.0
   ```
3. The GitHub Action will automatically publish the new version to the Chrome Web Store

## License

MIT