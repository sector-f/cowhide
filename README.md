### NAME
Cowhide - cower wrapper for updating AUR packages

### SYNOPSIS
**cowhide** **--builddir** *DIR*|**--update** [**--directory** *DIR*] [**--purge**]

### DESCRIPTION
**cowhide** is a cower wrapper written in bash that simplifies the process of updating AUR packages. It allows the user to download, build, and install updates, and provides the option of editing PKGBUILDs before compiling.

### OPTIONS
`-h` or `--help` Print help information.

`-b` or `--builddirectory <DIR>` Look in DIR for directories that contain PKGBUILDs and give the option of building/installing those packages.

`-u` or `--update` Check for outdated AUR packages and allow the user to download, build, and install the updated packages.

`-d` or `--directory <DIR>` Set the directory that packages are saved to when `-u` is passed. The default is `~/builds`.

`-p` or `--purge` If this option is passed, the folders downloaded by cower will be deleted. The folder they were downloaded to will not be deleted. E.g. `~/builds/linux-git/` will be deleted but `~/builds/` will not. This is to prevent the accidental deletion of preexisting files.
