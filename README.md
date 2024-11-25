# Workspace++ for Obsidian

A plugin for [Obsidian](https://obsidian.md).

This plugin seeks to improve the core workspace plugin, that has very little features.

### Key features
- [ ] Auto save on worksapce change
- [ ] Optimise the data that is stored to represent workspaces (Core plugin is very inefficient)
- [ ] Preserving graph views between workspaces (tabs in the future?)

Might come at the cost of stability.

### Start dev
- Clone this repo into your `VaultFolder/.obsidian/plugins/` folder. (Do not use your main vault)
- `cd` into the repo folder.
- Run `npm i` to initialise and install dependencies.
- Run `npm run dev` to start compilation in watch mode.
- Reload Obsidian to load the new version of your plugin. ([Hot reload plugin](https://github.com/pjeby/hot-reload))
- Enable plugin in settings window.
- Run `npm update` if there are.

### Versioning & Releases

- Update `manifest.json` with your new version number, such as `1.0.1`, and the minimum Obsidian version required for your latest release.
- Update `versions.json` file with `"new-plugin-version": "minimum-obsidian-version"` so older versions of Obsidian can download an older version of the plugin that's compatible.
- Create new GitHub release using your new version number as the "Tag version".
- Upload the files `manifest.json`, `main.js`, `styles.css` as binary attachments. Note: The manifest.json file must be in two places, first the root path of your repository and also in the release.
- Publish the release.

> You can simplify the version bump process by running `npm version patch`, `npm version minor` or `npm version major` after updating `minAppVersion` manually in `manifest.json`.
> The command will bump version in `manifest.json` and `package.json`, and add the entry for the new version to `versions.json`

### Obsidian API Documentation

See https://github.com/obsidianmd/obsidian-api
