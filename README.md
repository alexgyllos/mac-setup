# Mac Setup

A script to set up a macOS laptop for development.

It can be run multiple times on the same machine safely. It installs, upgrades, or skips packages based on what is already installed on the machine.

Forked from [here](https://github.com/CrugBarat/ANDigital-onboarding-mac-setup)

## Requirements

We support:

- macOS Big Sur (11)
- macOS Catalina (10.15)

Older versions may work but aren't tested.

## Install

(These commands should be run in **Terminal**)

To open Terminal:

1. Press Command+Space and search for Terminal.
2. Hit enter

Copy the below command into Terminal and hit enter:

```sh
curl --remote-name https://raw.githubusercontent.com/alexgyllos/mac-setup/develop/mac
```

Then copy the below command into Terminal and hit enter:

```sh
sh mac 2>&1 | tee ~/laptop.log
```

**You will need to enter your computer password a few times throughout the script to allow installations**

You are all set 🎉🎉🎉 - it should take less than 15 minutes to install (though this depends on your machine).

### Quick Test

At the end of the installation script, another script will run to attempt to check if any applications failed to install. (occasionally may claim some application are missing that aren't)

You can repeat this by running the following lines in terminal (although it's **not required**):

```sh
curl --remote-name https://raw.githubusercontent.com/alexgyllos/mac-setup/develop/laptop_install_test
sh laptop_install_test
```

NB: If you have any issues with running these scripts, please reach out to your AND Onboarding Admin.

---

## What it sets up

### Command line tools:

- [Homebrew](http://brew.sh/) for managing operating system libraries.
- [Git](https://git-scm.com/) for version control
- [Zsh](http://www.zsh.org/) as your command line shell
- [Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh) to add nice features to zsh - autocompletions, shortcuts etc.
- [tree](https://linux.die.net/man/1/tree) for visualising directory structure from the Terminal

### Programming languages and configuration:

- [Node.js](http://nodejs.org/) for JavaScript back-end development, and
- [NPM](https://www.npmjs.org/) for installing JavaScript packages

### GUI Apps:

- [VSCode](https://code.visualstudio.com/) IDE

### Fonts:

- Open Dyslexic for accessibility
