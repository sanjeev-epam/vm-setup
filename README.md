# My Azure Virtual Machine Setup

## Run the following block in an elevated PowerShell console
```javascript
Set-ExecutionPolicy Bypass -Scope Process -Force; 
[System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; 
iwr https://community.chocolatey.org/install.ps1 -UseBasicParsing | iex
```

## Chocolatey is ready to use. Run the following to install the essential tools

```
choco install git -y
```

```
choco install vscode -y
```

```
choco install docker-desktop -y
```

## Other useful tools

- TBD

## Turn on Windows Featurs
(images/turn-windows-features-on-or-off.png)


## Turn on Options Windows Features

## Must have for VSCode:

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