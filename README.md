<p align="center">
  <img width="325" alt="logo2" src="https://github.com/user-attachments/assets/7bd9520b-6917-4d53-8b66-be3de15d42a8" />
</p>

---
<br>

This is a theme made for the Pterodactyl game server management panel.\
**Note: This theme was last tested on Pterodactyl v2.0.0-beta.2**

If you have any issues, contact me on discord: https://discord.gg/sYGhc48k6P

<img width="957" height="448" alt="image" src="https://github.com/user-attachments/assets/2790bcbb-330e-4f8f-8b5b-1894e46b8777" />

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

## Images

<details>
  <summary>View Screenshots</summary>
<img width="1915" height="896" alt="image" src="https://github.com/user-attachments/assets/2790bcbb-330e-4f8f-8b5b-1894e46b8777" />

<img width="1918" height="911" alt="image" src="https://github.com/user-attachments/assets/fb899e6f-aeb1-4062-b15c-7ae732edc800" />

<img width="1910" height="904" alt="image" src="https://github.com/user-attachments/assets/87d5d4de-7d65-4a1f-b67e-1a578f1b2414" />
</details>

