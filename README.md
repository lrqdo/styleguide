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
Atom : https://atom.io/packages/linter-scss-lint

Unfortunately scss-lint does not support inheritance in configuration files, and is not likely to support it in the future (https://github.com/brigade/scss-lint/issues/516). And by default, scss-lint looks for the configuration file in the root of your current directory. 
This is why, for conveniency, the scss-lint.yml file is copied to the root of front-web : https://github.com/lrqdo/front-web/blob/master/package.json#L13
