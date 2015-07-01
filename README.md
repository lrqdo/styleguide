# Styleguide

Reference for our different styleguide in various languages

Please try your utmost to follow them.

As a rule of thumb, leave no errors, try to avoid warnings.

If anything stays, comment it so that the next developer does not waste time if no rule is edited.


## Javascript

How to use :
```
npm i -D lrqdo/styleguide babel-eslint
```

Add an .eslintrc file in the root of your project, that extends default rules :
```
{
    "extends": "./node_modules/styleguide/javascript/linters/.eslintrc"
}
```



## Scss

We are using https://github.com/brigade/scss-lint/#installation for linting.

```
gem install scss_lint
```
For SublimeText you can use this plugin : https://packagecontrol.io/packages/SublimeLinter-contrib-scss-lint

By default scss-lint needs to have the .scss-lint.yml file at the root of your project. You can either configure your editor to override this behavior, or copy the file at the root of your project, suing for example a npm hook in your package.json:

```
"scripts": {
    "postinstall": "cp node_modules/styleguide/scss/linters/.scss-lint.yml .scss-lint.yml"
}
```
