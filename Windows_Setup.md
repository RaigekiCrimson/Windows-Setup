# Windows Setup for Windows 11/10

## For Powershell: 

Set the execution policy to allow running powershell scripts:

`Set-ExecutionPolicy Bypass`

## Setting Up Chocolatey:

`Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))`

Restart Powershell for changes to take effect.

## Choco Installs:

These are the applications to install using chocolatey

`choco install firefox chromium slack vscode webstorm git gitkraken audacity vlc obs todoist steam 7zip dropbox raidrive bitwarden github-desktop windirstat nodejs`

## Chris Titus Windows Utility:

Chris Titus has a wonderful utility to help us configure and control windows settings. With it we can set windows update settings, install software using **winget** and remove unnecessary preinstalled apps.

`git clone https://github.com/ChrisTitusTech/winutil.git`

Launch Command:

`iwr -useb https://christitus.com/win | iex`

## Updating Packages in Chocolatey:

You can update all packages in Chocolatey using: 

`choco upgrade all -y`