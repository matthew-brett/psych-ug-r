*   [Install Linux on ChromeOS](https://chromeos.dev/en/linux/setup)
*   Follow instructions on [this StackOverflow
    answer](https://stackoverflow.com/a/49620964/1939576) (but see my comment
    at the end of that answer).  See the appendix below for full list of the
    commands we used.
*   Run command `rstudio` from the terminal.  Wait.

Thanks to Eleanor Woolley for help testing this procedure.

## More notes

*   [Getting files out of zip
    archives](https://www.howtogeek.com/409680/how-to-zip-or-unzip-files-on-a-chromebook)
*   [Finding your ChromeOS files from Linux
    / RStudio](https://superuser.com/a/1506916/1321158).  We actually did:

    ```
    cd
    ln -s /mnt/chromeos/MyFiles
    ```

    in order to make it easy to find the shared files from the home directory
    in Linux.

## Appendix: commands we used to install RStudio

These come from the StackOverflow post above, with a couple of tweaks.

Start the Linux terminal.  Copy/paste the following:

```
# Update, cleanup package listings and installs.
sudo apt-get update
sudo apt-get upgrade
sudo apt-get update --fix-missing
sudo apt autoclean
sudo apt clean
sudo apt-get autoremove
# Package to store keys identifying new repositories.
sudo apt install -y gnupg2
# Confirm identity of RStudio package listings.
sudo apt-key adv --keyserver keys.gnupg.net --recv-key 'E19F5F87128899B192B1A2C2AD5F960A256A04AF'
# Add the RStudio package listings to the config file.
sudo echo "deb http://cran.rstudio.com/bin/linux/debian buster-cran35/" >> /etc/apt/sources.list
# Update the list of packages.
sudo apt update
# Clipboard package.
sudo apt-get install -y xclip
# Install R itself.
sudo apt install -y r-base r-base-dev
# Other stuff RStudio likes.
sudo apt-get install -y gdebi-core
sudo apt install -y libgstreamer1.0 libgstreamer-plugins-base1.0 libxslt-dev libnss3
# A new dependency that seems to be needed.
sudo apt install -y libclang-dev
sudo apt --fix-broken install
# Download, install RStudio itself.
sudo curl -o rstudio.deb https://download1.rstudio.org/desktop/bionic/amd64/rstudio-1.2.5033-amd64.deb
sudo dpkg -i rstudio.deb
# Cleanup package listings and installs again.
sudo apt-get update
sudo apt-get upgrade
sudo apt --fix-broken install
sudo apt-get update --fix-missing
sudo apt autoclean
sudo apt-get clean
sudo apt-get autoremove
```
