# altodots

1. Download necessary stuff:
  yay -S reflector rsync
  sudo reflector --country 'US' --latest 10 --sort rate --save /etc/pacman.d/mirrorlist
  yay -S pywal swww
  yay -S waybar swaync starship myfetch neovim python-pywalfox hypridle hyprpicker hyprshot hyprlock pyprland wlogout fd cava brightnessctl clock-rs-git
  yay -S nerd-fonts
  yay -S nwg-look qogir-icon-theme materia-gtk-theme illogical-impulse-bibata-modern-classic-bin
  yay -S thunar gvfs tumbler eza bottom htop
  yay -S blueman bluez
  yay -S pipewire pipewire-pulse pipewire-alsa pipewire-jack pavucontrol pulsemixer
  yay -S gnome-network-displays gst-plugins-bad
2. Enable services
  systemctl enable bluetooth
  systemctl --user enable pipewire.service pipewire-pulse.service
  systemctl --user start pipewire.service pipewire-pulse.service
  sudo systemctl enable avahi-daemon
3. Copy the files to needed location:
  All files and folders in .config to /home/youruser/.config
  All files in .fonts to /home/youruser/.fonts
  Place your wallpaper in /home/youruser/wallpapers/walls/wallpaper.png
  The rest of the files (.zshrc and .p10k.zsh) place in /home/youruser/
4. Restart the system and you are ready to go!
