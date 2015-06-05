# distem-recipes
# Kameleon recipes to generate images for container testing

The recipes install: TAU, OpenMPI over Debian jessie.
Additionally different version of Linux Kernel: 3.2, 3.16 and 4.0 are compiled and installed.
The recipes allows to build imager for LXC and for bare metal.

## How to use them?

First, clone and enter the repository.

```bash
	$ git clone https://github.com/camilo1729/distem-recipes.git
	$ cd distem-recipes/
```

Please change the username in the recipe `jessie-distem-expe.yaml`
before using it. You have to put a valid Grid'5000 user account.
For building an image for Kadeploy using Grid'5000

```bash
	$ kameleon build jessie-distem-expe.yaml -b /tmp/

```
For building an image for LXC using Docker

```bash
	$ kameleon build jessie-tau-lxc.yaml -b /tmp/

```

This will use the /tmp directory to build the image.
