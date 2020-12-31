<p align="center" style="font-size: 26px">
	<b>GTA V Role Play playground for alt:V server</b>
</p>
<p align="center" style="font-size: 26px">
	[ <a href="https://altv.mp">altv.mp</a> | <a href="https://stuyk.com/">Thanks Stuyk</a> ]
</p>

## Documentation links

-   [ALT Client Docs](https://docs.altv.mp/js/api/alt-client.html)
-   [ALT Server Docs](https://docs.altv.mp/js/api/alt-server.html)
-   [Native Docs](https://natives.altv.mp/)
-   [Unofficial alt:V Docs](https://stuyk.github.io/altv-javascript-guide/)

⭐ This repository if you found it useful!

### Excerpt

alt:V has a lot of Boilerplates for TypeScript. However, they have one feature missing. They fail to create an environment where you can support multiple resource compilations. This boilerplate aims to fix that and allow multiple resources to be compiled at once and all your mods.

### Features

-   Full alt:V Type Support for VSCode
-   Built in script auto-compilation through `npm run watch`.
-   Built in auto-copy for non-typescript files.
-   Built in handling of multiple resources for compilation.
-   Easily expandable resource directory.
-   [altv-pkg](https://github.com/Stuyk/altv-pkg) support for auto-downloading alt:V Server Binaries.
-   Prettier Configuration for code formatting.

### Installation

[Get NodeJS 13+](https://nodejs.org/en/download/current/)

Install the node modules

```sh
npm install
```

Download Server Files

```sh
npm run update
```

Build Typescript Files

```sh
npm run build
```

### Start the Server

Use any of the following commands to start it.

Based on your environment.

| Linux        | Windows (CMD)     | Windows (Powershell) |
| ------------ | ----------------- | -------------------- |
| `./start.sh` | `altv-server.exe` | `./altv-server.exe`  |

<br />

### Development Mode

If you wish to work your game-mode simply open up VSCode. Open up a terminal and split it (`Ctrl + Shift + 5`).

Run the following in a terminal:

```sh
npm run watch
```

Run your server in another terminal:

| Linux        | Windows (CMD)     | Windows (Powershell) |
| ------------ | ----------------- | -------------------- |
| `./start.sh` | `altv-server.exe` | `./altv-server.exe`  |

<br />

### End Server Runtime

`ctrl + c` to kill your server.

### Reload changed resources

Directly on running server terminal type `reload RESOURCE_NAME` to reload module.

### src vs src-copy

### src

This folder should be used to write your typescript based game modes.

### src-copy

This folder should be used to copy car mods, mlos, etc. to your resources folder after compilation.

Simply add your modded resources, resource dependencies, etc. into this folder.

The build script will handle the rest.
