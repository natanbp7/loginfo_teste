# loginfo_teste
Teste de aptidão Loginfo
Compse Bootstrap Version [3.x/2.x]

## Installation
cd to the root of your app folder (where the composer.json file is) and run the following Composer command:

composer require friendsofcake/bootstrap-ui
Then load the plugin using CakePHP's console:

bin/cake plugin load BootstrapUI
## Setup
You can either use the Bootstrap commands to make the necessary changes, or do them manually.

Using the Bootstrap commands
To install the Bootstrap assets (Bootstrap's CSS/JS files, jQuery and Popper.js) via npm you can use the install command, or install them manually:

bin/cake bootstrap install
This will fetch all assets, copy the distribution assets to the BootstrapUI plugin's webroot directory, and symlink (or copy) them to your application's webroot directory.

You will need to modify your src/View/AppView class to either extend BootstrapUI\View\UIView or use the trait BootStrapUI\View\UIViewTrait. For doing this you can either use the modify_view command, or change your view manually:

bin/cake bootstrap modify_view
This will rewrite your src/View/AppView like described in AppView setup using UIView.

BootstrapUI ships with some example layouts. You can install them using the copy_layouts command, or copy them manually:

bin/cake bootstrap copy_layouts
This will copy the three example layouts cover.php, dashboard.php and signin.php to your application's src/templates/layout/TwitterBootstrap.


## Migrations
use Migrations\AbstractMigration;

class CategoriasProdutos extends AbstractMigration
{
    /**
     * Change Method.
     *
     * More information on this method is available here:
     * https://book.cakephp.org/phinx/0/en/migrations.html#the-change-method
     * @return void
     */
    public function change()
    {
    }
}
class Vendas extends AbstractMigration
{
    /**
     * Change Method.
     *
     * More information on this method is available here:
     * https://book.cakephp.org/phinx/0/en/migrations.html#the-change-method
     * @return void
     */
    public function change()


# CakePHP Application Skeleton





[![Build Status](https://img.shields.io/travis/cakephp/app/master.svg?style=flat-square)](https://travis-ci.org/cakephp/app)
[![Total Downloads](https://img.shields.io/packagist/dt/cakephp/app.svg?style=flat-square)](https://packagist.org/packages/cakephp/app)

A skeleton for creating applications with [CakePHP](https://cakephp.org) 3.x.

The framework source code can be found here: [cakephp/cakephp](https://github.com/cakephp/cakephp).
## Installation

1. Download [Composer](https://getcomposer.org/doc/00-intro.md) or update `composer self-update`.
2. Run `php composer.phar create-project --prefer-dist cakephp/app [app_name]`.

If Composer is installed globally, run

```bash
composer create-project --prefer-dist "cakephp/app:^3.8"
```

In case you want to use a custom app dir name (e.g. `/myapp/`):

```bash
composer create-project --prefer-dist "cakephp/app:^3.8" myapp
```

You can now either use your machine's webserver to view the default home page, or start
up the built-in webserver with:

```bash
bin/cake server -p 8765
```

Then visit `http://localhost:8765` to see the welcome page.

## Update

Since this skeleton is a starting point for your application and various files
would have been modified as per your needs, there isn't a way to provide
automated upgrades, so you have to do any updates manually.

## Configuration

Read and edit `config/app.php` and setup the `'Datasources'` and any other
configuration relevant for your application.

## Layout

The app skeleton uses a subset of [Foundation](http://foundation.zurb.com/) (v5) CSS
framework by default. You can, however, replace it with any other library or
custom styles.
