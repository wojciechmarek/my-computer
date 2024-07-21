# Command Line Interface

A set of valuable aliases and commands in the CLI.

# Commands

```bash
# Alias to copy path directly to the clipboard:
alias cpwd="pwd | tr -d '\n' | pbcopy && echo 'pwd copied to clipboard'"

# ZIP a file:
zip output_archive_name.zip folder_i_want_to_archive

# ZIP a file with a password:
zip -er output_archive_name.zip folder_i_want_to_archive
```