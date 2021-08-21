<header align="center">
    <div align="center">
        <img src="icon.png" alt="Logo" width="96" />
    </div>
    <h1 align="center">Linux Dev Setup</h1>
    <p align="center">Free as in freedom</p>
</header>

## 🐧 Distro

My distro of choice *currently* is [elementaryOS](https://elementary.io/). I find it a perfect balance between productivity, aesthetics, ease of use and reliability. It's based on Ubuntu and generally runs on the latest LTS release.

This setup is fine tuned for elementary but apart from some elementary specific apps most of it should apply to any distro. This setup is also consistent with my mac (for work) and windows (WSL) setup, apart from some platform specific apps.

## 🦊 Web browser

Install [Firefox](https://flathub.org/apps/details/org.mozilla.firefox) from flathub, this will also enable out of box support for flathub on Appcenter (so any other flathub app can be searched for and installed directly from the Appcenter). **Preference** - set search engine to ddg and disable search suggestions.

### Browser extensions

Some extensions I use (synced to account):

- [Bitwarden](https://addons.mozilla.org/en-US/firefox/addon/bitwarden-password-manager/) - OSS password manager
- [Dark Reader](https://addons.mozilla.org/en-US/firefox/addon/darkreader/) - for saving my eyes
- [Don't track me Google](https://addons.mozilla.org/en-US/firefox/addon/dont-track-me-google1/) - removes tracking info from links
- [Facebook Container](https://addons.mozilla.org/en-US/firefox/addon/facebook-container/) - restricts Facebook tracking
- [File Icon for GitHub, GitLab and Bitbucket](https://addons.mozilla.org/en-US/firefox/addon/github-file-icons/)
- [Hide W3Schools](https://addons.mozilla.org/en-US/firefox/addon/hide-w3schools/)
- [Keepa](https://addons.mozilla.org/en-US/firefox/addon/keepa/) - Amazon price tracker
- [Markdown Here](https://addons.mozilla.org/en-US/firefox/addon/markdown-here/) - for composing the *few* emails I write in markdown
- [MetaMask](https://addons.mozilla.org/en-US/firefox/addon/ether-metamask/) - hodl
- [Minimal Twitter](https://addons.mozilla.org/en-US/firefox/addon/min-twitter/)
- [OctoLinker](https://addons.mozilla.org/en-US/firefox/addon/octolinker/) - turns dependencies on GitHub into GitHub project links
- [Raindrop.io](https://addons.mozilla.org/en-US/firefox/addon/raindropio/) - cross browser/device bookmark manager
- [React dev tools](https://addons.mozilla.org/en-US/firefox/addon/react-devtools/)
- [Redux dev tools](https://addons.mozilla.org/en-US/firefox/addon/reduxdevtools/)
- [Snooze tabs](https://addons.mozilla.org/en-US/firefox/addon/snoozetabs/)
- [Svelte dev tools](https://addons.mozilla.org/en-US/firefox/addon/svelte-devtools/)
- [Tabliss](https://addons.mozilla.org/en-US/firefox/addon/tabliss/) - customizing new tab
- [uBlock origin](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/) - for keeping ads and unwantend content/tracking away
- [Wayback machine](https://addons.mozilla.org/en-US/firefox/addon/wayback-machine_new/)
- [Wikiwand](https://addons.mozilla.org/en-US/firefox/addon/wikiwand-wikipedia-modernized/) - snaps cleaner UI on top of wikipedia

## 🛠️ CLI

1. Install core packages:

```sh
sudo apt install git build-essential vim curl wget zsh xclip xsel
```

2. Configure `git`:

```sh
git config --global user.name "First Last"
git config --global user.email email@email.com
```

3. Change machine name:

```sh
sudo vim /etc/hostname
```

4. Install [`ohmyzsh`](https://github.com/ohmyzsh/ohmyzsh)

5. Sync `.zshrc` from [dotfiles](https://github.com/divyanshu013/dotfiles/blob/master/dotfiles/.zshrc) - useful plugins and aliases

### CLI plugins

- [ZSH autosuggestions](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md)
- [ZSH syntax highlighting](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md)
- [bgnotify](https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins/bgnotify) - notifies about long running terminal tasks
- [z](https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins/z)
- [sudo](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/sudo)

### CLI tools

- [gh](https://github.com/cli/cli/blob/trunk/docs/install_linux.md) - GitHub CLI
- [htop](https://github.com/htop-dev/htop) - interactive process viewer
- [fzf](https://github.com/junegunn/fzf#using-linux-package-managers) - fuzzy file finder
- [n](https://github.com/tj/n#third-party-installers) - node installer and version manager
- [fkill-cli](https://github.com/sindresorhus/fkill-cli#install) - fast process killer
- [fx](https://github.com/antonmedv/fx#install) - JSON viewer
- [bat](https://github.com/sharkdp/bat#on-ubuntu-using-apt) - better version of `cat`
- [diff-so-fancy](https://github.com/so-fancy/diff-so-fancy) - makes git diffs fancy
- [neofetch](https://github.com/dylanaraps/neofetch/wiki/Installation#ubuntu) - displays system info
- [pgcli](https://www.pgcli.com/install) - improved postgreSQL CLI
- [ag](https://github.com/ggreer/the_silver_searcher#linux) - fast code search tool
- [cliflix](https://github.com/fabiospampinato/cliflix)
- [jay](https://github.com/nikersify/jay) - JS CLI REPL
- [fd](https://github.com/sharkdp/fd#on-ubuntu) - find utility
- [qrcp](https://github.com/claudiodangelis/qrcp#deb-packages-ubuntu-debian-etc) - file sharing
- [croc](https://github.com/schollz/croc) - file transfer
- [ngrok](https://ngrok.com/download) - localhost sharing
- [yarn](https://classic.yarnpkg.com/en/docs/install#debian-stable)

## 🖥️ Apps

Most apps can be found on appcenter / flathub

- [ULauncher](https://ulauncher.io/) - alfred alternative for linux
  - [Clipboard](https://github.com/friday/ulauncher-clipboard) - clipboard manager
  - [Emoji](https://ext.ulauncher.io/-/github-ulauncher-ulauncher-emoji)
- [Eddy](https://appcenter.elementary.io/com.github.donadigo.eddy/) - for `.deb` files
- Discord
- Telegram
- Zoom
- Spotify
- Brave - for things that *only* works on Chrome
- Typora - markdown note taking app
- VLC
- [Authy](https://snapcraft.io/authy) - 2FA
- [Iriun](https://iriun.com/) - use your phone as camera
- [WOMic](https://wolicheng.com/womic/) - use your phone as microphone
- [DroidCam](http://www.dev47apps.com/) - features both camera and microphone functionality


## 🧑‍💻 Dev

1. [Cascadia Code](https://github.com/microsoft/cascadia-code) - coding font with italics and ligatures
2. Add [GPG](https://help.github.com/en/articles/managing-commit-signature-verification) and [SSH](https://help.github.com/en/articles/connecting-to-github-with-ssh) keys

### Dev tools and apps

Most apps can be found on appcenter / flathub

- [Harvey](https://appcenter.elementary.io/com.github.danrabbit.harvey.desktop/) - color contrast checker
- [Sequeler](https://appcenter.elementary.io/com.github.alecaddd.sequeler) - SQL database client
- [Beekeeper studio](https://github.com/beekeeper-studio/beekeeper-studio) - database client
- [Table Plus](https://tableplus.com/blog/2019/10/tableplus-linux-installation.html) - database client
- Terminal - stock elmentary terminal app
- VSCode
- [Insomnia](https://insomnia.rest/download) - REST client
- [React Native Debugger](https://github.com/jhen0409/react-native-debugger/)
- [Flipper](https://fbflipper.com/docs/getting-started/index/) - React Native stuff
- [ngrok](https://ngrok.com/download) - localhost tunel and forwarding
- [RunJS](https://runjs.app/) - JS playground
- Android Studio - React Native stuff

### VSCode extensions

Some extensions I use (synced):

- Bracket pair colorizer
- Cloak - hides secrets, useful for screencasts
- Diff
- DotENV
- Emoji
- ESLint
- Jest
- Live Share
- Markdown All in One
- Markdown Preview GitHub
- Material Icon Theme
- Noctis (theme set)
- Open In GitHub
- Partial Diff
- Pretteir
- RayThis
- React Native Tools
- Svelte for VS Code
- vscode-spotify
- vscode-styled-components
- EditorConfig for VS Code
- NPM Dependency

## 👀 Related

- [Mac dev setup](https://github.com/divyanshu013/mac-dev-setup)
- [Windows dev setup](https://github.com/divyanshu013/windows-dev-setup)
- [Dotfiles](https://github.com/divyanshu013/dotfiles)

*(a bit outdated)*

## 👋 Author

- [@divyanshu013](https://twitter.com/divyanshu013) please drop me your Linux dev setup tips :)

<a target="_blank" href="https://icons8.com/icon/17842/linux">Linux</a> icon by <a target="_blank" href="https://icons8.com">Icons8</a>
