![2by2 Project](https://github.com/2by2-Project/manifest/raw/Vanadium/images/2by2-logo-landscape.png)

## Getting Started

To get started with the 2by2 Project sources, you'll need to get
familiar with [Git and Repo](https://source.android.com/setup/build/downloading).

To initialize your local repository, use command:

```bash
repo init -u https://github.com/2by2-Project/manifest.git -b Vanadium --git-lfs
```

Then sync up:

```bash
repo sync -j$(nproc --all)
```

## Building the System

Initialize the ROM environment with the envsetup.sh script.

```bash
. build/envsetup.sh
```

Lunch your device after cloning all device sources if needed.

```bash
lunch devicecodename-buildtype
```

Start compilation

```bash
m bacon
```
