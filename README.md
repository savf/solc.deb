# Installation

## AMD64

Install the debian package directly with *apt* to automatically take care of all dependencies:

>`$ sudo apt install ./solc-0.4.24-amd64.deb`

## ARMHF

The package contains a patched version of the *libz3.so.4* library which is needed for the *solc* binary to work. To overwrite the existing *libz3.so.4* on the system, we need to use the *dpkg* parameter `--force-overwrite` during the installation:

>`$ sudo apt -o Dpkg::Options::="--force-overwrite" install ./solc-0.4.24-armhf.deb`
