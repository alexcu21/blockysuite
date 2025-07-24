# BlockySuite

A suite of stylish custom blocks for the WordPress Gutenberg editor. This plugin is a proof of concept for extending the block editor with visually appealing and functional blocks.

## Features

- **Curve Separator Block**: Create customizable curved separators for your content sections. Supports color, padding, and curve shape adjustments.
- **Buttons and Links Block**: Add interactive button and link components to your pages.

## Requirements

- WordPress 6.7 or higher
- PHP 7.4 or higher

## Installation

1. **Download or Clone** this repository into your WordPress plugins directory:
   ```sh
   git clone <repo-url> wp-content/plugins/blockysuite
   ```
   Or download and extract the ZIP file into `wp-content/plugins/blockysuite`.

2. **Install Dependencies & Build Assets** (for development or if installing from source):
   ```sh
   cd wp-content/plugins/blockysuite
   npm install
   npm run build
   ```
   > If you only need the plugin for use (not development), you can skip this step if the `build/` directory is present.

3. **Activate the Plugin**:
   - Go to the WordPress admin dashboard.
   - Navigate to **Plugins**.
   - Find **BlockySuite** and click **Activate**.

## Usage

- In the block editor, search for "Curve Separator" or "Buttons and Links" blocks.
- Add and customize them as needed in your content.

## Development

- **Start development build with hot reload:**
  ```sh
  npm run start
  ```
- **Build for production:**
  ```sh
  npm run build
  ```
- **Format code:**
  ```sh
  npm run format
  ```
- **Lint JS:**
  ```sh
  npm run lint:js
  ```
- **Lint CSS:**
  ```sh
  npm run lint:css
  ```
- **Create plugin ZIP:**
  ```sh
  npm run plugin-zip
  ```

## Automated Releases

This repository uses a GitHub Actions workflow to automatically create a new release every time code is merged into the `main` branch:

- The workflow builds the plugin and generates a ZIP file.
- A new GitHub Release is created using the latest tag (or commit SHA if no tag is present).
- The plugin ZIP file is attached to the release for easy download.

You can always find the latest release and download the ready-to-install plugin ZIP from the [Releases page](../../releases).

## License

GPL-2.0-or-later. See [LICENSE](https://www.gnu.org/licenses/gpl-2.0.html) for details.

## Author

- Alex Cuadra ([alexcuadra.dev](https://alexcuadra.dev))

---

*This plugin was scaffolded with the [@wordpress/create-block](https://developer.wordpress.org/block-editor/reference-guides/packages/packages-create-block/) tool.*
