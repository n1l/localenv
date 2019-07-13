# Preparing local development environment
A list of instructions how to prepare local environment

## Contents

1. [Install chocolatey](#i-choco-install)
1. [Add posh git](#i-poshgit)
1. [Install software](#i-software)
1. [Configure conemu](#i-conemu)
1. [Add ssh keys](#i-ssh)
1. [Update gitconfig](#i-gitconfig)
1. [VSCode extensions](#i-vscode-extensions)
1. [VSCode settings](#i-vscode-settings)

## <a name="i-choco-install"></a>Install chocolatey

* Execute remote signed scripts -  ``` Set-ExecutionPolicy RemoteSigned```
* [Chocolatey](https://chocolatey.org/ "https://chocolatey.org/")

## <a name="i-poshgit"></a>Add posh git

* Install module:
    ```install-module posh-git```

* Create profile:
    [Create and seetup powershell profile](https://www.howtogeek.com/50236/customizing-your-powershell-profile/ "howtogeek.com")

* Add poshgit to the profile:
    ```import-module posh-git```

## <a name="i-software"></a>Install software

* git
* vscode
* visual studio
* firefox development edition
* far manager
* ConEmu
* postman
* adobe reader
* dnspy

## <a name="i-conemu"></a>Configure conemu

[ConEmu quake style](https://conemu.github.io/en/SettingsQuake.html "Settings: Quake style")

## <a name="i-ssh"></a>Add new ssh keys to github

[Create new ssh key](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/ "Generating a new SSH key and adding it to the ssh-agent")

## <a name="i-gitconfig"></a>Change gitconfig

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
    cmd = code  $LOCAL $REMOTE --diff -rw
[mergetool "code"]
    cmd = code $MERGED -rw
    keepBackup = false
[merge]
    tool = code
[diff]
    tool = code
[core]
    editor = code -rw
[commit]
    verbose = 2
```

## <a name="i-vscode-extensions"></a>Install plugins in visual studio code

* ms-vscode.csharp
* ms-vscode.PowerShell
* msjsdiag.debugger-for-chrome
* ybaumes.highlight-trailing-white-spaces
* eamodio.gitlens
* will-stone.plastic
* usernamehw.errorlens

## <a name="i-vscode-settings"></a>Change vscode default settings

```
{
    "extensions.ignoreRecommendations": true,
    "window.zoomLevel": -1,
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
    "editor.tabSize": 2,
    "editor.insertSpaces": true,
    "editor.detectIndentation": false
}

```