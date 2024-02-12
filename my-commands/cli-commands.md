# CLI Commands

A set of valuable aliases and commands in the CLI.

### Copy the current directory path to the clipboard

```bash
alias cpwd="pwd | tr -d '\n' | pbcopy && echo 'pwd copied to clipboard'"
```

### Create a ZIP archive

```bash
zip output_archive_name.zip folder_i_want_to_archive
```

### Create a ZIP archive secured with a password

- `-r` - recursive, add also directories in the directories
- `-e` - encrypt

```bash
zip -er output_archive_name.zip folder_i_want_to_archive
```
