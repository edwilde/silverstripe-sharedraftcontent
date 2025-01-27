# Share Draft Content

[![CI](https://github.com/silverstripe/silverstripe-sharedraftcontent/actions/workflows/ci.yml/badge.svg)](https://github.com/silverstripe/silverstripe-sharedraftcontent/actions/workflows/ci.yml)
[![Silverstripe supported module](https://img.shields.io/badge/silverstripe-supported-0071C4.svg)](https://www.silverstripe.org/software/addons/silverstripe-commercially-supported-module-list/)

Share draft page content with non-CMS users.

## Overview

This module adds a 'Share draft' action menu to the CMS. This enables Content Authors to generate tokenised links to draft pages. Content authors can share these links with anyone, allowing non-CMS user to view draft page content. Each preview link is valid for 30 days.

## Requirements

- Silverstripe ^4.4

Note: this version is compatible with Silverstripe 4. For Silverstripe 3, please see the 1.x release line. Previous 2.x
releases exist for earlier Silverstripe 4.x versions.

## Installation

The easiest way to install is by using [Composer](https://getcomposer.org):

```sh
$ composer require silverstripe/sharedraftcontent
```

You'll also need to run `dev/build`. You should now see a link/button on the bottom-right of edit pages. Clicking the link will generate a new share link.

# Developer Tools

Get the dependencies by running `npm install`.

After making changes to SCSS files, run the build script `npm run build`. This will compile everything for you and output minified CSS files to the `css` directory.

## Share Links

The generated share links have a public key and hash. There can be any number of share links per-page, but all share links are unique, and cannot be used to gain access to pages other than the one each link was created for.

## Versioning

This library follows [Semver](http://semver.org). According to Semver, you will be able to upgrade to any minor or patch version of this library without any breaking changes to the public API. Semver also requires that we clearly define the public API for this library.

All methods, with `public` visibility, are part of the public API. All other methods are not part of the public API. Where possible, we'll try to keep `protected` methods backwards-compatible in minor/patch versions, but if you're overriding methods then please test your work before upgrading.

## Reporting Issues

Please [create an issue](http://github.com/silverstripe/silverstripe-sharedraftcontent/issues) for any bugs you've found, or features you're missing.
