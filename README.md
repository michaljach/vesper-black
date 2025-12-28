![Vesper Preview](preview.png)

# Vesper Black

Black, white and orange flavored dark theme for VSCode based on original Vesper.

<a href="https://marketplace.visualstudio.com/items?itemName=jach.vesper-black"><strong>Install →</strong></a>

> Disclaimer: This was hacked together following a tutorial. I have zero experience building themes. Made for personal usage. Not thoroughly tested at all, might have broken edge cases.

## How to Develop

1. Clone the repository:

   ```bash
   git clone https://github.com/jach/vesper-black.git
   cd vesper-black
   ```

2. Open the project in VS Code:

   ```bash
   code .
   ```

3. Edit the theme colors in `themes/Vesper-black-color-theme.json`

4. To test your changes, press `F5` to open a new VS Code window with your theme applied

5. Adjust colors and save to see updates in the test window

For more information on VS Code theme development, see the [VS Code Theme Documentation](https://code.visualstudio.com/api/extension-types/theme-extension)

## How to Release

1. Ensure all changes are committed and the theme looks good

2. Update the version in `package.json`:

   ```json
   "version": "x.y.z"
   ```

3. Create a git tag for the release:

   ```bash
   git tag vx.y.z
   git push origin vx.y.z
   ```

4. Package the extension:

   ```bash
   npm install -g vsce
   vsce package
   ```

5. Publish to the VS Code Marketplace:
   ```bash
   vsce publish
   ```

Make sure you have a Personal Access Token set up for the VS Code Marketplace before publishing.
