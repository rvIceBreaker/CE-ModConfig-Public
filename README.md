# CE-ModConfig-Public
Implementation files and help info for using ModConfig in Conan Exiles

### ModConfig is currently work-in-progress and invite-only

## What is ModConfig?

ModConfig provides a unified settings menu and workflow for mod developers to provide user configuration.

For players, ModConfig is built to be aesthetically consistent with Conan Exiles and provide a solid set of features that don't lack of functionality. Care is taken to ensure features such as controller support, server admin settings, and more work as you expect.

For mod developers, ModConfig is built to be lightweight and require minimal dependencies. It provides a toolkit of easy modifications to your existing projects that are built to be simple, straight forward, flexible and feature-complete.

## Features

* Define your settings using standardized controls, in a consolidated configuration window for users
* Handle changes to client-side and server-side settings without worrying about RPC events
* Integrate with or replace your existing configuration solutions
* Minimal project dependencies, minimal bloat in your project

## Revision handling

In testing, ModConfig soft-fails if revision differences crop up, and care is made to ensure changes to the public interface files do not regress in signature or functionality.

It is expected that outdated mods will simply lack newer features or controls, but never be forced into an unusable state; maintaining backwards compatibility is always a goal.

## Dependency handling

If users do not have ModConfig installed, your mod is not negatively affected, and you can continue to use your existing solutions to end-user configuration in addition to ModConfig if you choose.

ModConfig's dependencies are built to be light-weight and transparent. There are no special data types, structs, enumerations, or objects.
