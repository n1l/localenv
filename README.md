# Preparing local development environment
A list of instructions how to prepare local environment

## Install necessary software for development

* git
* vscode
* visual studio
* firefox development edition
* far manager
* ConEmu
* winmerge
* postman
* sql server
* adobe reader

## Configure conemu like quake terminal

[ConEmu quake style](https://conemu.github.io/en/SettingsQuake.html "Settings: Quake style")

## Add new ssh keys to github

[Create new ssh key](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/ "Generating a new SSH key and adding it to the ssh-agent")

## Change gitconfig

```
[user]
    name = <username>
    email = <email>
[alias]
    st = status
    lol = log --stat --graph --decorate
    fap = fetch --all --prune
    please = push --force-with-lease
    co = checkout
    ci = commit
[difftool "code"]
    cmd = code  $LOCAL $REMOTE --diff --wait
[mergetool "code"]
    cmd = code --wait $MERGED
[merge]
    tool = code
[diff]
    tool = code
[core]
    editor = code --wait
```

## Install plugins in visual studio code

* aaron-bond.better-comments
* blairleduc.net-core-starters-pack
* christian-kohler.npm-intellisense
* christian-kohler.path-intellisense
* CoenraadS.bracket-pair-colorizer
* dbaeumer.jshint
* dbaeumer.vscode-eslint
* dbankier.vscode-quick-select
* DotJoshJohnson.xml
* eamodio.gitlens
* EditorConfig.EditorConfig
* eg2.tslint
* eg2.vscode-npm-script
* HookyQR.beautify
* humao.rest-client
* infeng.vscode-react-typescript
* jchannon.csharpextensions
* k--kato.docomment
* ms-vscode.csharp
* ms-vscode.PowerShell
* msjsdiag.debugger-for-chrome
* PKief.material-icon-theme
* ybaumes.highlight-trailing-white-spaces

## Change vscode default settings

```
{
    "extensions.ignoreRecommendations": true,
    "window.zoomLevel": 0,
    "material-icon-theme.showUpdateMessage": false,
    "gitlens.advanced.messages": {
        "suppressCommitHasNoPreviousCommitWarning": false,
        "suppressCommitNotFoundWarning": false,
        "suppressFileNotUnderSourceControlWarning": false,
        "suppressGitVersionWarning": false,
        "suppressLineUncommittedWarning": false,
        "suppressNoRepositoryWarning": false,
        "suppressResultsExplorerNotice": false,
        "suppressShowKeyBindingsNotice": true,
        "suppressUpdateNotice": false,
        "suppressWelcomeNotice": true
    },
    "gitlens.keymap": "alternate",
   "editor.codeLens": false,
    "editor.renderWhitespace": "all",
    "editor.glyphMargin": false,
    "gitlens.historyExplorer.enabled": true
}

```


## Install chocolatey

[Chocolatey](https://chocolatey.org/ "https://chocolatey.org/")

## Add posh git

* Install module:
    ```install-module posh-git```

* Create profile:
    [Create and seetup powershell profile](https://www.howtogeek.com/50236/customizing-your-powershell-profile/ "howtogeek.com")

* Add poshgit to the profile:
    ```import-module posh-git```