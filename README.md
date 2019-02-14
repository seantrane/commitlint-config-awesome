# commitlint-config-awesome

> An awesome variation of [@commitlint/config-conventional](https://github.com/conventional-changelog/commitlint/blob/master/@commitlint/config-conventional).

---

[![Build Status](https://travis-ci.com/seantrane/commitlint-config-awesome.svg?branch=master)](https://travis-ci.com/seantrane/commitlint-config-awesome)[![devDependencies Status](https://david-dm.org/seantrane/commitlint-config-awesome/dev-status.svg)](https://david-dm.org/seantrane/commitlint-config-awesome?type=dev) [![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/) [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)

[![npm latest version](https://img.shields.io/npm/v/@seantrane/commitlint-config-awesome/latest.svg)](https://www.npmjs.com/package/@seantrane/commitlint-config-awesome) [![npm downloads per week](https://img.shields.io/npm/dw/@seantrane/commitlint-config-awesome.svg)](https://www.npmjs.com/package/@seantrane/commitlint-config-awesome) [![npm total downloads](https://img.shields.io/npm/dt/@seantrane/commitlint-config-awesome.svg)](https://www.npmjs.com/package/@seantrane/commitlint-config-awesome)

## Table of Contents

- [About the Package](#about)
- [Install](#install)
- [Usage](#usage)
- [Custom Configuration](#custom-configuration)
- [Support](#support)
- [Contributing](#contributing)
- [Changelog](#changelog)
- [License](#license)

---

## About the Package <a id="about"></a>

This package is a [`commitlint`](https://github.com/conventional-changelog/commitlint) configuration for commit message conventions and enforcement. It's a modified variation of [@commitlint/config-conventional](https://github.com/conventional-changelog/commitlint/blob/master/@commitlint/config-conventional), with the following enhancements:

- Commit message header-length is extended to 80 characters, _provoked by lengthy Greenkeeper's commit message subject lines_.

_[Learn more about `commitlint` configuration](https://github.com/conventional-changelog/commitlint#config)._

## Install <a id="install"></a>

```sh
npm install -D commitlint-config-awesome
```

## Usage <a id="usage"></a>

Use the `"extends": "awesome"` property in your `commitlint` config, then add any additional configuration as required.

### Using `package.json` file

```json
{
  "commitlint": {
    "extends": ["awesome"]
  }
}
```

### Using `.commitlintrc.json` file

```json
{
  "extends": ["awesome"]
}
```

### Using `.commitlintrc.yml` file

```yaml
extends: [awesome]
```

### Using `commitlint.config.js`, `.commitlintrc.js` file

```js
module.exports = {
  extends: ['awesome']
};
```

## Custom Configuration <a id="custom-configuration"></a>

There are many ways to implement custom configurations. Review [the complete list of possible rules](https://github.com/conventional-changelog/commitlint/blob/master/docs/reference-rules.md) to learn more.

You can override the rules immediately following the `extends` property. See the following examples.

### Using JSON

```json
{
  "extends": ["awesome"],
  "rules": {
    "header-max-length": [0, "always", 100]
  }
}
```

### Using YAML

```yaml
extends: [awesome]
rules:
  header-max-length: [0, 'always', 100]
```

### Using JavaScript

```js
module.exports = {
  extends: ['awesome'],
  rules: {
    'header-max-length': [0, 'always', 100]
  }
};
```

### Forking and publishing your own configuration

Depending on how far down the rabbit role you need to go, you may want to publish your own configuration.

Fork the repo, then perform a few find-replace tasks on all files in your version of the repository:

1. _Find_ `commitlint-config-awesome`, _replace_ with `commitlint-config-your-config-name`
2. _Find_ `awesome`, _replace_ with `your-config-name`
3. _Find_ `seantrane`, _replace_ with `your-profile`
4. Delete files; `rm -Rf CODEOWNERS CONTRIBUTING.md`

---

## Support <a id="support"></a>

Submit an [issue](https://github.com/seantrane/commitlint-config-awesome/issues/new), in which you should provide as much detail as necessary for your issue.

## Contributing <a id="contributing"></a>

Contributions are always appreciated. Read [CONTRIBUTING.md](https://github.com/seantrane/commitlint-config-awesome/blob/master/CONTRIBUTING.md) documentation to learn more.

## Changelog <a id="changelog"></a>

Release details are documented in the [CHANGELOG.md](https://github.com/seantrane/commitlint-config-awesome/CHANGELOG.md) file, and on the [GitHub Releases page](https://github.com/seantrane/commitlint-config-awesome/releases).

---

## License <a id="license"></a>

[ISC License](https://github.com/seantrane/commitlint-config-awesome/blob/master/LICENSE)

Copyright (c) 2018 [Sean Trane Sciarrone](https://github.com/seantrane)
