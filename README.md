# Mecha Bar
![Mecha Bar](/preview/v1.1.png)

## System Information
> **Note:** This configuration is initially tested and optimized for a laptop with the following system setup:

- **Operating System**: Arch Linux
- **Display Server**: Wayland
- **Window Manager**: Hyprland
- **Monitor Resolution**: 1920x1080

## Dependencies
To ensure Mecha Bar works properly, make sure to install the following dependencies:
- pipewire
- wireplumber
- pavucontrol
- playerctl
- brightnessctl
- python
- rofi
- wlogout
- ttf-jetbrains-mono-nerd
- networkmanager

## Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/Sejjy/MechaBar.git
   cd MechaBar
   ```
   
2. **Copy the configuration files:**
    
    Copy the `config.jsonc` and `style.css` files to `~/.config/waybar`:
    ```bash
    mkdir -p ~/.config/waybar/
    cp config.jsonc ~/.config/waybar/
    cp style.css ~/.config/waybar/
    ```

3. **Setup scripts:**
    
    Copy the `scripts` folder to `~/.config/waybar`:
    ```bash
    cp -r scripts ~/.config/waybar/
    ```

    Copy the scripts to `~/.local/share/bin`:
    ```bash
    mkdir -p ~/.local/share/bin
    cp scripts/* ~/.local/share/bin/
    ```

4. **Copy additional configuration files:**
    - **rofi:** Copy the files to `~/.config/rofi`:
        ```bash
        mkdir -p ~/.config/rofi
        cp -r rofi/* ~/.config/rofi/
        ```

    - **wlogout:** Copy the files to `~/.config/wlogout`:
        ```bash
        mkdir -p ~/.config/wlogout
        cp -r wlogout/* ~/.config/wlogout/
        ```

5. **Restart Waybar to apply the changes:**
    ```bash
    killall waybar
    waybar &
    ```

## Customization
You can modify the configuration files to match your setup. However, if you use alternative tools or dependencies, you'll need to adjust the scripts and configurations accordingly.

## Credits
This configuration uses base modules and scripts from prasanthrangan's [hyprdots](https://github.com/prasanthrangan/hyprdots), which served as the foundation for this setup.