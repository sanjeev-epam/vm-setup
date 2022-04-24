# My Azure Virtual Machine Setup

## Copy following block and run in PowerShell
```javascript
Set-ExecutionPolicy Bypass -Scope Process -Force; 
[System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; 
iwr https://community.chocolatey.org/install.ps1 -UseBasicParsing | iex

## With chocolatey ready, do the following

```javascript
choco install git -y

```javascript
choco install vscode -y

```javascript
choco install docker-desktop -y```

## Usage
```javascript
import copyCodeBlock from '@pickra/copy-code-block';
// OR
const copyCodeBlock = require('@pickra/copy-code-block');
```

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