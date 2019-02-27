# Changes

## v0.8.6 (AerisWeather)

* Fix - Replaced bad GeoJSON with and "empty" (really contains 1 element) GeoJSON so mapnik doesn't blow up.
     See: https://github.com/mapnik/node-mapnik/issues/913

## v0.8.5 (AerisWeather)

* Fix - Issues with including the wrong lib at runtime
* Fix - Default to mapnik reference 3.0.22 since 3.1 isn't published yet for node-mapnik v4.2.1

## v0.8.4 (AerisWeather)
(Publish issues, same as v0.8.3)

## v0.8.3 (AerisWeather)

* Removed mapnik peering dependency. Allow our dependencies to deal with that for us.
* Removed package-lock so we don't get duplicate library issues.
* Updated tilelive-bridge, moved under @aerisweather namespace so we can use latest mapnik

## v0.8.2 - 7/12/18

* Delegate `getInfo()` to `tilelive-bridge` to prevent data leakage

## v0.8.1 - 7/10/18

* Update to match new `carto.Renderer.render()` return signature

## v0.8.0 - 6/28/18

* Upgrade `@mapbox/tilelive-bridge` to `^3.0.0`

## v0.7.0 - 5/2/18

* Support YAML input in place of a URI (or as a `yaml` property on the provided
  URI object)
* Remove deprecated `layer.name` property

## v0.6.1 - 6/14/17

* Fix dependency `require`s

## v0.6.0 - 6/13/17

* Update dependencies

## v0.5.0 - 5/27/16

* Update `tilelive-bridge` dependency to support MVT v2 spec.

## v0.4.3 - 1/18/16

* Fix `getInfo` callback

## v0.4.2 - 10/27/15

* Eliminate unnecessary (and potentially expensive) sorting of object keys to
  be written into Mapnik XML.

## v0.4.1 - 10/27/15

* Catch errors from `normalize()`

## v0.4.0 - 8/17/15

* Use newest `mapnik-reference` (for compatibility w/ mapnik 3.x)

## v0.3.0 - 1/15/15

* Declare a peer dependency on `mapnik`

## v0.2.0 - 1/15/15

* Fix use of `mapnik-reference`
* Update dependencies
* Use synchronous `carto.render()`

## v0.1.3 - 1/15/15

* Relax `mapnik` dependency to work with 3.x.x
* Update `mapnik-reference` dependency

## v0.1.2 - 7/3/14

* Handle relative paths in datasource files properly
* Partial sync with tm2

## v0.1.1 - 6/30/14

* Don't crash when a layer doesn't have an extent set (JesseCrocker)

## v0.1.0 - 4/28/14

* Initial version
