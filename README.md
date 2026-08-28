## Installation

```
flatpak install flathub page.codeberg.stilic.Soda
```

## Running

```
flatpak run page.codeberg.stilic.Soda
```

## MangoHud installation

```
flatpak install org.freedesktop.Platform.VulkanLayer.MangoHud/x86_64/25.08
```

## Important permissions

```
# Allow Soda Launcher to detect Steam users and games
sudo flatpak override page.codeberg.stilic.Soda --filesystem=~/.var/app/com.valvesoftware.Steam/
sudo flatpak override page.codeberg.stilic.Soda --talk-name=org.freedesktop.Flatpak

# Allow Steam to run Soda Launcher shortcuts
sudo flatpak override com.valvesoftware.Steam --talk-name=org.freedesktop.Flatpak

# Allow Steam to see Soda Launcher games icons
sudo flatpak override com.valvesoftware.Steam --filesystem=~/.var/app/page.codeberg.stilic.Soda/config/soda-launcher/
sudo flatpak override com.valvesoftware.Steam --filesystem=~/.config/soda-launcher/
```

### Known issues

- The 'stop' button won't close games/apps
- Gamescope doesn't work
- It may not use the system theme in some DEs
