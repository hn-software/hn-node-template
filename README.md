# HN Node Template

Ready-to-code, strict template for node applications.

A HN product.

## Usage

Clone the repo with SSH:

```
  git clone --depth 1 git@github.com:hn-software/hn-node-template.git
  cd hn-node-template
  npx rimraf ./.git
```
or

Clone the repo with https:

```
  git clone --depth 1 https://github.com/hn-software/hn-node-template.git
  cd hn-node-template
  npx rimraf ./.git
```

Install the dependencies:

```
npm  install
```

## Development environment

Linux is recommended since some features *might* not work on windows. Everything is tested for linux.

## Linting

This template contains very strict rules for linting. If some linting rule is blocking your change and you are 100% sure that the change should be done with your way or it's better to do with your way, change/disable the rule instead of changing your code.

You can use eslint comments to disable rules for some parts. If you do that please add a comment to explain why that was necessary.

If you see something good to have is not checked by linters please add a TODO or create a github issue so we can work on a new linting rule.

There is also `.editorconfig` file included in the template. Most of the crucial file settings will be automatically configured for you. Some of the code editors support `.editorconfig` natively and some editors support it with plugins. You can check [editorconfig's website](https://editorconfig.org/) to see if your code editor supports it. Eslint will still check the file settings. `.editorconfig` is just for setting up your code editor automatically and there will be no manual file settings change required for supported settings.

## Testing

Create exact same project structure in `test/unit` folder to unit test your code.

## Open to contribution

If you encounter any settings, code etc. that you don't like and you know a better way to do the same thing, do not hesitate to create a pull request for the change. If you know any way to enhance the template, do not hesitate to add or remove something.

For major changes, please open an issue first to discuss what you would like to change.

## Dependencies

Dependencies are using the exact specified version. Without `^1.0.0` or `~1.0.0`. It's `1.0.0`. Please follow the same approach. Dependencies are manually updated to see all the changes in packages and apply new features to the template.

## Documentation

Whenever you update/delete/add something, please update/create documentation with your change. Update `README.md` file if it's necessary. Try using comment lines to explain things.

## Git

Create granular commits and branches. Follow SRP. A commit or branch should not include *anything* unrelated with that change.

If you find some optimization/improvement unrelated with your current change create another branch.

In github settings, squash and merge is forced. So if you create a merge request for more than one thing, it will be hard for someone to understand changes by looking the commit history.

### .gitignore

Our .gitignore has been created with [gitignore.io](https://www.toptal.com/developers/gitignore). It is updated manually time to time. Please do not touch the generated part. Below you can add or override anything.

### Pre commit hooks

Pre commit hooks are configured with the help of `husky`. Tests and linters will run when you commit. It will reject your commit if some tests are missing, if tests fail or if linting fails.

## Github

Github workflows configured for this template.

## Recommended IDE / Editor

Everything is OK but this template is configured to work best with Visual Studio Code and tested with it.
