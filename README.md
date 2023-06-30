
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/iGore/ddev-gitpod-shopware6.git)

# Shopware 6 production template

This repository contains the production template that enables you to build,
package and deploy Shopware 6 to production shops.

## Installation and usage instructions

## Install ddev local
https://ddev.readthedocs.io/en/latest/

git clone https://github.com/lme-adesso/ddev-gitpod-shopware6.git

# Commands after cloning:

ddev start -y
ddev composer install
ddev exec bin/console system:setup --database-url=mysql://db:db@db:3306/db --app-url='${DDEV_PRIMARY_URL}'
ddev exec bin/console system:install --create-database --basic-setup

# Go to:
http://adesso-shopware.ddev.site

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
