# Linux Virtual hosts
#####How To Set Up Apache Virtual Hosts on Debian 8.6

###Step 1: Create new Virtual host file
Start by copying the file `virtual.conf` to folder `/etc/apache2/sites-available/` for new domain.

Next, changing file's name. ( There, i use name: `virtual` )

After, changing the `ServerName`, `ServerAdmin`, `DocumentRoot`

###Step 2: Enable the new Virtual hosts files by following command line:

`a2ensite virtual.conf`

###Step 3: Restart Apache by foolowing command line:

`service apache2 restart`

###Step 4: Set up Local hosts file

Open `hosts` file: `nano /etc/hosts`

Add new VPS IP to the the bottom of this file ( like localhost )
