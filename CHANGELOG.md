# Changelog

All notable changes to this project will be documented in this file, in reverse chronological order by release.

## 2.8.0 - TBD

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

## 2.7.0 - 2019-05-14

### Added

- [zendframework/zend-authentication#44](https://github.com/zendframework/zend-authentication/pull/44) adds support for PHP 7.3.
- [zendframework/zend-authentication#47](https://github.com/zendframework/zend-authentication/pull/47) adds
  configuration option to `Laminas\Authentication\Validator\Authentication` for
  mapping custom authentication result codes to existing and new validation
  message types.

### Changed

- [zendframework/zend-authentication#42](https://github.com/zendframework/zend-authentication/pull/42) Changes authentication using Basic scheme
  to re-challenge the client when credentials in Authorization header can not be base64 decoded.

### Deprecated

- Nothing.

### Removed

- [zendframework/zend-authentication#44](https://github.com/zendframework/zend-authentication/pull/44) removes support for laminas-stdlib v2 releases.

### Fixed

- Nothing.

## 2.6.0 - 2018-04-12

### Added

- [zendframework/zend-authentication#34](https://github.com/zendframework/zend-authentication/pull/34) adds support for PHP 7.2.

### Changed

- [zendframework/zend-authentication#14](https://github.com/zendframework/zend-authentication/pull/14) modifies the `Laminas\Authentication\Validator\Authentication` class such that
  it now will pull an adapter from the composed `AuthenticationService` instance if no
  authentication adapter is registered directly with the validator. This will only work
  if the adapter is a `ValidatableAdapterInterface` implementation (all `AbstractAdapter`
  instances are already implementations).

### Deprecated

- Nothing.

### Removed

- [zendframework/zend-authentication#30](https://github.com/zendframework/zend-authentication/pull/30) removes support for HHVM.

- [zendframework/zend-authentication#30](https://github.com/zendframework/zend-authentication/pull/30) removes support for PHP 5.5.

### Fixed

- Nothing.

## 2.5.4 - 2018-04-12

### Added

- [zendframework/zend-authentication#9](https://github.com/zendframework/zend-authentication/pull/9) adds and
  publishes documentation to https://docs.laminas.dev/laminas-authentication/

### Changed

- Nothing.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- [zendframework/zend-authentication#29](https://github.com/zendframework/zend-authentication/pull/29) fixes how the HTTP Auth adapter treats credentials,
  ensuring it splits only on the first `:` character, and thus allows `:` characters
  as part of the password segment of the credential.

## 2.5.3 - 2016-02-29

### Added

- Nothing.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- [zendframework/zend-authentication#8](https://github.com/zendframework/zend-authentication/pull/8) updates
  dependencies to allow usage of laminas-stdlib 3.0, and to require tests to
  pass against PHP 7.

## 2.5.2 - 2015-06-15

### Added

- [zendframework/zend-authentication#4](https://github.com/zendframework/zend-authentication/pull/4) adds
  documentation, which can be compiled using [bookdown](http://bookdown.io):
  `bookdown doc/bookdown.json`; docs can then be viewed by starting a web server
  via `php -S 0.0.0.0:8000 -t doc/html/` and browsing to http://localhost:8000/.

  (Add bookdown globally using `composer global require bookdown/bookdown`.)

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- Nothing.
