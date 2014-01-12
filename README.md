# angular-semver-sort [![Build Status](https://travis-ci.org/monterail/angular-semver-sort.png)](https://travis-ci.org/monterail/angular-semver-sort)

> Angular.js filter for ordering collections by [semantic version number](http://semver.org).

## Installation

```sh
bower install angular-semver-sort
```

If you’re building a Rails app, you can easily use it with [Rails Assets](https://rails-assets.org)—this package is available as `rails-assets-angular-semver-sort`.

## Usage

### semverSort()

```html
<ol ng-repeat="version in gem.versions | semverSort">
  <li ng-bind="version">
</ol>
```

### semverSort(property)

```html
<ol ng-repeat="gem in gems | semverSort:'version'">
  <li ng-bind="gem.version">
</ol>
```

## Development

Clone the repository, then:

```sh
npm install

grunt
grunt test
```

## Credits

The filter is **includes** the browser build of [node-semver](https://github.com/isaacs/node-semver), the BSD-licensed semver parser created by Isaac Z. Schlueter.

Made for [Rails Assets](https://rails-assets.org).
