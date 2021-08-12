# Deprecated
A modules won't load it's dependencies. Please do not use it.

# snpm
Some well-good npm wrapper that saves your storage space.

## What's the difference?
Normally, normal `npm` will install a package in `node_modules` directory at each nodejs project which is sometime **Waste your storage as well**.
While snpm is linking it's `node_modules` to it's **Main Directory** that located at `~/.snpm` and install package on that directory as well which is **Saves your Storage** because they're only **Link** to snpm `node_modules`.

This wrapper is only some experiment that i made to saves my storage space for good. 
Because this wrapper is only experiment wrapper, Don't expect something is good / completely good. There's also some part that i should fix it. You're also free to open PR for some changes.

## Requirements
- Has [NodeJS](https://nodejs.org) installed with `npm`

## Installing
```bash
curl -L# https://raw.githubusercontent.com/Yonle/snpm/master/snpm -o $PREFIX/bin/snpm
chmod +x $PREFIX/bin/snpm
```

## Variables
* `PKGS_DIR` is used to locate where a package should be stored / where it's stored. Default is `~/.snpm`
* `NPM_BINS` is used to locate where `npm` binary located. Used to execute a command. Default is `$PREFIX/bin/npm`

## Installing packages
```bash
snpm install <pkg name. Use space to install multiple package>
```

## Uninstalling packages
To uninstall packages, Go to `~/.snpm` directory, There's a binary files called `remove`. Do `./remove [package name that want to removed]`. 

Alternative, Do `snpm remove [pkg name]`

