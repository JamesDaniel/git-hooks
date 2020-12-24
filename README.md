# Commit message hook automation for local git repositories

## Links
- https://github.com/typicode/husky/tree/master

## Requirements
- nodejs >= 10
- `/bin/bash` exists
- husky config exists in `package.json`
- it is a git repository `npm init`
- hisky is installed `npm install --save-dev husky`

## Debugging issues
- rm -rf .git/hooks
- npm uninstall husky
- npm install --save-dev husky
