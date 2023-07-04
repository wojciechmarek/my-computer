# My Computer

This repo contains a loose set of programs, extensions as well as commands I like to use. I use them on my Mac, so they are not guaranteed to exist or work on other platforms.

## Table of Contents

- [Software](#software)
- [Legacy software](#legacy-software)
- [VS Code Extensions](#vs-code-extensions)
- [Web Development](#web-development)
- [Brew](#brew)
- [Node Version Manager](#node-version-manager)

## Software

List of software I use on my Mac.

### Development

- [VS Code](https://code.visualstudio.com/)

### Web Browsers

- [Brave Browser](https://brave.com/)
- [Google Chrome](https://www.google.com/chrome/)
- [Firefox Developer Edition](https://www.mozilla.org/en-US/firefox/developer/)
- [Safari](https://www.apple.com/safari/)
- [Edge](https://www.microsoft.com/en-us/edge)

### Design

- [Figma](https://www.figma.com/)
- [Just Color Picker](https://annystudio.com/software/colorpicker/)
- [Blender](https://www.blender.org/)
- [Pixelmator](https://www.pixelmator.com/)

### Communication

- [Microsoft Teams](https://www.microsoft.com/en-us/microsoft-365/microsoft-teams/group-chat-software)
- [Zoom](https://zoom.us/)

### English Language

- [DeepL](https://www.deepl.com/translator)
- [Grammarly](https://www.grammarly.com/)

### Productivity

- [Trello](https://trello.com/)
- [Spotify](https://www.spotify.com/)
- [BreakTimer](https://apps.apple.com/us/app/breaktimer/id1196200164?mt=12)
- [eqMac](https://eqmac.app/)
- [Rectangle](https://rectangleapp.com/)

### Utilities

- [Docker](https://www.docker.com/)
- [Postman](https://www.postman.com/)
- [Robo 3T](https://robomongo.org/)
- [Virtual Box](https://www.virtualbox.org/)
- [Responsively](https://responsively.app/)

### Terminals

- [Tabby](https://tabby.io/)
- [Cool Retro Term](https://github.com/Swordfish90/cool-retro-term)

## Legacy Software

List of software I used to use on my Mac and Windows.

### Legacy development

- [Visual Studio](https://visualstudio.microsoft.com/)
- [Rider](https://www.jetbrains.com/rider/)
- [WebStorm](https://www.jetbrains.com/webstorm/)

### Legacy Web Browsers

- [Internet Explorer](https://en.wikipedia.org/wiki/Internet_Explorer)

## VS Code Extensions

List of VS Code extensions I use.

### General

- [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
- [Bracket Pair Colorizer](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer)
- [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
- [Color Highlight](https://marketplace.visualstudio.com/items?itemName=naumovs.color-highlight)
- [DotENV](https://marketplace.visualstudio.com/items?itemName=mikestead.dotenv)

### Git

- [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
- [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)

### Theme

- [Luvia Theme](https://marketplace.visualstudio.com/items?itemName=maciekkoks.luvia-theme)

### Tools

- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
- [Rest Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client)
- [SVG Viewer](https://marketplace.visualstudio.com/items?itemName=cssho.vscode-svgviewer)
- [Quokka](https://marketplace.visualstudio.com/items?itemName=WallabyJs.quokka-vscode)
- [Power Mode](https://marketplace.visualstudio.com/items?itemName=hoovercj.vscode-power-mode)

### Linters

- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [stylelint](https://marketplace.visualstudio.com/items?itemName=stylelint.vscode-stylelint)
- [SonarLint](https://marketplace.visualstudio.com/items?itemName=SonarSource.sonarlint-vscode)
- [Web Accessibility](https://marketplace.visualstudio.com/items?itemName=MaxvanderSchee.web-accessibility)

## Web Development

A set of useful commands for web development.

### Cloudflare

You can set up a tunnel to your local server using Cloudflare's Tunnel (formerly Argo Tunnel). You can expose your local server to other people on the internet.

```bash
brew install cloudflared
cloudflared tunnel --url http://localhost:5500
```

### Modern port kill

NPM way to kill a port.

```bash
npx kill-port 8080
```

### Old-school port kill

Native kill a port.

```bash
lsof -i tcp:[port]
kill -9 [process_id]
```

or a combination of the two:

```bash
lsof -ti tcp:[port] | xargs kill
```

### Light Server

Light Server is a simple, zero-configuration command-line http server. By default, it serves the current directory on port 8080.

```bash
npx http-server
```

```bash
npx http-server -p 5500
```

### WiFi Password

Get your WiFi password.

```bash
npx wifi-password-cli
```

### Remove node_modules

Remove node_modules folder and all its content.

```bash
npx npkill
```

### My IP

Get your public IP address.

```bash
npx public-ip-cli
```

## Brew

A set of useful commands for [Brew](https://brew.sh/).

### List of installed packages

```bash
brew list
```

### Package info

```bash
brew info [package]
```

### Brew manager update

```bash
brew update
```

### Package update

```bash
brew upgrade [package]
```

### List of all outdated packages

```bash
brew outdated
```

### Install package outside the quarantine

```bash
brew install --cask --no-quarantine [package]
```

## Node Version Manager

A set of commands for Node Version Manager (NVM).

### List of installed versions

```bash
nvm ls
```

### Brew package info

```bash
brew info [package]
```

### Install a specific version

```bash
nvm i 14
```

or more specific:

```bash
nvm i 13.1.4
```

### Uninstall a specific version

```bash
nvm uninstall 13.0.0
```

### Run a code with a specific version

```bash
nvm exec [version] [command]
```

### Change globally a version of Node

```bash
nvm use 13
```

### Return to the version of Node that was installed on the system

```bash
nvm use system
```
