01. Install zsh
sudo apt install zsh
02. check the default terminal
echo $0
03. Make zsh default terminal
chsh
/bin/zsh
04. Re-login/reboot
05. Run terminal after rebooting and enter [2] for generating default profile. Confirm the terminal change via step (02)
06. Install git & curl if not setup
07. Install oh-my-zsh via curl
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
08. Install powerlevel10k
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
09. Download the nerdfonts and copy all fonts into .fonts folder under HOME. If not present, create one
10. Change the "Monospace Text" font from your tweaks/appearance to "MesloLGS NF Regular"
11. Edit the zsh profile
gedit ~/.zshrc
12. Find the ZSH_THEME="robbyrussell" and change the theme robbyrussell to powerlevel10k/powerlevel10k
13. Save and restart terminal.
14. The config page will appear. Just proceed with your choice. (only keep in mind to select unicode in Character set)
15. To reconfigure setting, run-
p9k_configure
