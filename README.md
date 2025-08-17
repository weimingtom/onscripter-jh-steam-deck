# onscripter-jh-steam-deck
[WIP] My ONScripter-jh Steam Deck port

# How to build
* https://www.reddit.com/r/SteamDeck/comments/t8al0i/install_arch_packages_on_your_steam_deck/  
If you have not already, use passwd to create a password for the deck user.  
I setup my deck user password in decktop mode (not game mode), in system settings by GUI (not command line)  
It's necessary when using sudo in command line    
https://www.vnwiki.xyz/linux/cdemu.html  
* $ sudo steamos-readonly disable
* $ sudo pacman-key --init
* $ sudo pacman-key --populate
* $ sudo pacman -S vim
* $ sudo pacman -S gcc glibc linux-api-headers
* $ sudo pacman -S bzip2 sdl2 sdl2_image sdl2_ttf sdl2_mixer fontconfig libjpeg-turbo
* $ make clean
* $ make -j8
* $ ./onscripter
