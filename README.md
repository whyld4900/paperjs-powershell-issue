## Prerequisite:

- You have https://gitforwindows.org/ installed

## To Test:

- Run `npm i` from powershell or cmd and it will install paper 0.12.11 correctly
- If you remove the .npmrc file and try `npm i` it will fail

## To Grok:

- Powershell cannot handle the square brackets `"preinstall": "[[ $npm_config_heading == 'npm' ]] && npx npm-force-resolutions || true",` from paper's package.json. This project's .npmrc file tells npm to run its commands/scripts with bash. So calling npm commands from powershell really run with bash, thus avoiding the brackets issue.
