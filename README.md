<h1 align="center">
  <br>
  <a href="https://github.com/vesparny/marky"><img src="https://cloud.githubusercontent.com/assets/82070/14968420/fd7960b4-10bc-11e6-80ef-a7eb63fb1677.png" alt="Marky" width="200"></a>
  <br>
  Marky
  <br>
  <br>
</h1>

<h4 align="center">A Markdown editor</h4>
<h4 align="center">For OS X, Windows and Linux</h4>
<h5 align="center">Built with Electron and React + Redux</h5>


<p align="center">
  <a href="https://travis-ci.org/vesparny/marky"><img src="https://img.shields.io/travis/vesparny/marky/master.svg" alt="Travis"></a>
  <a href="https://github.com/vesparny/marky/releases"><img src="https://img.shields.io/github/release/vesparny/marky.svg" alt="Release"></a>
  <a href="https://github.com/vesparny/marky/releases"><img src="https://img.shields.io/github/downloads/vesparny/marky/total.svg" alt="Downloads"></a>
  <a href="https://david-dm.org/vesparny/marky"><img src="https://david-dm.org/vesparny/marky/status.svg" alt="Dependency status"></a>
  <a href="https://david-dm.org/vesparny/marky#info=devDependencies"><img src="https://david-dm.org/vesparny/marky/dev-status.svg" alt="Dev dependency status"></a>
</p>



## Install

**Marky** is still under development. You can download the latest version from the [releases](https://github.com/vesparny/marky/releases) page.

Please not that binaries are not signed. If you need them to be signed you can easily do it with your own certificates.


<p align="center">
  <img src="https://cloud.githubusercontent.com/assets/82070/14969062/8ad12e30-10c0-11e6-8537-002630cb2e6a.gif" style="max-width:100%" alt="screenshot" align="center">
</p>

## Features

* Live preview
* GitHub Flavored Markdown support
* Search in Markdown
* Syntax highlighting
* Emoji Support
* Words count
* Resizable panels
* Finder integration (OS X)

## Technologies used

* [electron](https://github.com/electron/electron)
* [React](https://facebook.github.io/react/)
* [Redux](https://github.com/reactjs/redux/)

## Roadmap

Refer to open [issues](https://github.com/vesparny/marky/issues). Also feel free to propose features and report bugs.

## How to Contribute

### Install dependencies

```
$ npm install
```

### Run app

```
$ npm start
```

### Package app

Builds app binaries for OS X, Linux, and Windows.

```bash
$ npm run build
```

To build for one platform:

```bash
$ npm run build -- [platform]
```

Where `[platform]` is `darwin`, `linux`, `win32`, or `all` (default).

The following optional arguments are available:

- `--sign` - Sign the application (OS X, Windows)
- `--package=[type]` - Package single output type.
   - `deb` - Debian package
   - `zip` - Linux zip file
   - `dmg` - OS X disk image
   - `exe` - Windows installer
   - `portable` - Windows portable app
   - `all` - All platforms (default)

Note: Even with the `--package` option, the auto-update files (.nupkg for Windows, *-darwin.zip for OS X) will always be produced.

#### Windows build notes

To package the Windows app from non-Windows platforms, [Wine](https://www.winehq.org/) needs
to be installed.

On OS X, first install [XQuartz](http://www.xquartz.org/), then run:

```
brew install wine
```

(Requires the [Homebrew](http://brew.sh/) package manager.)

### Code Style

[![js-standard-style](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)

## Inspiration

* https://github.com/feross/webtorrent-desktop (the build script has been basically copy-pasted from there)
* https://github.com/chentsulin/electron-react-boilerplate

## License

MIT. Copyright (c) [Alessandro Arnodo](https://alessandro.arnodo.net).
