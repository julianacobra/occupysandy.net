occupysandy.net
===============

Standalone site for Occupy Sandy

# Install Guide

Let's install this sucker!

## Clone the Repo

From the server location you wish to use clone this repository via the command line.

`$ git clone git://github.com/occupynet/occupysandy.net.git .`

Notice the trailing period, this asks git to clone the repo into the current directroy.

## Configure `wp-config.php`

From the installed folder move or copy `wp-config-sample.php` to `wp-config.php`

I moved it then opened it in my perfered command line editor, like so:

``` bash
$ mv wp-config-sample.php wp-config.php
$ vim wp-config.php
```

More detailed info about the [wp-config file](http://codex.wordpress.org/Editing_wp-config.php) via the WordPress Codex.

## Create and add your MySQL database info

If you are unsure about setting up a MySQL database and user please check out [WordPress.org's Install Guide](http://codex.wordpress.org/Installing_WordPress#Step_2:_Create_the_Database_and_a_User)

Now find the following section of the `wp-config.php` file:

``` php
// ** MySQL settings - You can get this info from your web host ** //
/** The name of the database for WordPress */
define('DB_NAME', 'database_name_here');

/** MySQL database username */
define('DB_USER', 'username_here');

/** MySQL database password */
define('DB_PASSWORD', 'password_here');

/** MySQL hostname */
define('DB_HOST', 'localhost');
```

Input the database name, user name, and user password where asked. Your hostname is almost always going to be localhost, unless you know, don't change it.

Wow, great work so far. Before you close the file be sure to go to the `Authentication Unique Keys and Salts.` section of the config and fill those things in. Not doing so is less than good.

## Complete Database install

Now visit the URL where you've installed the wordpress. You should be presented with the welcome install page. If not, try and navigate to `yousite.com/wp-admin/install.php`. Otherwise you should [review the WordPress.org install instructions](http://codex.wordpress.org/Installing_WordPress)

Finish the install and then login.

## Configure the Theme

(more to come...)

