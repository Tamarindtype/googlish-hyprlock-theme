<div align="center">
    <h1>✦ Google-ish Hyprlock Theme ✦</h1>
    <h3></h3>
</div>

## ▶️ Preview
<details>
	<summary><b>Without Profile & User Info</b></summary>
	<img src="https://github.com/user-attachments/assets/7bbacd47-b0d7-4132-9951-53dc0ead604c" alt="Hyprlock-Without-Profile" width="1280">
</details>
<details>
	<summary><b>With Profile & User Info</b></summary>
	<img src="https://github.com/user-attachments/assets/9a58a6e2-a71f-4b28-998a-8a45c8950aaf" alt="Hyprlock-With-Profile" width="1280">
</details>
<details>
	<summary><b>With Profile & User Info [12H Format]</b></summary>
	<img src="https://github.com/user-attachments/assets/e0049860-7511-432e-8814-8d17d448182b" alt="Hyprlock-With-Profile" width="1280">
</details>

## 📦 Installation
><i><b>❗ This configuration is based on a 1080p display, if you are using a higher screen resolution,</br>you may need to reconfigure the sizes and recoordinate all the components.</b></i>

<b>Auto-Installation :</b>
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/Tamarindtype/googlish-hyprlock-theme/main/install.sh)"
```
</br><b>Manual Installation :</b>
```bash
# Backup your current Hyprlock config first!
# Clone the repository
git clone https://github.com/Tamarindtype/googlish-hyprlock-theme.git

# Move all the files to the hyprland config folder
mv ./googlish-hyprlock-theme/* ~/.config/hypr/

# Go to script folder
cd $HOME/.config/hypr/hyprlock/

# Change all the scripts permission to make them executable
chmod +x *.sh

# Run the Hyprlock
hyprlock
```

## 🗄️ Directory Structure
```md
$HOME
└── .config
    └── hypr
        ├── hyprlock
        │  ├── assets
        │  ├── battery.sh
        │  ├── bluetooth.sh
        │  ├── change_wallpaper.sh
        │  ├── greeting.sh
        │  ├── network.sh
        │  ├── medianotif.sh
        │  └── weatherinfo.sh
        └── hyprlock.conf
```

## 🗨️ FAQ
| Question | Answer |
| --- | --- |
| Profile & User info does not appear? | By default, it set without profile and user info. You can enable it by uncomment the `image` @PROFILE PICTURE and `label` @USER INFO in `hyprlock.conf` |
| Battery percentage number does not appear? | Change your battery module in `battery.sh`. The default is `BAT0`, you can check it by running this command `ls /sys/class/power_supply/` |
| How to change the 24H Format to 12H Format? | Comment the 24H format and uncomment the 12H format. also uncomment the AM/PM `label` & `shape` in `hyprlock.conf` |
| null location or Unable to determine your location? | Change the IP Geolocation provider in `weatherinfo.sh` |

## 🏅 Recommendations
| Type | Name | Links |
| --- | --- | --- |
| Regular | PP Neue Machina | [Pangram Pangram](https://pangrampangram.com/products/neue-machina) |
| Nerd Font | Geist & Space Mono | [Nerd Fonts](https://github.com/ryanoasis/nerd-fonts/releases) |
| Emoji | Apple Emoji | [apple-emoji-linux](https://github.com/samuelngs/apple-emoji-linux) |

## ✨ Special Thanks & Credits

| Details | Credit |
| --- | --- |
| Battery & Playerctl Widget Scripts | @ashish-kus [minimal Hyprlock](https://gist.github.com/ashish-kus/dd562b0bf5e8488a09e0b9c289f4574c) |
| Helped Me Create Dynamic WiFi, Bluetooth, Weathercast and Greeting Widget | @OPENAI [ChatGPT](https://chatgpt.com/)|