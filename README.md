<p align="center">
  <img width="325" alt="logo2" src="https://github.com/user-attachments/assets/7bd9520b-6917-4d53-8b66-be3de15d42a8" />
</p>

---
<br>

This is a theme made for the Pterodactyl game server management panel.\
**Note: This theme was last tested on Pterodactyl v2.0.0-beta.2**

If you have any issues, contact me on discord: https://discord.gg/sYGhc48k6P

<br>

## Instructions

<details>
<summary>Installing/Updating the theme</summary>

## Installation

Requirements: Pterodactyl Panel 2.0

### Download the theme
The first step is to download the theme. The command below saves the latest release as a zip file in the temporary folder.
If the URL does not work, you can manually download the zip file from the releases tab
```
cd /var/www/pterodactyl
wget -O /tmp/galaxy.zip https://github.com/32dev/GalaxyTheme/releases/latest/download/galaxy-theme.zip
```

### Install the extension

Next you need to install Galaxy as a panel extension.
If you already have the theme installed, add --replace to update it to the newest version
```
php artisan p:extension:install /tmp/galaxy.zip --enable
```

### Remove the temporary file
You can now get rid of the zip file you downloaded
```
rm /tmp/galaxy.zip
```


### Activate the theme
If you want all of your panel's users to use the Galaxy theme, run the command below.
Otherwise, you may skip this step and find the theme under the 'Themes' section of your admin panel
```
php artisan p:theme:activate galaxy
``` 

</details>

<details>
<summary>Uninstalling the Theme </summary>

## Uninstalling the theme

### Switching to the default theme
The panel will not you remove a theme that is active, so you need to switch all users back to the default first.
```
cd /var/www/pterodactyl
php artisan p:theme:reset
```

### Remove the extension
This deletes Galaxy from your panel.

```
php artisan p:extension:remove galaxy
```

</details>
