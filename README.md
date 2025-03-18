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

### 📁 `nxp-phobos`

NXP platform for the PhobOS distribution. PhobOS is a ostree based Debian distribution, it have custom boot configuration and uses the `ostree` tool to manage the system updates.

### 📁 `rpi-deimos`

Raspberry Pi platform for the DeimOS reference distribution. DeimOS is a simple Debian based distribution with default boot configuration and uses `apt` to manage the system updates.

### 📁 `rpi-phobos`

Raspberry Pi platform for the PhobOS distribution. PhobOS is a ostree based Debian distribution, it have custom boot configuration and uses the `ostree` tool to manage the system updates.
