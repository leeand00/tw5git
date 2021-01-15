# 1. Install Ansible

```bash
sudo apt-get install ansible
```

# 2. Use the ping module on the locahost

```bash
ansible -m ping localhost
 success => {
   "changed": false,
   "ping": "pong"
}
```

- I don't know why....

# 3. Install curl 

```bash
apt-get install `curl`
```

# 4. Install / Configure `git`

```bash
apt-get install git
apt-get install git-flow
git config --global user.email "helpdeskaleer@gmail.com"
git config --global user.name "Andrew J. Leer"
```

# 5. Install vim

```bash
apt-get install vim
apt-get install vim-gtk
```
# 6. Clone dotifles

```bash
$ git clone http://192.168.57.196:3000/HelpDeskAleerPersonal/dotfiles.git ~
```

# 7. Install Vundle.vim
## (`apt-get` for `vim` bascially...)

```bash
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
# When ./init.sh is run:
#  - Plugins are specified in src/vundle.conf will be auto installed.
#  - Soft symlink will be created to dotfies/.vimrc in ~/.vimrc
cd ~/dotfiles 
./init.sh
```








