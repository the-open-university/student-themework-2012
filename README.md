# student-themework-2012

## Overview
This package contains the current [Student Theme](http://www2.open.ac.uk/students/style-guide) and aims to help us build an efficient workflow for bridging theme design and theme implementation.

## Usage
All of the theme files should be put inside the 'public' folder of this package. Inside this folder you may create whatever folder structure you wish.

This package also contains a Laravel Service Provider, which will register the public directory of this package with CodeSleeve/asset-pipeline. This allows us to simply reference the theme files in the manifest file using local paths.

## Installation
To install this package into a Laravel App using CodeSleeve/asset-pipeline:

1. Install this package using Composer

2. Add `OU\ThemeStudent2012\ThemeStudent2012ServiceProvider` to your `app/config/app.php` file

3. Run `composer dump-autoload`

4. Run `php artisan dump-autoload`

5. Run `php artisan asset:publish "ou/theme-student2012"` to publish all of the assets to the `public/packages/ou/theme-student2012` directory of your app (you will need to do this everytime you pull a new commit)

6. Add references to the CSS and JS files into your manifest files e.g. //= require styles
