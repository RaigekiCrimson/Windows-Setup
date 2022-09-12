For Powershell: 

Set-ExecutionPolicy Bypass

Setting Up Chocolatey:

Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))

Restart Powershell

Choco Installs:

choco install firefox chromium slack vscode webstorm git gitkraken audacity vlc obs todoist steam 7zip dropbox raidrive bitwarden github-desktop mailspring windirstat nodejs 
Chris Titus Windows Utility:

git clone https://github.com/ChrisTitusTech/winutil.git

    Launch Command:

        iwr -useb https://christitus.com/win | iex

Updating Packages in Chocolatey:

You can update all packages in Chocolatey using: 

    choco upgrade all -y