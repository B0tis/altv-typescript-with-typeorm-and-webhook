<p align="center" style="font-size: 26px">
	<b>Typescript Boilerplate for alt:V - v4.1.0</b>
</p>
<p align="center">
	<img src="https://thumbs.gfycat.com/FabulousFlawlessLamb-size_restricted.gif" width="350" title="hover text">
</p>

<p align="center">
	<sup>Super Fast Compilation</sup>
</p>

[⌨️ Learn how to script for alt:V](https://altv.stuyk.com/)

[❤️ Become a Sponsor of my Open Source Work](https://github.com/sponsors/Stuyk/)

[💡 Need a Roleplay Script? Try Athena!](https://athenaframework.com/)

[🎮 alt:V Multiplayer for GTA:V](https://altv.mp)

⭐ This repository if you found it useful!

# Features

A simple Typescript Boilerplate that builds incredibly fast using the [SWC Library](https://github.com/swc-project/swc).

-   Full alt:V Type Support for VSCode
-   Built in auto-copy for non-typescript files.
-   Built in handling of multiple resources for compilation.
-   Built in server restart after compilation.
-   Easily expandable resource directory.
-   [altv-pkg](https://github.com/Stuyk/altv-pkg) support for auto-downloading alt:V Server Binaries.
-   Prettier Configuration for code formatting.
-   Tried and tested and used by the Athena Framework for over 1 year.

-   Examples how to use TypeORM for an AltV project
-   Examples for the use and implementation of a Discord webhook
-   Examples of how to customize AltV's server.cfg to suit your needs


# Installation

* [Install NodeJS 16+](https://nodejs.org/en/download/current/)
* [Install GIT](https://git-scm.com/downloads)

## Clone the Repository

Use the command below in any terminal, command prompt, etc.

```sh
git clone https://github.com/Stuyk/altv-typescript
```


## Install the Repository

Use the command below in any terminal, command prompt, etc.

```sh
cd altv-typescript
npm install
```

follow **only step 4** from the [TypeORM website](https://typeorm.io/#installation).

## Configure the Repository

modify the server.cfg:
- modify the [wh_default](https://github.com/BotisDerG/altv-typescript-with-typeorm-and-webhook/blob/cb228b49dad086607e71e1191b9aff04982e4d4c/server.cfg#L25) for the Discord Webhook
	- you can command the Line or just remove the Webhooklink if you dont want to use this
- and fill out the Database Config so the Server can connect to your DB
	- if you want to add a new Table or Column you just have to edit or add a new enity [here](https://github.com/BotisDerG/altv-typescript-with-typeorm-and-webhook/blob/cb228b49dad086607e71e1191b9aff04982e4d4c/src/core/server/modules/db/entities) (and add it to the entities in the index.ts [here](https://github.com/BotisDerG/altv-typescript-with-typeorm-and-webhook/blob/cb228b49dad086607e71e1191b9aff04982e4d4c/src/core/server/modules/db/index.ts#L15))
	- If you want to connect to a database type other than "mariadb", you must also edit the index.ts [here](https://github.com/BotisDerG/altv-typescript-with-typeorm-and-webhook/blob/cb228b49dad086607e71e1191b9aff04982e4d4c/src/core/server/modules/db/index.ts#L9)

## Download Server Files

Use the command below in any terminal, command prompt, etc. This will download all necessary server files from an additional package used by this project.

```sh
npm run update
```

## Build Typescript Files

Use the command below in any terminal, command prompt, etc. This will build your TypeScript code into JavaScript.

```sh
npm run build
```

## Start Production Server (Windows)

Run this command to run the server in production mode.

```
npm run windows
```

## Start Production Server (Linux)

Run this command to run the server in production mode.

```
npm run linux
```

## Start Developer Server (Windows)

Run this command to run the server in development mode.

```
npm run dev
```

## End Server Runtime

Use the key combination `ctrl + c` to kill your server in your terminal, command prompt, etc.

## How to Add Mods, and New Resources

This quickstart repository for Typescript allows mods.

However, **do not put your resources in the `resources` folder**.

Instead you should put resources, mods, etc. in the `src` folder in their own folder. They will be automatically copied to the `resources` folder after the code is transpiled.
