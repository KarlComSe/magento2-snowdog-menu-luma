# Luma support for Snowdog Menu for Magento 2

[![Packagist](https://img.shields.io/packagist/v/vseager/magento2-snowdog-menu-luma?style=for-the-badge)](https://packagist.org/packages/vseager/magento2-snowdog-menu-luma)
[![Packagist](https://img.shields.io/packagist/dt/vseager/magento2-snowdog-menu-luma?style=for-the-badge)](https://packagist.org/packages/vseager/magento2-snowdog-menu-luma)
[![Packagist](https://img.shields.io/packagist/dm/vseager/magento2-snowdog-menu-luma?style=for-the-badge)](https://packagist.org/packages/vseager/magento2-snowdog-menu-luma)


Seamlessly integrate the popular Snowdog Menu for Magento 2 with the Luma theme templates. No custom templates or CSS required. Just install, create a menu with the identifier `main`, populate and enjoy!

Supports the following node types:

* Category
* Product
* CMS Page Link
* Custom URL
* Category Child

## Installation

```
composer require vseager/magento2-snowdog-menu-luma
```

## Usage

Just install and use add a Menu node with the ID `main`.

You can use the "Node CSS classes" field on the menu nodes to apply custom classes to the frontend if you wish to use them for styling.

## ⚠️ Important: Not Compatible with Magento Full Page Cache (FPC)

This module replaces the `catalog.topnav` block with the Snowdog Menu using a plugin.

However, **this does not work when Full Page Cache (FPC) is enabled** which is the default in Magento production mode. Cached pages bypass the plugin, and the menu will not appear or update.
