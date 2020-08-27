
# Auto Import Relative Path (vscode extension)

[![Current version of Auto Import Relative Path][version svg]][package] [![Current installs of Auto Import Relative Path][installs svg]][package] [![Current downloads of Auto Import Relative Path][downloads svg]][package] [![Current ratings of Auto Import Relative Path][ratings svg]][package]

[version svg]: https://vsmarketplacebadge.apphb.com/version-short/electreefrying.auto-import.svg
[installs svg]: https://vsmarketplacebadge.apphb.com/installs/electreefrying.auto-import.svg
[downloads svg]: https://vsmarketplacebadge.apphb.com/downloads/electreefrying.auto-import.svg
[ratings svg]: https://vsmarketplacebadge.apphb.com/rating-short/ElecTreeFrying.auto-import.svg
[package]: https://marketplace.visualstudio.com/items?itemName=ElecTreeFrying.auto-import

Auto import relative path [extension] for [VS Code]. Auto import relative path without typing long and tedious import statements and file paths.

[VS Code]: https://code.visualstudio.com/
[extension]: https://marketplace.visualstudio.com/VSCode

*This extension is my alternative solution of drag and drop import that is currently not available in VS Code.*

> Drag and drop to import files in JS! [#61667][0] </br> 
> Allow to add file reference with drag and drop. [#5240][1]

[0]: https://github.com/microsoft/vscode/issues/61667
[1]: https://github.com/microsoft/vscode/issues/5240

## Features

* [Configure import styles](#import-statements--javascript)
* [Usage](#usage)
* [Import to cursor](#Import-to-cursor)
* [Import to bottom](#Import-to-bottom)
* [Import to top](#Import-to-top)
* _[Keybindings]_
* _[HTML Support]_
* _[Markdown Support]_

[Keybindings]: https://github.com/ElecTreeFrying/auto-import-relative-path/blob/master/DEMO.md#keybindings
[HTML Support]: https://github.com/ElecTreeFrying/auto-import-relative-path/blob/master/DEMO.md#html-support
[Markdown Support]: https://github.com/ElecTreeFrying/auto-import-relative-path/blob/master/DEMO.md#markdown-support

## Supported file types

| Markup Language | Programming Language |  Stylesheet  |
|:---------------:|:--------------------:|:------------:|
|      .html      | .js, .jsx, .ts, .tsx |     .css     |
|       .md       |                      | .scss, .sass |
|                 |                      |     .less    |

## Usage

1. `Ctrl+Shift+A` a file in explorer → `Ctrl+I` in your editor tab. [demo][usage-example-1]
2. or `Alt+D` a file in explorer to automatically import in editor tab. [demo][usage-example-2]

### [Click here for more usage examples.]

[usage-example-1]: https://github.com/ElecTreeFrying/auto-import-relative-path/blob/master/DEMO.md#auto-import-from-explorer
[usage-example-2]: https://github.com/ElecTreeFrying/auto-import-relative-path/blob/master/DEMO.md#single-keybinding-import

[Click here for more usage examples.]: https://github.com/ElecTreeFrying/auto-import-relative-path/blob/master/DEMO.md

![auto-import-demo](https://github.com/ElecTreeFrying/auto-import-relative-path/raw/master/images/playback.gif "auto import relative path demo")

## Commands

| Command              | Key Binding    | Description                                                                          |
| -------------------- | -------------- | ------------------------------------------------------------------------------------ |
| `Auto Import: Copy`  | `Ctrl+Shift+A` | Copy relative path of selected file in explorer.                                     |
| `Auto Import: Paste` | `Ctrl+I`       | Paste import statement on selected tab.                                              |
| `Auto Import: Auto`  | `Alt+D`        | Auto copy and paste import statement of a file from explorer to selected tab.        |

## Configuration Settings

### General settings

* `quoteStyle`: Select quote style for relative import path. *(double/single quote)*
* `importType`: Paste import on selected line, at the top or bottom of the import list.
* `addSemicolon`: Toggle include semicolon at the end of import statement.
* `disableNotifs`: Disable all notifications.

### Import statements > Javascript

* `importStatements.javascript.jsSupport`: Select **.js** import style.
* `importStatements.javascript.jsxSupport`: Select **.jsx** import style.
* `importStatements.javascript.withExtnameJS`: Include file type at the end of relative import path.

### Import statements > Typescript

* `importStatements.typescript.tsSupport`: Select **.ts** import style.
* `importStatements.typescript.tsxSupport`: Select **.tsx** import style.
* `importStatements.typescript.withExtnameTS`: Include file type at the end of relative import path.
* `importStatements.typescript.addExportName`: Toggle component name in import statement. **(Angular feature)**

### Import statements > Stylesheet

* `importStatements.stylesheet.cssSupport`: Select **.css** import style.
* `importStatements.stylesheet.scssSupport`: Select **.scss** import style.
* `importStatements.stylesheet.lessSupport`: Select **.less** import style.
* `importStatements.stylesheet.withExtnameCSS`: Include file type at the end of relative import path.

### Import statements > HTML

* `importStatements.html.htmlScriptSupport`: Select script import style for HTML.
* `importStatements.html.htmlStylesheetSupport`: Select stylesheet import style for HTML.

### Import statements > Markdown

* `importStatements.markdown.markdownSupport`: Select **.md** import style.
* `importStatements.markdown.markdownImageSupport`: Select import style for image import in markdown.

### Settings Preview

![extension-settings-preview](https://github.com/ElecTreeFrying/auto-import-relative-path/raw/master/images/settings.gif "auto import relative path extension settings preview")

## Demo

### Import to cursor

1. `Ctrl+Shift+A` a file in explorer → `Ctrl+I` in your editor tab.
2. or `Alt+D` a file in explorer to automatically import in editor tab.

![extension-settings-preview](https://github.com/ElecTreeFrying/auto-import-relative-path/raw/master/images/cursor.gif "import to cursor using ctrl+i command")

### Import to bottom

1. `Ctrl+Shift+A` a file in explorer → `Ctrl+I` in your editor tab.
2. or `Alt+D` a file in explorer to automatically import in editor tab.

![extension-settings-preview](https://github.com/ElecTreeFrying/auto-import-relative-path/raw/master/images/bottom.gif "import to bottom using ctrl+i command")

### Import to top

1. `Ctrl+Shift+A` a file in explorer → `Ctrl+I` in your editor tab.
2. or `Alt+D` a file in explorer to automatically import in editor tab.

![extension-settings-preview](https://github.com/ElecTreeFrying/auto-import-relative-path/raw/master/images/top.gif "import to top using ctrl+i command")

## To do

- [ ] (Svelte) Add auto import support to **.svelte** file extensions. _**(Aug. 2020)**_
- [ ] (Vue) Add auto import support to **.vue** file extensions. _**(Sept. 2020)**_
- [ ] (Python) Add auto import support to **.py** file extensions.
- [ ] (Java) Add auto import support to **.java** file extensions.
- [ ] (PHP) Add auto import support to **.php** file extensions.

## Installation

  1. Install VS Code v1.42.0 or higher
  2. Launch Visual Studio Code
  3. Enter command `Ctrl+Shift+P` (Windows, Linux) or `Cmd+Shift+P` (OSX)
  4. Select → `Extensions: Install Extensions`.
  5. Choose **Auto Import Relative Path** by _ElecTreeFrying_
  6. Reload Visual Studio Code

## Changelog

See [CHANGELOG] for more information.

[CHANGELOG]: https://github.com/ElecTreeFrying/auto-import-relative-path/blob/master/CHANGELOG.md

## Contributing

* File bugs, or any feature requests in [GitHub Issues].
* Leave a review on [Visual Studio Marketplace].

[Github Issues]: https://github.com/ElecTreeFrying/auto-import-relative-path/issues
[Visual Studio Marketplace]: https://marketplace.visualstudio.com/items?itemName=ElecTreeFrying.auto-import&ssr=false#review-details

## Support

### Donate by Bitcoin (BTC)

bc1q9hjnxk67c9y6tsyp8jde43xg9hacf0kgdxq6jsxl47666d3hk8aqunv0xr

![donate-by-bitcoin](https://github.com/ElecTreeFrying/auto-import-relative-path/raw/master/images/BITCOIN.png "donate by bitcoin")

### Donate by Mining

|      Mining address (NiceHash)     |
|:----------------------------------:|
| 3GJoX9cKs7eUHr6n5LcwNYEkSoD6mEqb1r |

## Related

[More extensions of mine.]

[More extensions of mine.]: https://marketplace.visualstudio.com/publishers/ElecTreeFrying

## License

[MIT]

[MIT]: https://marketplace.visualstudio.com/items/ElecTreeFrying.auto-import/license