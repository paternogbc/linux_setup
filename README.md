# Commands setup Linux (ubuntu or deb-based distros)

## Update system

```
sudo apt update 
sudo apt upgrade
```

## Basic configuration

Enable minimize icons on docs
```
gsettings set org.gnome.shell.extensions.dash-to-dock click-action minimize
```

# Midia codecs
```
sudo apt install ubuntu-restricted-extras
```

# Synapt and cmake
```
sudo apt-get install synaptic cmake 
```

# Install albert

Follow instruxctions [here](https://software.opensuse.org/download.html?project=home:manuelschneid3r&package=albert)


## Install (R)
Add public key

```
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys E298A3A825C0D65DFD57CBB651716619E084DAB9
```

```
sudo apt install r-base r-base-dev
```

## Linux libs for data Science (R tidyverse)
```
sudo apt install libcurl4-openssl-dev libmagick++-dev libxml2-dev libssl-dev libgmp3-dev libglpk-dev
```

## Install essential r-packages
```
R -e 'install.packages(c("tidyverse", "blogdown", "bookdown", "sensiPhy"))'
```
## Generate public key for Github

```
ssh-keygen -t rsa -b 4096 -C "paternogbc@gmail.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
```

## Add public key to Github
```
sudo apt-get install xclip
xclip -sel clip < ~/.ssh/id_rsa.pub
```
