# CE-ModConfig-Public
Implementation files and help info for using ModConfig in Conan Exiles

![](https://github.com/rvIceBreaker/CE-ModConfig-Public/blob/main/help/img/readme_preview1.png)

Read the [wiki](https://github.com/rvIceBreaker/CE-ModConfig-Public/wiki) to get started

## What is ModConfig?

ModConfig provides a unified configuration menu for players to change mod settings and a workflow for mod developers to provide user configuration.

For players, ModConfig is built to be aesthetically consistent with Conan Exiles' UI. It aims to provide a solid configuration panel, and work as you expect. Care is taken to ensure features such as controller support, server admin settings, and more work without hassle.

For mod developers, ModConfig is built to be lightweight and require minimal dependencies. It provides a toolkit for your existing projects that is built to be simple, straight forward, flexible and feature-complete.

[Find the Workshop download here](https://steamcommunity.com/sharedfiles/filedetails/?id=2677532812)

## Features

* Define your settings using standardized controls in a consolidated configuration window for users
* Handle changes to client-side and server-side settings without worrying about RPC events
* Integrate with or replace your existing configuration solutions
* Minimal project dependencies, minimal bloat in your project

## Revision handling

In testing, ModConfig soft-fails if revision differences crop up and care is made to ensure changes to the public interface files do not regress in signature or functionality.

It is expected that outdated mods will simply lack newer features or controls but never be forced into an unusable state; maintaining backwards compatibility is always a goal.

## Dependency handling

If users do not have ModConfig installed your mod is not negatively affected, and you can continue to use your existing solutions for end-user configuration in addition to ModConfig if you choose.

ModConfig's dependencies are built to be light-weight and transparent. There are no special data types, structs, enumerations, or objects.
