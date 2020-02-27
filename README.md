# emoji-code

[![apm](https://flat.badgen.net/apm/license/emoji-code)](https://atom.io/packages/emoji-code)
[![apm](https://flat.badgen.net/apm/v/emoji-code)](https://atom.io/packages/emoji-code)
[![apm](https://flat.badgen.net/apm/dl/emoji-code)](https://atom.io/packages/emoji-code)
[![CircleCI](https://flat.badgen.net/circleci/github/idleberg/atom-emoji-code)](https://circleci.com/gh/idleberg/atom-emoji-code)
[![David](https://flat.badgen.net/david/dep/idleberg/atom-emoji-code)](https://david-dm.org/idleberg/atom-emoji-code)

Snippets to insert escaped Emoji code into a variety of languages, including:

- CSS
- CoffeeScript
- HTML
- JSON
- JavaScript
- LiveScript
- Python
- Ruby
- Twig
- TypeScript

This package is also available for [Sublime Text](https://github.com/idleberg/sublime-emoji-code) and [Visual Studio Code](https://github.com/idleberg/vscode-emoji-code).

![Screenshot](https://raw.github.com/idleberg/atom-emoji-code/master/screenshot.gif)

*Screenshot of completions in Atom with [one-light-ui](https://github.com/atom/one-light-ui)*

## Installation

### apm

Install `emoji-code` from Atom's [Package Manager](http://flight-manual.atom.io/using-atom/sections/atom-packages/) or the command-line equivalent:

`$ apm install emoji-code`

### Using Git

Change to your Atom packages directory:

```bash
# Windows
$ cd %USERPROFILE%\.atom\packages

# Linux & macOS
$ cd ~/.atom/packages/
```

Clone repository as `emoji-code`:

```bash
$ git clone https://github.com/idleberg/atom-emoji-code emoji-code
```

Inside the cloned directory, install Node dependencies:

```bash
$ yarn || npm install
```

## Usage

All emojis are prefixed with `ji`, following the string of the official [Unicode terminology](http://unicode.org/Public/emoji/3.0/emoji-sequences.txt).

**Examples:**

Let's say, you want to insert the 😄 emoji

* HTML: `ji:grinning-face` becomes `&#x1F600;`
* CSS: `ji:grinning-face` becomes `content: '\1F600';`
* JavaScript: `ji:grinning-face` becomes `\u{1F600}`
* Python: `ji:grinning-face` becomes `\U0001F600`
* Ruby: `ji:grinning-face` becomes `\u{1F600}`

Keep in mind that Atom supports fuzzy completion, inviting you to use abbreviation of your preference.

## Contribute
### Setup
1. Fork this repo
1. Clone the fork on your development machine
1. Install dependencies: `npm install`
1. Link package to atom (so you can test changes): `apm link <repo root> --name dev-emoji-code`
1. Disable the official version of `emoji-code` to prevent conflicts

### Workflow
1. `src/build.js` generates the snippets and saves them in `snippets`
1. Run `guard` to build on file changes (or run `npm run build` manually after each change)
   - Note: `guard` needs to be installed: `gem install guard guard-shell`
     (this requires Ruby)
1. Refresh Atom to test changes: `Ctrl+Shift+P` and select `Window: Reload`

## License

This work is licensed under the [The MIT License](LICENSE.md).

## Donate

You are welcome to support this project using [Flattr](https://flattr.com/submit/auto?user_id=idleberg&url=https://github.com/idleberg/atom-emoji-code) or Bitcoin `17CXJuPsmhuTzFV2k4RKYwpEHVjskJktRd`
