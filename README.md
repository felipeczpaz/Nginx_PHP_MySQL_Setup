# Nginx PHP MySQL Setup

This script automates the setup of an Nginx web server with PHP and MySQL on a Debian-based system.

## Prerequisites
- A Debian-based Linux distribution (tested on Ubuntu)
- Bash shell

## Usage
1. Open a terminal.
2. Clone this repository or download the script.
3. Make the script executable:
    ```bash
    chmod +x setup_nginx_php_mysql.sh
    ```
4. Run the script:
    ```bash
    ./setup_nginx_php_mysql.sh
    ```

## What does this script do?
- Updates package lists
- Upgrades installed packages
- Performs distribution upgrade
- Installs Nginx, MySQL Server, PHP-FPM, and PHP MySQL extension
- Secures MySQL installation
- Creates a directory for the specified domain and sets ownership
- Determines PHP version and sets fastcgi_pass dynamically
- Creates Nginx server block configuration file for the specified domain
- Creates a symbolic link to enable the site
- Checks Nginx configuration
- Restarts Nginx

## Customization
Before running the script, ensure to customize the following variables according to your setup:
- `MYSQL_ROOT_PASSWORD`: Define your MySQL root password.
- `YOUR_DOMAIN`: Define your domain.

## Disclaimer
This script is provided as-is, use at your own risk. It is recommended to review and understand the script before executing it, especially if you're deploying it on a production system.

## License
This project is licensed under the [MIT License](LICENSE).
