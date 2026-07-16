# Build a WordPress Job Dashboard

**Recommended Expertise:** WordPress development, PHP, REST APIs, JavaScript, performance optimization, and plugin architecture

---

# Steps Overview

- Create the custom plugin.
- Connect to one API (e.g., Ashby).
- Display job listings.
- Add search and filters.
- Add company pages and job details.
- Support multiple ATS providers (Ashby, Workday, Greenhouse, Lever).
- Add user features like favorites and alerts.
- Polish it with a professional interface.

---

# Purpose

Demonstrate to WordPress / Automattic my aptitude for building in WordPress; Offer new WP job search experience to moorcoders.

---

# I. CREATE PLUGIN

## Here's what you need:

- WordPress (open source) — Free to download and develop with.
- PHP — The primary language for WordPress plugins. Free.
- A code editor — Free options include Visual Studio Code, Notepad++, or VSCodium.
- A local development environment — Free options include Local, XAMPP, Laragon (Windows), or MAMP's free version.
- A web browser for testing.

## System Requirements

(A modern local development environment typically includes):

- PHP 8.x
- MySQL or MariaDB
- Apache or Nginx
- WordPress 6.x or later

## Basic workflow:

1. Install WordPress on your computer using a local development environment.
2. Create a new folder in the `wp-content/plugins` directory.
3. Add a PHP file with a plugin header, for example:

```php
<?php
/*
 * Plugin Name: My First Plugin
 * Description: My first WordPress plugin.
 * Version: 1.0
 * Author: Your Name
 */

defined('ABSPATH') || exit;

// Your code goes here.
```

4. Go to Plugins in the WordPress admin dashboard and activate your plugin.
5. Add functionality using WordPress hooks (`add_action()` and `add_filter()`), APIs, and custom code.

---

# Steps

## Install PHP, MySQL / MariaDB, and a Web Server; Start the services:

```bash
sudo apt update
sudo apt install mysql-server
```

or

```bash
sudo apt update
sudo apt install apache2 mysql-server php libapache2-mod-php php-mysql unzip curl
```

(or `sudo apt install mariadb-server`)

```bash
sudo systemctl start apache2
sudo systemctl start mysql
```

---

# Install WP-CLI

```bash
curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
```

```bash
php wp-cli.phar --info
```

```bash
chmod +x wp-cli.phar
```

```bash
sudo mv wp-cli.phar /usr/local/bin/wp
```

## Verify:

```bash
wp --info
```

---

# Create a Project Directory

```bash
sudo mkdir /var/www/html/wordpress
sudo chown $USER:$USER /var/www/html/wordpress
cd /var/www/html/wordpress
```

---

# Download WordPress

```bash
wp core download
```

---

# Create the MySQL / MariaDB database and Generate the configuration

```bash
wp config create --dbname=wordpress --dbuser=wpuser --dbpass=wpuser
```

---

# Install WordPress

```bash
wp core install \
  --url=http://localhost/wordpress \
  --title="moorcode" \
  --admin_user=admin \
  --admin_password=wpadmin \
  --admin_email=moorcodellc@gmail.com
```

---

# II. CONNECT TO ONE API (E.G., ASHBY)

## Here's what you need:

## Basic workflow:

---

# III. DISPLAY JOB LISTINGS

## Here's what you need:

## Basic workflow:

---

# IV. ADD SEARCH AND FILTERS

## Here's what you need:

## Basic workflow:

---

# V. ADD COMPANY PAGES AND JOB DETAILS

## Here's what you need:

## Basic workflow:

---

# VI. SUPPORT MULTIPLE ATS PROVIDERS (ASHBY, WORKDAY, GREENHOUSE, LEVER)

## Here's what you need:

## Basic workflow:

---

# VII. ADD USER FEATURES LIKE FAVORITES AND ALERTS

## Here's what you need:

## Basic workflow:

---

# VIII. POLISH IT WITH A PROFESSIONAL INTERFACE

## Here's what you need:

## Basic workflow:
