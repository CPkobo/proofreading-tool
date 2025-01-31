proofreading-tool
===

[![Build/release](https://github.com/gecko655/proofreading-tool/actions/workflows/electron-release.yml/badge.svg)](https://github.com/gecko655/proofreading-tool/actions/workflows/electron-release.yml)


![proofreading-tool-demo](https://user-images.githubusercontent.com/6166778/116985820-f616d580-ad07-11eb-971f-60ec887cff67.gif)


GUIで動作する文書校正ツール
GUI tool for textlinting.

# Usage

https://gecko655.hatenablog.com/entry/proofreading-tool

# Install
https://github.com/gecko655/proofreading-tool/releases

# How to build

## Prepare
```bash
# Fetch dependencies
npm install
# Build webpack
npm run webpack # or `npm run webpack-prod` or `npm run webpack-watch`
```

## Debug
```bash
npm start
```

## Test
```bash
npm run lint # or `npm run lint:fix` (prettier fixes the code format)
```

## Build for production
```bash
npm run webpack-prod
npm run dist:mac # or `npm run dist:win`
```
The build artifacts should be located under the `dist/` folder.

## Release

- Edit package.json to update version number.
- Push tag with the same version number with prefix 'v'.
```bash
git tag vX.Y.Z
git push --tags
```

- [GitHub Action](https://github.com/gecko655/proofreading-tool/actions) creates a [draft release](https://github.com/gecko655/proofreading-tool/releases)
- Release the draft.

# LICENSE
This software is released under [GPLv3 LICENSE](LICENSE).

This software uses [xpdf(pdftotext)](https://www.xpdfreader.com/), which is released under GPLv3 license.

# special thanks
https://github.com/mixigroup
