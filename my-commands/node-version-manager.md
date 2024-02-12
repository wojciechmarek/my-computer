# Node Version Manager

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
