
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/iGore/ddev-gitpod-shopware6.git)

# Shopware 6 production template

This repository contains the production template that enables you to build,
package and deploy Shopware 6 to production shops.

## Installation and usage instructions

## Install ddev local
https://ddev.readthedocs.io/en/latest/

git clone https://github.com/lme-adesso/ddev-gitpod-shopware6.git

# Commands after cloning:

1. ddev start -y
2. ddev composer install
3. in .env URL anpassen auf: APP_URL="https://radeberger.adesso.localhost"
4. ddev exec bin/console system:setup --database-url=mysql://db:db@db:3306/db --app-url='https://raderberger.adesso.localhost'
5. ddev exec bin/console system:install --create-database --basic-setup --force
6. ddev php bin/console cache:clear
7. ddev ssh 
8. mkdir custom/plugins

# Go to:
http://adesso-shopware.local

# Switch to docker container:

ddev ssh

# Use bin/console:

ddev php bin/console

## GitPod

Please refer to the
[documentation](https://developer.shopware.com/docs/guides/installation/template)
for instructions on how to use this template.


## Prerequisites:
1. [Sign up for gitpod.io](https://gitpod.io/login)

## Try it out:
1. Click on the following link
  https://gitpod.io/#https://github.com/iGore/ddev-gitpod-shopware6.git
1. Your environment is being prepared, wait about 40 seconds (A splash screen will appear)
2. `ddev launch /admin`to open login
3. The default credentials are username `admin` and password `shopware`.
4. :tada:

# Inspired by
* https://github.com/shaal/ddev-gitpod/tree/main
* https://github.com/codeblick/gitpod-shopware-6


# Based on
* https://github.com/shopware/production
