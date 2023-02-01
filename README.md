# Mac Setup

## Install OX X Command Line Tools

```bash
xcode-select --install
```

## Install Ansible

```bash
python3 -m pip install ansible
```

## Get this repo

```bash
mkdir ~/projects
cd projects
git clone https://github.com/rteabeault/mac-setup
cd mac-setup
```

## Download Playbook Requirements

```bash
~/Library/Python/3.9/bin/ansible-galaxy install -r requirements.yaml
```

## Run Playbook

```bash
~/Library/Python/3.9/bin/ansible-playbook osx.yaml --ask-become-pass
```

## Post Install Steps
* Login to 1password
* Start Chrome and login to google.
* Move github ssh private key to .ssh dir
* Setup Dropbox
* Setup Calibre
    * Make ~/Dropbox/Apps/Calibre available offline
    * Make ~/Dropbox/Public available offline
    * Start Calibre and ensure that it is using the config from ~/Dropbox/Apps/Calibre
* Login to Spotify
* Login to Discord
* Login to Slack
* Setup Obsidian
    * Clone git@github.com:rteabeault/notes.github
    * Set Obsidian to use this folder.

## TODO
* Enable home directory in finder
* Ensure .ssh directory exists
