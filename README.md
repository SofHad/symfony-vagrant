Environment Information
========================

## IP

    Vagrant box:   33.33.33.10
    Remote XDebug: 33.33.33.1

## Database

    Name: vagrant
    User: root
    Pass: root


Installed Components
========================

 - Apache2
 - Compass
 - Composer
 - Less
 - Git
 - Memcached
 - MySQL
 - NodeJS
 - PHP
 - Ruby
 - SASS
 - SQLite
 - XDebug


Symfony2
========================

1) Installing
----------------------------------

Ensure you have the following tools installed on your computer:

 - Vagrant (http://vagrantup.com)
 - VirtualBox (http://www.virtualbox.com)
 - PHP (http://www.php.net)
 - GIT (http://git-scm.com)
 - Composer (http://getcomposer.org)

 1. Clone this repo and the vagrant submodule:

        git clone --recursive git://github.com/simshaun/symfony-vagrant.git

 2. Install Symfony in the root of the symfony-vagrant repo.
    Follow the installation instructions on http://symfony.com/download

 3. `cd` to the **vagrant** folder.

 4. Run `vagrant up`. This may take a few minutes.


2) Post-Install
----------------------------------

Symfony restricts access to **app_dev.php** and **config.php** by default.

If you need to use either of these files:

 1. Open each file in a text editor.

 2. At the top of the file, add the *Vagrant box IP* (default: 33.33.33.10) to the
    array of allowed REMOTE_ADDR.
