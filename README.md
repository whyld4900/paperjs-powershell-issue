## Assumptions:

- you have https://gitforwindows.org/ installed
- you have an .npmrc setting the script shell (https://docs.npmjs.com/cli/v6/using-npm/config#script-shell) to run with bash

## Test:

- run `npm i` from powershell or cmd and it will install paper 0.12.11 correctly
- if you remove the .npmrc file and try `npm i` it will fail
