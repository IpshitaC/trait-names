# Personality Insights Trait Names
![last-release](https://img.shields.io/github/tag/personality-insights/trait-names.svg)
[![npm-version](https://img.shields.io/npm/v/personality-trait-names.svg)](https://www.npmjs.com/package/personality-trait-names)
[![npm-license](https://img.shields.io/npm/l/personality-trait-names.svg)](https://www.npmjs.com/package/personality-trait-names)
[![Build Status](https://travis-ci.org/personality-insights/trait-names.svg?branch=master)](https://travis-ci.org/personality-insights/trait-names)
[![codecov.io](https://codecov.io/github/personality-insights/trait-names/coverage.svg?branch=master)](https://codecov.io/github/personality-insights/trait-names?branch=master)
[![npm-downloads](https://img.shields.io/npm/dm/personality-trait-names.svg)](https://www.npmjs.com/package/personality-trait-names)

Obtain names for Personality Insights' traits.

## Getting Started

1. Require and instance `personality-trait-names` component

  ```JavaScript
  const PersonalityTraitNames = require('personality-trait-names');
  const traitNames = new PersonalityTraitNames({ locale: 'es' });
  ```

2. Get your trait name

  ```JavaScript
  const opennessName  = traitNames.name('Structure');
  ```

3. Render names somewhere! Try rendering them as cards!

See the complete [example code][example_code] or [try it live][live_example]

## More Features

There are more features available such as:

- Including the component as a browser script. Component will be exported as the
global variable `PersonalityTraitNames`.

## API Methods

The available methods are the following ones:
  - `constructor :: (Options) -> PersonalityTraitNames` - Obtain an instance of `PersonalityTraitNames`.
  - `name :: (TraitID) -> String` - Obtain the name for the given `TraitID`.

Definitions:
 - `TraitID` is a `String` ID from IBM Watson Personality Insights traits.
 - `Options` are options for the trait descriptions component. Available options are:
   - `locale` - A `String` with the locale used to generate the names.

 [example_code]: https://github.com/personality-insights/trait-names/blob/master/examples/example.html
 [live_example]: https://rawgit.com/personality-insights/trait-names/master/examples/example.html
