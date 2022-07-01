# Spectral Ruleset for API Design Guidelines

This repository contains a ruleset for [Spectral](https://stoplight.io/open-source/spectral) based on the API Guidelines from doubleSlash Net-Business GmbH. The ruleset is published as package in the public [npm registry](https://www.npmjs.com/package/@doubleslashde/rest-complete-set/).

The latest version of API Guidelines from doubleSlash Net-Business GmbH are available in the following formats:

* HTML as [GitHub Page](https://doubleslashde.github.io/API-Design-Guidelines)
* [PDF](https://doubleslashde.github.io/API-Design-Guidelines/REST_API_Guidelines.pdf)


## Usage
If you decide to add this Spectral ruleset, you need to install `npm` as a prerequisite. Then you need to add it as dependency for npm. To do so, you first need to create a package.json file with the following content (replace the version):

```javascript
{
    "dependencies": {
        "@doubleslashde/rest-complete-set": "x.x.x",
        "@stoplight/spectral-cli": "^6.1.1"
    },
    "scripts": {
        "lint": "spectral lint path/to/openAPI"
    }
}
```
Your `spectral.yml` ruleset needs to include the module as following:
```yaml
extends: 
    - '@doubleslashde/rest-complete-set'
```
After you did the configuration, you can pull the ruleset with `npm install`. Then you can run the linting with `npm run lint`.



## Versioning

The versioning of the ruleset is done with release branches. The naming convention of the branches is as follows: 'release/vMAJOR.MINOR' (i.e. `release/v1.0`).

- The major version is incremented when rules are modified or deleted.
- The minor version is incremented when a new rule is added.



## Feedback

If you have any feedback, please reach out to us at info@doubleSlash.de.



## License
This ruleset is published under the CC BY 4.0 (Creative commons Attribution 4.0) license. Please see [LICENSE file](./LICENSE).
