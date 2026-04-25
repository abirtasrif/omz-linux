1.  Install zsh
    `sudo apt install zsh`
2.  check the default terminal
    `echo $0`
3.  Make zsh default terminal<br>
    `chsh` <br>
    `/bin/zsh `
4.  Re-login/reboot
5.  Run terminal after rebooting and enter [2] for generating default profile. Confirm the terminal change via step (02)
6.  Install git & curl if not setup
7.  Install oh-my-zsh via curl<br>
    `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
8.  Install powerlevel10k<br>
    `git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k`
9.  Download any [nerd font ](https://www.nerdfonts.com/font-downloads) and copy the font into .fonts folder under HOME. If not present, create one. Or you may use one from this repository

10. Change the "Monospace Text" font from your tweaks/appearance to the Nerd font you've downloaded. Be sure to use the monspace category. Check by scrolling before you confirm.
    You can also go to the terminal preference and change the font from there.
11. Edit the zsh profile<br>
    `gedit ~/.zshrc`
    If your system doesn't have gedit preinstalled, you may also use terminal based editor by using below command<br>
    `nano ~/.zshrc`
12. Find the ZSH_THEME="robbyrussell" and change the theme `robbyrussell` to `powerlevel10k/powerlevel10k`
13. Save and restart terminal.
14. The config page will appear. Just proceed with your choice. (only keep in mind to select unicode in Character set)
15. To reconfigure setting in future, run<br>
    `p9k_configure`

### optional

16. To use in VSCODE terminal, use zsh terminal and change font to one monospace Nerd Font. Example of Daddy font mono and use this value in vscode settings.json<br>
    `"terminal.integrated.fontFamily": "DaddyTimeMono Nerd Font Mono"`

17. you can tweak the configuration by editing `~/.p10k.zsh` file.
    18.to view the color codes of 255 colors, you may run below command in terminal<br>
    `for i in {0..255}; do print -Pn “%K{$i} %k%F{$i}${(l:3::0:)i}%f “ ${${(M)$((i%6)):#3}:+$’\n’}; done`

-ENJOY-
