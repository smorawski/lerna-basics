# Lerna Cheat Sheet

## Basic commands
`lerna init --independent` - create lerna file. Flag `independent` defines if all packages should be versioned separatly.

`lerna bootstrap --<flags>` - runs `npm i && npm run prepare` on all packages

`lerna clean --<flags>` - clear `node-modules` for all packages

`lerna run <script_name> --<flags>` - runs script defined in each package

`lerna exec <cmd> --<flags>` - runs command for all packages

`lerna publish --<flags>` - publishes packages to npm

## Usefull flags

`--scope=<package-name1>,<package-name2>...` - defines on which packages should command be executed

`--loglevel <silent/verbose/silly/success/failure>` - defines what type of output should be returned to console

`--concurrency <number || 4>` - defines how many threads should be run in parallel

## Available variables

`$LERNA_PACKAGE_NAME` - current package

`$LERNA_ROOT_PATH` - root path of project

<b>Remeber about adding slash before dollar sign, while running command with those variables!</B>


