# <h3>Oh My Venus</h3>
![Preview](2025-06-17_00-22.png)

- [`fonts_and_terminals.md`](fonts_and_terminals.md) – Panduan install font dan terminal di berbagai distro.
- [`cheatsheet.md`](cheatsheet.md) – Cheat Sheet (Shortcuts)

<h1>Setup</h1>

```bash
# ==============================================
#            LINUX / DWM SETUP TOOLS           
# ==============================================
Defaults Layouts [F] Move Layouts to [M] gapplesgrid shortcut windows + Tab

user@linux:~$ rofi -dump-config > config.rasi  
user@linux:~$ cd .dwm  

user@linux:~/.dwm$ sudo mv menu bar dmenu_run /usr/local/bin/  
user@linux:~/.dwm$ sudo mv dark-owl.rasi /usr/share/rofi/themes/
user@linux:~/.dwm$ mv .Xresources /home/$USER/ && xrdb -merge ~/.Xresources
user@linux:~/.dwm$ sudo make install && sudo make clean install  
user@linux:~/.dwm$ exit  

# ==============================================
#             NOTES & TROUBLESHOOTING            
# ==============================================

# [!] Replace '$USER' with your actual username  
# [!] Requires sudo privileges for system paths

