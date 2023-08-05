# Sway Dotfiles

Clonar repositorios

#Enlace a Carpetas
sudo ln -s /home/luism/dotfilessway/usr/share/sway/ /usr/share
sudo ln -s /home/luism/dotfilessway/etc/sway /etc  
rm -rf ~/.config/foot 
rm -rf ~/.config/waybar 
rm -rf ~/.config/sway 
rm -rf ~/.config/rofi
rm -rf ~/.bashrc
ln -s /home/luism/dotfilessway/home/.bashrc  /home/luism/
ln -s /home/luism/dotfilessway/home/.config/foot /home/luism/.config
ln -s /home/luism/dotfilessway/home/.config/waybar /home/luism/.config
ln -s /home/luism/dotfilessway/home/.config/sway /home/luism/.config
ln -s /home/luism/dotfilessway/home/.config/rofi /home/luism/.config


#Instalar

dnf groupinstall "development tools" -y;
install https://mirrors.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://mirrors.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
install cargo golang inotifywait wlsunset mako light kanshi nmtui swappy playerctl conky wob system-config-printer hplip xfce4-screenshooter  polkit-gnome neovim  calcurse pcmanfm bat lsd file-roller g++  thunar-volman xkill viewnior gtk-murrine-engine gtk2-engines  materia-gtk-theme  xarchiver zsh-autosuggestions zsh zsh-syntax-highlighting redshift thunar-media-tags-plugin thunar-vcs-plugin thunar-archive-plugin thunar-sendto-clamtk udiskie sqlite unrar p7zip;

dnf5 config-manager --add-repo https://download.docker.com/linux/fedora/docker-ce.repo;
install docker-ce docker-ce-cli containerd.io docker-compose-plugin;
go install go.senan.xyz/cliphist@latest;
cargo install sworkstyle;
 sudo dnf install \
  https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm;
sudo dnf install \
  https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm;
