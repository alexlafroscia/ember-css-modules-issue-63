# ember-css-modules-issue-63

This repository is a minimal reproduction of [`ember-css-modules#63`](https://github.com/salsify/ember-css-modules/issues/63), which states that `ember-css-modules` processes files more than once when one of those classes is composed from.  This is demonstrated by composing from a file that throws a PostCSS warning; the warning will be printed three times, once for the actual implementation of the erronious class, and once for each of the times that class is composed from.

## How to reproduce

Run the following:

```bash
yarn
yarn start
```
