<!-- readme-sync:repo:start -->
# hazel

Lightweight update server for Electron apps that works with electron\-updater
<!-- readme-sync:repo:end -->

<!-- readme-sync:header:start -->
<p>
  <a href="https://kitze.io/?ref=kitze%2Fhazel"><img src="https://unavatar.io/x/thekitze" align="left" hspace="12" width="64" height="64" alt="Kitze"></a>
  <strong>Made by <a href="https://kitze.io/?ref=kitze%2Fhazel">Kitze</a></strong><br>
  <a href="https://kitze.io/?ref=kitze%2Fhazel">kitze.io</a> · <a href="https://x.com/thekitze?ref=kitze%2Fhazel">X</a> · <a href="https://youtube.com/kitze?ref=kitze%2Fhazel">YouTube</a>
</p>
<br clear="all">


<h3>More projects by Kitze</h3>
<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://zerotoshipped.com/?ref=kitze%2Fhazel"><img src="https://zerotoshipped.com/ship.png" width="72" alt="Zero To Shipped logo"></a><br>
      <strong><a href="https://zerotoshipped.com/?ref=kitze%2Fhazel">Zero To Shipped</a></strong><br>
      A full-stack starter kit for web and mobile apps.
    </td>
    <td width="50%" valign="top">
      <a href="https://sotto.to/?ref=kitze%2Fhazel"><img src="https://sotto.to/apple-touch-icon.png" width="48" alt="Sotto logo"></a><br>
      <strong><a href="https://sotto.to/?ref=kitze%2Fhazel">Sotto</a></strong><br>
      Voice-to-text for macOS. Local AI, one-time purchase.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://tinkerer.club/?ref=kitze%2Fhazel"><img src="https://app.tinkerer.club/brand/tinkerer-logo-128.png" width="48" alt="Tinkerer Club logo"></a><br>
      <strong><a href="https://tinkerer.club/?ref=kitze%2Fhazel">Tinkerer Club</a></strong><br>
      A private community for builders, self-hosters, and AI tinkerers.
    </td>
    <td width="50%" valign="top">
      <a href="https://sizzy.co/?ref=kitze%2Fhazel"><img src="https://sizzy.co/apple-touch-icon.png" width="48" alt="Sizzy logo"></a><br>
      <strong><a href="https://sizzy.co/?ref=kitze%2Fhazel">Sizzy</a></strong><br>
      The browser for web developers.
    </td>
  </tr>
</table>

<h3>Sponsors</h3>
<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://postiz.com/?ref=kitze%2Fhazel"><img src="https://media.gifs.so/sponsors/50b4a915f9c47b5328b97281/b08730d86b240100fd72d42b828923856d14d82d50eb5698b99cf8e2ca125288.webp" width="40" alt="Postiz logo"></a><br>
      <strong><a href="https://postiz.com/?ref=kitze%2Fhazel">Postiz</a></strong><br>
      Schedule social posts with AI agents.
    </td>
    <td width="50%" valign="top">
      <a href="https://www.founderstack.pro/?ref=kitze%2Fhazel"><img src="https://media.gifs.so/sponsors/bc182e02573bf0e14da0cb0c/f164ca56c7b1d7869e589917f716e58355536eef30854f62c49f711c07a7de96.webp" width="40" alt="FounderStack logo"></a><br>
      <strong><a href="https://www.founderstack.pro/?ref=kitze%2Fhazel">FounderStack</a></strong><br>
      A SaaS stack for your business, without subscriptions.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://matte.app/?ref=kitze%2Fhazel"><img src="https://media.gifs.so/sponsors/4193d8ef8f8b0660107703fe/66b20a60c4d9e1da3d999efe862e86f600ebb5a4ffa3a8b63f40a507fef91f66.webp" width="40" alt="Matte logo"></a><br>
      <strong><a href="https://matte.app/?ref=kitze%2Fhazel">Matte</a></strong><br>
      3D mockups, screen recordings, and video editing.
    </td>
    <td width="50%" valign="top">
      <a href="https://htmlcsstoimage.com/?ref=kitze%2Fhazel"><img src="https://media.gifs.so/sponsors/f4c20d84da68764c3f7a4f67/167bf23cf98b11e2d55ea9aa69f83052daceb881bdea7b76925ffa185ed66d2b.webp" width="40" alt="HTML/CSS to Image logo"></a><br>
      <strong><a href="https://htmlcsstoimage.com/?ref=kitze%2Fhazel">HTML/CSS to Image</a></strong><br>
      Turn HTML/CSS into images, PDFs, and screenshots.
    </td>
  </tr>
  <tr>
    <td colspan="2" valign="top">
      <a href="https://namemyventi.com/?ref=kitze%2Fhazel"><img src="https://media.gifs.so/sponsors/da87180867c3c7451bd30d7b/43ce5be2540cf23d3d7d7104ba829a455a9608861a780e0ec2b35b189695f7ea.webp" width="40" alt="NameMyVenti logo"></a><br>
      <strong><a href="https://namemyventi.com/?ref=kitze%2Fhazel">NameMyVenti</a></strong><br>
      Get your brand shouted out at Starbucks.
    </td>
  </tr>
</table>

<br>

<hr>

<br>
<!-- readme-sync:header:end -->

# Hazel

[![Build Status](https://travis-ci.org/zeit/hazel.svg?branch=master)](https://travis-ci.org/zeit/hazel)
[![XO code style](https://img.shields.io/badge/code_style-XO-5ed9c7.svg)](https://github.com/sindresorhus/xo)
[![Join the community on Spectrum](https://withspectrum.github.io/badge/badge.svg)](https://spectrum.chat/zeit)

This project lets you deploy an update server for [Electron](https://electron.atom.io) apps with ease: You only need to run a single command and fill out two text fields.

The result will be faster and more lightweight than any other solution out there! :rocket:

- Built on top of [micro](https://github.com/zeit/micro), the tiniest HTTP framework for Node.js
- Pulls the latest release data from [GitHub Releases](https://help.github.com/articles/creating-releases/) and caches it in memory
- Refreshes the cache every **15 minutes** (custom interval [possible](#options))
- When asked for an update, it returns the link to the GitHub asset directly (saves bandwidth)
- Supports **macOS** and **Windows** apps
- Scales very nicely across multiple [Now](https://zeit.co/now) instances

## Usage

With [Now CLI](https://zeit.co/download), you can deploy an update server like this:

```bash
now zeit/hazel
```

You'll be asked for the value of two environment variables:

- `ACCOUNT`: Your username or organisation name on GitHub
- `REPOSITORY`: The name of the repository to pull releases from
- `PORT`: The port on which Hazel should run

Once it's deployed, paste the deployment address into your code (please keep in mind that updates should only occur in the production version of the app, not while developing):

```js
const { app, autoUpdater } = require('electron')

const server = <your-deployment-url>
const feed = `${server}/update/${process.platform}/${app.getVersion()}`

autoUpdater.setFeedURL(feed)
```

That's it! :white_check_mark:

From now on, the auto updater will ask your Hazel deployment for updates!

## Options

The following environment variables can be used optionally:

- `INTERVAL`: Refreshes the cache every x minutes ([restrictions](https://developer.github.com/changes/2012-10-14-rate-limit-changes/))
- `PRE`: When defined with a value of `1`, only pre-releases will be cached
- `TOKEN`: Your GitHub token (for private repos)
- `URL`: The server's URL (for private repos - when running on [Now](https://zeit.co/now), this field is filled with the URL of the deployment automatically)

## Statistics

Since Hazel routes all the traffic for downloading the actual application files to [GitHub Releases](https://help.github.com/articles/creating-releases/), you can use their API to determine the download count for a certain release.

As an example, check out the [latest Now Desktop release](https://api.github.com/repos/zeit/now-desktop/releases/latest) and search for `mac.zip`. You'll find a release containing a sub property named `download_count` with the amount of downloads as its value.

## Routes

### /

Displays an overview page showing the cached repository with the different available platforms and file sizes. Links to the repo, releases, specific cached version and direct downloads for each platform are present.

### /download

Automatically detects the platform/OS of the visitor by parsing the user agent and then downloads the appropriate copy of your application.

If the latest version of the application wasn't yet pulled from [GitHub Releases](https://help.github.com/articles/creating-releases/), it will return a message and the status code `404`. The same happens if the latest release doesn't contain a file for the detected platform.

### /download/:platform

Accepts a platform (like "darwin" or "win32") to download the appropriate copy your app for. I generally suggest using either `process.platform` ([more](https://nodejs.org/api/process.html#process_process_platform)) or `os.platform()` ([more](https://nodejs.org/api/os.html#os_os_platform)) to retrieve this string.

If the cache isn't filled yet or doesn't contain a download link for the specified platform, it will respond like `/`.

### /update/:platform/:version

Checks if there is an update available by reading from the cache.

If the latest version of the application wasn't yet pulled from [GitHub Releases](https://help.github.com/articles/creating-releases/), it will return the `204` status code. The same happens if the latest release doesn't contain a file for the specified platform.

### /update/win32/:version/RELEASES

This endpoint was specifically crafted for the Windows platform (called "win32" [in Node.js](https://nodejs.org/api/process.html#process_process_platform)).

Since the [Windows version](https://github.com/Squirrel/Squirrel.Windows) of Squirrel (the software that powers auto updates inside [Electron](https://electron.atom.io)) requires access to a file named "RELEASES" when checking for updates, this endpoint will respond with a cached version of the file that contains a download link to a `.nupkg` file (the application update).

## Programmatic Usage

You can add Hazel to an existing HTTP server, if you want. For example, this will allow you to implement custom analytics on certain paths.

```js
const hazel = require('hazel-server')

http.createServer((req, res) => {
  hazel(req, res)
})
```

## Contributing

1. [Fork](https://help.github.com/articles/fork-a-repo/) this repository to your own GitHub account and then [clone](https://help.github.com/articles/cloning-a-repository/) it to your local device
2. Move into the directory of your clone: `cd hazel`
3. Run the development server: `npm run dev`

## Credits

Huge thanks to my ([@leo](https://github.com/leo)'s) friend [Andy](http://twitter.com/andybitz_), who suggested the name "Hazel" (since the auto updater software inside [Electron](https://electron.atom.io) is called "Squirrel") and [Matheus](https://twitter.com/matheusfrndes) for collecting ideas with me.

## Author

Leo Lamprecht ([@notquiteleo](https://twitter.com/notquiteleo)) - [ZEIT](https://zeit.co)


<!-- readme-sync:footer:start -->
<hr>
<h3>More projects by Kitze</h3>
<h4>Apps &amp; tools</h4>
<table>
  <tr>
    <td width="50%" valign="top">
      <strong><a href="https://gifs.so/?ref=kitze%2Fhazel">gifs.so</a></strong><br>
      Search, copy, and download reaction GIFs.
    </td>
    <td width="50%" valign="top">
      <strong><a href="https://glink.so/?ref=kitze%2Fhazel">Glink</a></strong><br>
      Feedback, roadmaps, changelogs, and discussions.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <strong><a href="https://benji.so/?ref=kitze%2Fhazel">Benji</a></strong><br>
      Tasks, habits, calendar, health, and routines in one place.
    </td>
    <td width="50%" valign="top">
      <strong><a href="https://dmx.to/?ref=kitze%2Fhazel">DMX</a></strong><br>
      A focused desktop client for X.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <strong><a href="https://glink.so/kitze/mindy?ref=kitze%2Fhazel">Mindy</a></strong><br>
      An AI browser that keeps your work organized.
    </td>
    <td width="50%" valign="top">
      <strong><a href="https://glink.so/kitze/supermac?ref=kitze%2Fhazel">Supermac</a></strong><br>
      A macOS command center for everyday workflows.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <strong><a href="https://glink.so/kitze/k67-1787136958277?ref=kitze%2Fhazel">K67</a></strong><br>
      A fork of T3 Code for working with coding agents.
    </td>
    <td width="50%" valign="top">
      <strong><a href="https://perkz.to/?ref=kitze%2Fhazel">Perkz</a></strong><br>
      Sell and manage access to private GitHub repositories.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <strong><a href="https://glink.so/kitze/labz?ref=kitze%2Fhazel">Labz</a></strong><br>
      A platform for teaching workshops and courses.
    </td>
    <td width="50%" valign="top">
      <strong><a href="https://glink.so/kitze/popcorner-1762890546557?ref=kitze%2Fhazel">Popcorner</a></strong><br>
      Organize your movies and TV shows.
    </td>
  </tr>
  <tr>
    <td colspan="2" valign="top">
      <strong><a href="https://glink.so/kitze/champions?ref=kitze%2Fhazel">Champions Online</a></strong><br>
      A free multiplayer card-game platform.
    </td>
  </tr>
</table>

<h4>Open source</h4>
<table>
  <tr>
    <td width="50%" valign="top">
      <strong><a href="https://github.com/kitze/skillbox?ref=kitze%2Fhazel">Skillbox</a></strong><br>
      A self-hosted, versioned skills library for AI agents.
    </td>
    <td width="50%" valign="top">
      <strong><a href="https://github.com/kitze/unclutter?ref=kitze%2Fhazel">Unclutter</a></strong><br>
      Remove page clutter with AI-powered, reusable browser rules.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <strong><a href="https://github.com/kitze/pagegrade?ref=kitze%2Fhazel">PageGrade</a></strong><br>
      Grade page clarity, writing, and on-page SEO.
    </td>
    <td width="50%" valign="top">
      <strong><a href="https://github.com/kitze/council?ref=kitze%2Fhazel">Council</a></strong><br>
      Let your coding agents deliberate together before making a plan.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <strong><a href="https://github.com/kitze/codexmaxx?ref=kitze%2Fhazel">CodexMaxx</a></strong><br>
      Manage Codex accounts, usage, and active sessions on macOS.
    </td>
    <td width="50%" valign="top">
      <strong><a href="https://github.com/kitze/react-hanger?ref=kitze%2Fhazel">React Hanger</a></strong><br>
      A collection of useful React hooks.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <strong><a href="https://github.com/kitze/react-genie?ref=kitze%2Fhazel">React Genie</a></strong><br>
      Animate React elements as they enter the viewport.
    </td>
    <td width="50%" valign="top">
      <strong><a href="https://github.com/kitze/mobx-router?ref=kitze%2Fhazel">MobX Router</a></strong><br>
      A simple router for MobX and React apps.
    </td>
  </tr>
</table>

<p><a href="https://kitze.io/projects?ref=kitze%2Fhazel">All projects</a> · <a href="https://github.com/kitze?ref=kitze%2Fhazel">GitHub</a> · <a href="https://x.com/thekitze?ref=kitze%2Fhazel">Follow on X</a> · <a href="https://youtube.com/kitze?ref=kitze%2Fhazel">YouTube</a></p>
<!-- readme-sync:footer:end -->
