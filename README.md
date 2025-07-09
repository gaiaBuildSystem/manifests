# Gaia Manifests

<p align="center">
    <img src="./.assets/repo.png" height="220" />
</p>

These are the manifests for the Gaia project. They are used to build Debian based Linux distributions with multi-layer cookbooks.

The manifest are organized by folder, each folder contains a `manifest.json` file that describes the layers that are part of a Linux distro. The folder name is the `<platform>-<distro>`.


## Usage

Copy the desired `manifest.json` to the root of the work directory that you cloned the Gaia core git repo and run the following command:

```bash
./gaia/scripts/init
```

## Manifests

### 📁 `dev-phobos`

Development manifest for the PhobOS distribution. PhobOS is a ostree based Debian distribution, it have custom boot configuration and uses the `ostree` tool to manage the system updates. This manifest get all the layers supported by the PhobOS and is commonly used for development purposes.

### 📁 `nxp-phobos`

NXP platform for the PhobOS distribution. PhobOS is a ostree based Debian distribution, it have custom boot configuration and uses the `ostree` tool to manage the system updates.

### 📁 `qemu-phobos`

QEMU platform for the PhobOS distribution. PhobOS is a ostree based Debian distribution, it have custom boot configuration and uses the `ostree` tool to manage the system updates. This manifest has the minimum required layers to run the PhobOS distribution in QEMU emulators.

### 📁 `rpi-deimos`

Raspberry Pi platform for the DeimOS reference distribution. DeimOS is a simple Debian based distribution with default boot configuration and uses `apt` to manage the system updates.

### 📁 `rpi-phobos`

Raspberry Pi platform for the PhobOS distribution. PhobOS is a ostree based Debian distribution, it have custom boot configuration and uses the `ostree` tool to manage the system updates.

### 📁 `intel-deimos`

Intel x86_64 platform for the DeimOS reference distribution. DeimOS is a simple Debian based distribution with default boot configuration and uses `apt` to manage the system updates.

### 📁 `intel-phobos`

Intel x86_64 platform for the PhobOS distribution. PhobOS is a ostree based Debian distribution, it have custom boot configuration and uses the `ostree` tool to manage the system updates.

### 📁 `wsl-torizon`

Create the Torizon for WSL 2 Development Environment.This was especially designed for have an already set up development environment for [Torizon](https://www.torizon.io/) and the [Torizon IDE Extension for Visual Studio Code](https://developer.toradex.com/torizon/application-development/ide-extension/) in an easy way.
