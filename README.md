# @nodecraft/eslint-config
[![Actions Status](https://github.com/nodecraft/eslint-config/workflows/Test/badge.svg)](https://github.com/nodecraft/eslint-config/actions)

This package is modeled heavily off of [Airbnb's base config](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb-base). A huge thanks to their team.

## Usage

We export our standard ESLint configuration.

Our default export contains all of our ESLint rules, including ECMAScript 6+. It requires `eslint`, `eslint-plugin-node`, `eslint-plugin-json` & `eslint-plugin-unicorn` & `eslint-plugin-vue`.

1. Install the correct versions of each package, which are listed by the command:

```sh
npm info "@nodecraft/eslint-config@latest" peerDependencies
```

If using npm 5+, use this shortcut:

```sh
npx install-peerdeps --dev @nodecraft/eslint-config
```


2. Add `"extends": "@nodecraft"` to your .eslintrc

If your application uses Vue.js, also add `@nodecraft/eslint-config/vue` to your `extends` array to inherit our Vue rules, as well as `@nodecraft/eslint-config/vue-a11y` for our Vue Accessibility rules.