# Setup Apache2 on Ubuntu

```sh
sudo apt-get remove --purge apache2 apache2-utils
sudo apt-get install --reinstall apache2 apache2-utils
sudo service apache2 start

# check apache2
sudo service apache2 status
```
