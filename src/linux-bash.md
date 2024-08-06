# Linux

The bash linux commands.

## Commands

### basic

```bash
id # details about user's groups
pwd
uname -a # details about kernel
whoami # username
hostname # system's name
whereis docker # all catalogs with a docker file
which docker - # path to the docker executable file
ls # list items in the catalog
ls -l # list the items in a column, shows more details (access rights)
```

### basic (need to install them before usage)

```bash
neofetch # info about the system
htop # the CLI process manager
btop # more advanced CLI prcess manager
```

### systemctl (start a process)

```bash
systemctl start httpd
systemctl --user start httpd # start as user
systemctl stop httpd
systemctl restart httpd
systemcrl disable httpd # remove from the autostart
systemctl status httpd
```

### system (an alternative way to start a process)

```bash
service httpd start
service httpd stop
service httpd restart
```

### kill (terminate the process)

```bash
# PID (Process ID) can bee taken from System Monitor / htop, then:
kill PID
```

### files

```bash
./file # starts a file (or opens it)
touch file.txt # creates a new file
cat file.txt # displays the content of the file
nano file.txt # opens a file in the nano CLI editor
zip /directory # zips a directory
unzip archive # unzip a directory
df # file storage status
```

### dnf (Dandified YUM, a package manager)

```bash
# add a new repository the manager:
sudo dnf config-manager --add-repo https://download.docker.com/linux/fedora/docker-ce.repo 

dnf search docker # search for a docker package in all repos

dnf install docker
dnf install docker httpd tabby # a few packages can be installed under a one command
dnf install /path/to/package.rpm # install from the downloaded file
dnf -y install docker # accepts also all questions

dnf remove docker
dnf check-update docker
dnf upgrade docker
dnf downgrade docker
dnf info docker
```

### chmod (change mode tool)

```bash
-rwxrwxrwx. # full possible rights for all grups

# usually some rights are limited:
-rw-r--r--. 1 steve steve 422 Sep  8 08:55 README.md
drwxr-xr-x. 1 steve steve 254 Sep  8 08:51 src
```
