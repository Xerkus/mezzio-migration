# Changelog

All notable changes to this project will be documented in this file, in reverse chronological order by release.

## 0.1.5 - TBD

### Added

- Nothing.

### Changed

- Nothing.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- Nothing.

## 0.1.4 - 2019-11-22

### Added

- [zendframework/zend-expressive-migration#18](https://github.com/zendframework/zend-expressive-migration/pull/18) adds compatibility with symfony/console ^5.0.

### Changed

- Nothing.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- [zendframework/zend-expressive-migration#17](https://github.com/zendframework/zend-expressive-migration/pull/17) fixes saving composer.json contents.
  In some edge cases we saved invalid composer.json content with empty `[]` instead of `{}` for some sections.
  Now we are dropping empty sections.

## 0.1.3 - 2018-03-20

### Added

- Nothing.

### Changed

- Nothing.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- [zendframework/zend-expressive-migration#10](https://github.com/zendframework/zend-expressive-migration/pull/10)
  fixes a scenario whereby the RC4 skeleton would be selected over the stable
  one as the basis for the bootstrap files.

- [zendframework/zend-expressive-migration#12](https://github.com/zendframework/zend-expressive-migration/pull/12)
  modifies how laminas-diactoros is added to the root package. Instead of an
  additional `composer require` statement fired early, it is added to the
  package requirements, and the package requirements are now installed before any
  development requirements to ensure the PSR-7 implementation is discovered.

## 0.1.2 - 2018-03-15

### Added

- Nothing.

### Changed

- Nothing.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- Fixes an issue that occurs when running in an application that does not
  require laminas-diactoros in the package root. The tool now explicitly requires it
  before doing any other migrations.

- Adds a default directory in which to convert middleware to request handlers.

- Adds logic to remove the tool package itself during migration, ensuring it is
  not present in the final artifacts.

## 0.1.1 - 2018-03-15

### Added

- Nothing.

### Changed

- [zendframework/zend-expressive-migration#3](https://github.com/zendframework/zend-expressive-migration/pull/3)
  updates the list of expected versions in the README to reflect released
  versions.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- [zendframework/zend-expressive-migration#4](https://github.com/zendframework/zend-expressive-migration/pull/4)
  fixes some Windows compatibility problems.

- [zendframework/zend-expressive-migration#5](https://github.com/zendframework/zend-expressive-migration/pull/5)
  fixes some minor issues in detecting the latest version of the skeleton, as
  well as retrieving content from the skeleton.

- [zendframework/zend-expressive-migration#5](https://github.com/zendframework/zend-expressive-migration/pull/5)
  updates the tool to remove any "minimum-stability" settings in the
  `composer.json`.

## 0.1.0 - 2018-03-14

Initial functionality for migrating to version 3.

### Added

- Nothing.

### Changed

- Nothing.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- Nothing.
