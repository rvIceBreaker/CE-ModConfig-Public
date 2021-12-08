# CE-ModConfig-Public
Implementation files and help info for using ModConfig in Conan Exiles

## What is ModConfig?

ModConfig provides a framework for mods to expose settings to end-users.

Mod authors have the ability to define and handle client-side settings or server-side settings in a simple way, without requiring a ton of additional work.

## Features

* Define your settings using standardized controls, in a consolidated configuration window for users
* Handle changes to client-side and server-side settings without setting up RPC events
* Integrate with or replace your existing configuration solutions
* Minimal project dependencies, minimal bloat in your project

### For Users
ModConfig provides a clean, friendly panel to tweak the settings of mods that you use. For users, it focuses on being easy to use, and integrating into Conan Exiles as if this functionality was built in.

You can tweak settings for either your local client or server-side settings in a unified window, using standard controls that fit into the rest of the Conan Exiles UI/UX.

### For Developers
For developers, ModConfig maintains a focus on keeping control in the hands of mod authors, as well as being lightweight and easy to integrate into existing projects.

You can intuitively define settings and their associated controls, and capture changes by end-users

* Get/Set functions are provided by a single interface object
* Procedurally define your settings structure (both client and server) in one function call
* Control how settings and their values are exposed and displayed to the end-user

ModConfig tries to simplify the process for you without taking away control

* Client-server RPC calls are handled internally to pass along client-to-server settings changes
* All UI functionality is stored inside ModConfig
* Changes to server-side settings are pre-validated, but can be validated by your mod as well
* Settings changes make no assumptions about how you serialize your data, and can be integrated into existing schemes

## Revision handling

In testing, ModConfig soft-fails if revision differences crop up, and care is made to ensure changes to the public interface files do not regress in signature or functionality.

It is expected that outdated mods will simply lack newer features or controls, but never be forced into an unusable state; maintaining backwards compatibility is always a goal.

## Dependency handling

If users do not have ModConfig installed, your mod is not negatively affected, and you can continue to use your existing solutions to end-user configuration in addition to ModConfig if you choose.

ModConfig's dependencies are built to be light-weight and transparent. There are no special data types, structs, enumerations, or objects.