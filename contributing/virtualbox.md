If you're working with Windows, or want to enforce separation of concerns within your work environment, consider working in a virtual machine with [VirtualBox](https://www.virtualbox.org/wiki/Downloads).

1. Download virtual box for your host operating system on this page : https://www.virtualbox.org/wiki/Downloads
2. Install VirtualBox on your system, and launch it.
3. Get a Linux flavour of your choice from OSBoxes: [here](http://www.osboxes.org/virtualbox-images/). Recommended images are Xubuntu or Lubuntu, which are 'lighter' variants of Ubuntu, a Debian based Linux distro. If you enjoy migraines, give Arch Linux a shot ;) Go make some coffee as the download will take awhile depending on the speed of your connection.
4. Go make some coffee as it will take awhile depending on the speed of your connection.
5. Open VirtualBox, click on 'New'. Give it a name (e.g. OpenMined Workspace), and choose its type (Linux), and version (Ubuntu 64/32 bit).
6. Click on next, and assign memory to the virtual machine from the host system. Example: If you have 16 GB of RAM on your host machine, assign 4 GB (4096 MB) or more to the virtual machine.
7. Choose 'Use an existing virtual hard disk', and choose the `.vdi` file which was extracted from the zipped/tar file downloaded from OSBoxes.
8. Boot up the virtual machine(password: osboxes.org), and proceed to the instructions found [here](https://github.com/OpenMined/Docs/blob/master/contributing/quickstart.md).