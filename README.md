<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# Kanboard for YunoHost

[![Integration level](https://dash.yunohost.org/integration/kanboard.svg)](https://dash.yunohost.org/appci/app/kanboard) ![](https://ci-apps.yunohost.org/ci/badges/kanboard.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/kanboard.maintain.svg)  
[![Install Kanboard with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=kanboard)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install Kanboard quickly and simply on a YunoHost server.
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview

Kanban project management software

**Shipped version:** 1.2.21~ynh2

**Demo:** https://demo.yunohost.org/kanboard/

## Screenshots

![](./doc/screenshots/board.png)

## Disclaimers / important information

## Limitations

## Additional information

### How to connect as external (non-SSOwat) users

You have to edit this file `/var/www/kanboard/config.php`, find the line `define('REVERSE_PROXY_AUTH', true);` and change it from `true` to `false`.
**Warning** this disables the possibility to connect with SSOwat users. You will *only* be able to connect with Kanboard users created inside of Kanboard.
Then you can connect.

**NB**: if you don't make that change, you will get the following error message "Access Forbidden".

This is due to a Kanboard limitation.

## Documentation and resources

* Official app website: https://kanboard.net
* Official admin documentation: https://docs.kanboard.org/en/latest/
* Upstream app code repository: https://github.com/kanboard/kanboard
* YunoHost documentation for this app: https://yunohost.org/app_kanboard
* Report a bug: https://github.com/YunoHost-Apps/kanboard_ynh/issues

## Developer info

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/kanboard_ynh/tree/testing).

To try the testing branch, please proceed like that.
```
sudo yunohost app install https://github.com/YunoHost-Apps/kanboard_ynh/tree/testing --debug
or
sudo yunohost app upgrade kanboard -u https://github.com/YunoHost-Apps/kanboard_ynh/tree/testing --debug
```

**More info regarding app packaging:** https://yunohost.org/packaging_apps