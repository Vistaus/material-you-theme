# Material You Color Theming
Applies generated libadwaita theme from wallpaper using Material You

![extension-screenshot](https://i.imgur.com/VLXfoEa_d.webp?maxwidth=2160&shape=thumb&fidelity=high)

<div align="center">
  <a href="https://extensions.gnome.org/extension/5236/material-you-color-theming/">
    <img src="https://img.shields.io/badge/Install%20from-extensions.gnome.org-4A86CF?style=for-the-badge&logo=Gnome&logoColor=white"/>
  </a>  
</div>

## Installation
Copy the extension to your extensions folder (create the folder if it does not exist).
```
git clone https://github.com/avanishsubbiah/material-you-theme
cd material-you-theme
make && make install
```
Log out and log back in and you should be able to enable it in your extension manager.

NOTE: Using the extension now will theme your native installed libadwaita apps, follow the steps below to have the theme apply to GTK3 and flatpak apps.

### Libadwaita
#### Native
Theming for native libadwaita will work by default.
#### Flatpak
Install [Flatseal](https://github.com/tchx84/Flatseal), and add `xdg-config/gtk-4.0:ro` to **Other Files** under the category **Filesystem** in the **All Applications** section.

### GTK3
#### Native
Install the [adw-gtk3](https://github.com/lassekongo83/adw-gtk3) theme and apply it.
#### Flatpak
After installing the [adw-gtk3](https://github.com/lassekongo83/adw-gtk3) add `xdg-config/gtk-3.0:ro` to **Other Files** under the category **Filesystem** in the **All Applications** section using [Flatseal](https://github.com/tchx84/Flatseal).

## Usage
Once the extension is enabled the extension will update your theme based on your current wallpaper and system dark mode preference. When you change your system dark mode preference or wallpaper the extension will automatically refresh your theme.

## Uninstall
Disabling the extension in your extension manager will undo theme changes back to default.
