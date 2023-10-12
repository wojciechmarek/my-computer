# My commands

This repository contains a set of CLI commands I use in my daily work.

## Table of Contents

- [Legacy software](#legacy-software)
- [Web Development](#web-development)
- [Brew (MacOS Package Manager)](#brew)
- [Node Version Manager](#node-version-manager)
- [CLI Aliases](#cli-aliases)
- [ZIP Commands](#zip-commands)

## Legacy Software

The list of software I used to use months or years ago; currently, I do not use it or use it occasionally.

### Legacy Languages

- [C#](https://docs.microsoft.com/en-us/dotnet/csharp/)
- [C++](https://docs.microsoft.com/en-us/cpp/cpp/?view=msvc-160)
- [C](https://docs.microsoft.com/en-us/cpp/c-language/?view=msvc-160)

### Legacy development

- [Visual Studio](https://visualstudio.microsoft.com/)
- [Rider](https://www.jetbrains.com/rider/)
- [WebStorm](https://www.jetbrains.com/webstorm/)
- [ReSharper](https://www.jetbrains.com/resharper/)
- [Microsoft SQL Server Management Studio](https://docs.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver15)

### Legacy Frameworks

- [Windows Forms](https://docs.microsoft.com/en-us/dotnet/desktop/winforms/?view=netdesktop-5.0)
- [WPF](https://docs.microsoft.com/en-us/dotnet/desktop/wpf/?view=netdesktop-5.0)
- [Xamarin](https://dotnet.microsoft.com/apps/xamarin)
- [ASP.NET (Core)](https://docs.microsoft.com/en-us/aspnet/core/?view=aspnetcore-5.0)
- [Entity Framework (Core)](https://docs.microsoft.com/en-us/ef/core/)
- [AVR & ATmega micro-controllers](https://en.wikipedia.org/wiki/AVR_microcontrollers)
- [Arduino](https://www.arduino.cc/)

### Legacy Web Browsers

- [Internet Explorer](https://en.wikipedia.org/wiki/Internet_Explorer)

### Legacy Design

- [Paint](https://en.wikipedia.org/wiki/Microsoft_Paint)
- [Gimp](https://www.gimp.org/)

## Web Development

A set of useful general commands for web development.

### Cloudflare

The tunnel to your local server using Cloudflare's Tunnel (formerly Argo Tunnel). You can expose your local server to other people on the internet (e.g. to the client/managers during tedious "Meeting Driven Development" sessions on Teams / Zoom / etc.)

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

Light Server is a simple, zero-configuration command-line HTTP server. By default, it serves the current directory on port 8080.

```bash
npx http-server
```

```bash
npx http-server -p 5500
```

### Remove node_modules

Remove node_modules folder and all its content.

```bash
npx npkill
```

### WiFi Password

Get your WiFi password.

```bash
npx wifi-password-cli
```

### My IP

Get your public IP address.

```bash
npx public-ip-cli
```

### Speed Test

Test your internet connection speed.

```bash
npx speed-test
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

### Install the package outside the quarantine

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

or more specifically:

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

## CLI Aliases

A set of valuable aliases for the command line.

### Copy the current directory path to the clipboard

```bash
alias cpwd="pwd | tr -d '\n' | pbcopy && echo 'pwd copied to clipboard'"
```

## ZIP commands

A set of useful ZIP commands

### Create a ZIP archive

```bash
zip my_archive.zip folder_i_want_to_archive
```

## Create a ZIP archive secured with a password

- `-r` - recursive, add also directories in the directories
- `-e` - encrypt

```bash
zip -er my_archive.zip folder_i_want_to_archive
```

