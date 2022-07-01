## How to include the Guidelines to your Spectral lint

If you decide to add our spectral guidelines, you must have npm installed.
Then you need to add it as npm dependency.
To do so, you first need to create a package.json file with the following content:
```
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
Your spectral.yml ruleset needs to include the module as following:
```
extends: 
    - '@doubleslashde/rest-complete-set'
```
After you did the configuration, you can pull the ruleset with `npm install`. 
Then you can run the linting with `npm run lint`.
