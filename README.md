# dotfiles
### gnome-terminal
Find the profile id:
``` dconf dump /org/gnome/terminal/legacy/profiles:/ | grep -e "\[\:\|visible-name"```

Load the profile:
```dconf load /org/gnome/terminal/legacy/profiles:/:the_profile_id_you_found/ < gnome-terminal.dconf

To export the profile:
``` dconf dump /org/gnome/terminal/legacy/profiles:/:5d76d981-4755-45d9-9d7f-6a222dfe3c97/ > gnome-terminal.dconf ``` 
