# Release Notes for 6.x

## [Unreleased](https://github.com/laravel/framework/compare/v6.0.3...6.x)

### Added
- Added `TestResponse::assertJsonPath()` method ([#29957](https://github.com/laravel/framework/pull/29957))

### Fixed
- Fixed `__()` with `null` parameter ([#29967](https://github.com/laravel/framework/pull/29967)) 
- Fixed modifying `updated_at` column on custom pivot model ([#29970](https://github.com/laravel/framework/pull/29970))

### Changed
- Make it possible to disable encryption via `0`/`false` ([#29985](https://github.com/laravel/framework/pull/29985))

### Refactoring
- Changed imports to Alpha ordering in stubs ([#29954](https://github.com/laravel/framework/pull/29954), [#29958](https://github.com/laravel/framework/pull/29958))
- Used value helper where possible ([#29959](https://github.com/laravel/framework/pull/29959))

### TODO:
- Sort imports alphabetically on class generation from stub ([#29951](https://github.com/laravel/framework/pull/29951))
- Convert Responsables to Response objects in VerifyCsrfToken ([#29972](https://github.com/laravel/framework/pull/29972))
- Allow adding NotFoundHttpException to "allowed" exceptions in tests ([#29975](https://github.com/laravel/framework/pull/29975))
- Add events to signal when scheduled task runs ([#29888](https://github.com/laravel/framework/pull/29888))
- Postgresql column precision declaration fix ([#29873](https://github.com/laravel/framework/pull/29873))
- Allow adding command arguments and options with objects ([#29987](https://github.com/laravel/framework/pull/29987))


## [v6.0.3 (2019-09-10)](https://github.com/laravel/framework/compare/v6.0.2...v6.0.3)

### Reverted
- Reverted [Wrapped `MySQL` default values in parentheses](https://github.com/laravel/framework/pull/29878) ([#29943](https://github.com/laravel/framework/pull/29943))

### Refactoring
- Converted `call_user_func` where appropriate to native calls ([#29932](https://github.com/laravel/framework/pull/29932))
- Changed imports to Alpha ordering ([#29933](https://github.com/laravel/framework/pull/29933))


## [v6.0.2 (2019-09-10)](https://github.com/laravel/framework/compare/v6.0.1...v6.0.2)

### Changed
- Used `Application::normalizeCachePath()` method to define cache path`s ([#29890](https://github.com/laravel/framework/pull/29890), [ac9dbf6](https://github.com/laravel/framework/commit/ac9dbf6beaded2ad86f5595958c75e3c4b1147ae))
- Wrapped `MySQL` default values in parentheses ([#29878](https://github.com/laravel/framework/pull/29878))

### Fixed
- Prevent `event auto discovery` from crashing when trying to instantiate files without php classes ([#29895](https://github.com/laravel/framework/pull/29895))
- Fix resolving class command via container ([#29869](https://github.com/laravel/framework/pull/29869))


## [v6.0.1 (2019-09-06)](https://github.com/laravel/framework/compare/v6.0.0...v6.0.1)

### Fixed
- Fixed `Schedule::runInBackground()` not fired on Windows ([#29826](https://github.com/laravel/framework/pull/29826))

### Changed
- Throw `Symfony\Component\Routing\Exception\RouteNotFoundException` instead of `InvalidArgumentException` in `UrlGenerator::route()` ([#29861](https://github.com/laravel/framework/pull/29861))

### Reverted
- Reverted: [`Extract registered event and login to registered method`](https://github.com/laravel/framework/pull/27807) ([#29875](https://github.com/laravel/framework/pull/29875))


## [v6.0.0 (2019-09-03)](https://github.com/laravel/framework/compare/5.8...v6.0.0)

Check the upgrade guide in the [Official Laravel Documentation](https://laravel.com/docs/6.0/upgrade).
