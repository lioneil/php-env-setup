Lamp Server Installation:
  ```bash
  sudo apt-get update & sudo apt-get upgrade
  sudo apt-get install lamp-server^
  sudo mysql_secure_installation
  // Use this answers
  > Validate? no
  > New Password: root
  > Re-enter Password: root
  > Remove anonymous users: y
  > Disallow remote login: y
  > Remove test database: y
  > Reload privileges: y
  # When accessing mysql via terminal, use sudo
  sudo mysql -uroot -p
  > password: root
  ```

  ```bash
  sudo apt-get install phpmyadmin
  > select `apache`, if prompted
  ```

  Restart Services:
  ```bash
  sudo service apache2 restart
  sudo service mysql restart
  ```

  Add Virtual Hosts:
  ```bash
  mkdir ~/Projects
  # Backup the default 'html' folder
  sudo mv /var/www/html /var/www/html.bak
  sudo ln -s ~/Projects /var/www/html
  ```
  If all goes well, remove the `html.bak` folder.

  Install NodeJS
  ```
  sudo apt install nodejs
  sudo apt install npm
  ```

  Install Composer
  ```
  https://getcomposer.org/download/
  ```


OS Misc:
  - Go to Ubuntu Settings > Keyboard Shortcuts and Set "Home folder" shortcut to "SUPER+E"

Bash Terminal Setup:
  - Download [.bashrc](./.bashrc)

Apps:
  Dropbox
  Sublime Text 3
    `ln -s ~/Dropbox/path/to/Backup/Sublime/Packages/User ~/.config/sublime-text-3/Packages/User`
  Atom Editor
