# My Azure Virtual Machine Setup

## Install Chocolatey

Run the following block in an elevated PowerShell console
```javascript
Set-ExecutionPolicy Bypass -Scope Process -Force; 
[System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; 
iwr https://community.chocolatey.org/install.ps1 -UseBasicParsing | iex
```

## Install essential tools

```
choco install git -y
```

```
choco install vscode -y
```

```
choco install docker-desktop -y
```

## Docker version

Yet to find the details of what are the issues with the most recent Docker Desktop Version. But it is better to use 4.6.0 for Sitecore.Demo.Platform.

```
choco install docker-desktop --version=4.6.0 -y
```


## Other useful tools

- TBD

## Turn on Windows Features

![Windows features](images/turn-windows-features-on-or-off.png)

## Enable optional featurs on Windows

This will make sure Windows Containers can be enabled on Docker Desktop

```
Enable-WindowsOptionalFeature -Online -FeatureName $("Microsoft-Hyper-V", "Containers") -All
```
or, if no restart condition is needed.

```
Enable-WindowsOptionalFeature -Online -FeatureName $("Microsoft-Hyper-V", "Containers") -All -NoRestart
```


## Must have Extentions for VSCode

- Docker
- ESLint
- Markdown All in One
- markdownlint
- Prettier - Code formatter
- Prettier ESLint
- Stylelint
- Tailwind CSS IntelliSense
- Trailing Spaces
- TypeScript Hero
- YAML

## Configure Windows to have a large Page File

Careful, do not make it too large. Run the following in a windows run "type here to search". When the service appears right click and run as an Administrator

```
SystemPropertiesAdvanced
```

Click on "Advance" > "Change" (Virtual Memory) >  

## Install MkCert

```
choco install mkcert -y
```

## Docker cleanup

```
docker system prune -a
```
To uninstall and clean a previous version

<a href="https://github.com/moby/docker-ci-zap" target="_blank">Zap Docker</a>
