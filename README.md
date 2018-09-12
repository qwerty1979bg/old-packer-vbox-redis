# Packer template to create a REDIS vagrant box using VirtualBox

This repository contains a Packer template for building a vagrant basebox with REDIS installed, using VirtualBox

## Usage

1. [Install Packer](https://www.packer.io/intro/getting-started/install.html#precompiled-binaries)
2. [Install VirtualBox](https://www.virtualbox.org/manual/ch02.html)
3. [Install VirtualBox Extension Pack](https://www.virtualbox.org/manual/ch01.html#intro-installing)
4. Clone this repository and `cd` into it.

Run the following:

```
$ packer build redis64.json
```

At the end, you should have an OVF + VMDK and BOX files ready to use.

(Todo:)
- use ssh keys instead of hardcoded user
- in the worst case - at least remove the user after the provisioning
