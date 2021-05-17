# Termux Superuser
Runs Android su with all Termux binaries included in superuser mode (implies: we will be able to run binaries nano in su)  
[Rooted Andriod] 

# Motive
Andriod su has few important binaries missing out of the box like "nano". And if you try to add it, it is not persistent (after every boot you are back to square 1).
Termux super user directly uses termux's binaries with Andriod su, avoiding redundancy of binaries in both environment.

# Pre-Requisites
1. Update Termux to latest version:-
  - `$ apt clean`
  - `$ apt update -y`  
  - `$ apt upgrade -y`  
And update once again:
  - `$ apt update -y`
  - `$ apt upgrade -y`
2. Then install git in Termux: `$ pkg install git`
3. Finally Restart Termux to get into updated termux: `$ exit` 

# Setup Instructions
1. Git this repo to HOME directory of Termux: `$ git clone https://github.com/name-is-cipher/termux-superuser $HOME/termux-superuser`
2. change the directory into termux-superuser folder: `$ cd $HOME/termux-superuser`
3. Make "install.sh" executable: `$ chmod +x $HOME/install.sh`
4. Then finally run the installer to install: `$ ./install.sh`
5. et voilà, installation is finshed !!!
6. Run 'xsu' any where to start Termux Superuser.

# Additinol info
- This intallation creates a execuatable "bin" folder in $HOME/.termux folder, you can place your any personal binaries or executables in that folder.
- Unfortunatly aliases can't be exported to termux superuser, but my turnaround solution is make executable file in the name of your alias and past the command inside that file and finally place this executable file in $HOME/bin, by this way aliases can be executed in both the environments.

# Creator
> **Author**: [name_is_cipher](https://github.com/name-is-cipher)  
> **Mail**: aravindswami135@gmail.com
