LAD software environment container utilities
============================================

Local Installation
------------------

*The environment has been tested on linux (requires singularity v3+ or apptainer v1+)
and MacOS (requires docker)*

Please follow the steps below to setup and run the container in your environment.

1. Create a local directory that you want to work in, e.g `$HOME/lad`, and go into this
   directory.
```bash
mkdir $HOME/lad
cd $HOME/lad
```

2. Execute the following line in your terminal to get the install script.
```bash
wget -o https://raw.githubusercontent.com/JeffersonLab/lad-shell/main/install.sh
```
To install execute:
```bash
./install
```
By defult install scirpt install `main` tag container.

To specify the specific release of the container do following.
```bash
./install --version <tag>
```
OR 
if you want to install default container in single line (i.e. `main`)
```bash
curl -L https://raw.githubusercontent.com/JeffersonLab/lad-shell/main/install.sh | bash
```

3. Install script creates a executable file `lad-shell`. Excecute the following to get into the lad-shell cotainer environment.
```bash
./lad-shell
```

4. Within your  environment (`lad-shell`), you can install software to the
   internal prefix `$LAD_SHELL_PREFIX`


NOTE: This is inspired from : https://github.com/eic/eic-shell/tree/main

