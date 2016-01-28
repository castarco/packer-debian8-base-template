# Debian Jessie Base Template for Vagrant
In this repo you can find a minimal Debian 8 image for Vagrant.

## Using the already built image
If you don't have special needs for your project you can start with the already built image hosted in Atlas:

```
vagrant init castarco/debian_jessie64
```

A `Vagrantfile` will be created in the current dir. Then, to start the VM you only have to type:
```
vagrant up
```

## Building your own image
If this image doesn't suit your needs you'll have to build your own. First of all, you need to get [Packer](https://www.packer.io/). After that, you need to get [Virtualbox](https://www.packer.io/docs/builders/virtualbox-iso.html):
```
packer build template.json -only=virtualbox-iso
```
based on your needs.

## Contributing
If you think you can improve the building template or the scripts for building the images I'll be glad to merge your changes, just follow these steps:

* Read first the [GitHub using pull requests documentation](https://help.github.com/articles/using-pull-requests/)
* Fork the repo to your own account
* Create a topic branch for your new feature/patch/bugfix
* Apply your modifications
* Run the build to make sure anything got broken
* Commit your changes
* Push your changes to your topic branch
* Create a new pull request from the topic branch


