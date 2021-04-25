# PteroThemes 🎨
 Themes for Pterodactyl v1.x

## Automatic Installation
Install them manually, or use this (outdated) script to install them automatically:
https://github.com/WeLikeToCodeStuff/ptero-1.0-theme-install

# Manual Installation
Follow this guide to manually install themes:

## User Panel
Create a file called main.css in `/var/www/pterodactyl/resources/scripts`

In that file put this text

```@import url(https://oreokitten.github.io/latest/dark-n-purple/user.css);```

After that edit the file **index.tsx** in /var/www/pterodactyl/resources/scripts

On line 6 at the end of the imports add this

```import './main.css';```
After this build the panel, you can find information of how to do that scroll down

After building just reload your panel and the theme is applied.

# Admin Panel
In the file admin.blade.php in `/var/www/pterodactyl/resources/views/layouts/`

On line 36 put the text
```<link rel="stylesheet" href="https://oreokitten.github.io/latest/dark-n-purple/admin.css">```

After this build the panel, you can find information of how to do that scroll down

After building just reload your panel and the theme is applied.

## How to build panel?
# Install Dependencies
The following commands will install the necessary dependencies for building your panel.

# Install NodeJS
TIP

You may have to add sudo to the following commands if you are not root.

# Using Nodesource
# Ubuntu/Debian
`curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -`

`apt install -y nodejs`

# CentOS
`curl -sL https://rpm.nodesource.com/setup_12.x | sudo -E bash -`
`yum install -y nodejs # CentOS 7`
`dnf install -y nodejs # CentOS 8`
By now, you should have NodeJS 12 installed. Make sure this is the case by checking node -v

# Using Node Version Manager(opens new window)
`curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/master/install.sh | bash`

`nvm install node`

`nvm alias default node`

`nvm use node`

`node -v` should say 12.20.0 or newer

# Install Yarn and Panel Dependencies
# Install yarn
`npm i -g yarn`

# Speed up the proccess (Optional)
You can run this command to speed up the proccess. If you choose to use it, this is your last step!
`cd /var/www/pterodactyl && yarn install && yarn add @emotion/react && /var/www/pterodactyl`

# If you didn't use command above, continue:
`cd /var/www/pterodactyl`

# Installs panel build dependencies
`yarn install`
`yarn add @emotion/react`

#Build Panel
Run this in your panel directory to apply changes (usually` /var/www/pterodactyl`)

# Build panel
yarn build:production

## Enola
Instructions to install the theme Enola are here
[Enola (Latest Panel Version)](https://github.com/OreoKitten/PteroThemes/tree/main/latest/Enola)
![Preview](./preview/enola.png)


## Twilight
Instructions to install the theme Twilight are here
[Enola (Latest Panel Version)](https://github.com/OreoKitten/PteroThemes/tree/main/latest/Twilight)
![Preview](./preview/twilight.png)

## Recolor
This theme is a recolor of the panel that you can edit, more information here
[Recolor](https://github.com/OreoKitten/PteroThemes/tree/main/latest/Recolor)

## Dark-n-Purple
This theme is a recolor of the panel that you can edit, more information here
[Darn-n-Purple (Latest Panel Version)](https://github.com/OreoKitten/PteroThemes/tree/main/latest/Dark-n-Purple)
![Preview](./preview/Dracula.png)
![Preview](./preview/Dracula2.png)

