# My Azure Virtual Machine Setup

## Copy following block and run in PowerShell
```javascript
Set-ExecutionPolicy Bypass -Scope Process -Force; 
[System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; 
iwr https://community.chocolatey.org/install.ps1 -UseBasicParsing | iex
```

## With Chocolatey ready, copy and run the following tools

```javascript
choco install git -y
```

```javascript
choco install vscode -y
```

```javascript
choco install docker-desktop -y
```

## Other useful tools

```

choco install microsoft-windows-terminal -y 

```

## Turn on Windows Featurs

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