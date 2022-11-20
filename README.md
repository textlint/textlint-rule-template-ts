# textlint-rule template

This is TEMPLATE REPOSITORY for creating textlint rule.

TypeScript version of <https://github.com/textlint/textlint-rule-template>

## Install

Requirements:

- Git
- Node.js 16+
- npm 8+

Use [create-textlint-rule](https://github.com/textlint/create-textlint-rule):

```
$ npx create-textlint-rule example --typescript
```

Or, Run following steps manually:

```sh
ruleName="textlint-rule-example"
git clone --depth=1 https://github.com/textlint/textlint-rule-template-ts.git ${ruleName}
cd ${ruleName}
# Initialize git
rm -rf .git/
rm -rf .github/
git init
# Initialize npm
npm init
npm install
# Initialize README
# Notice: force update exist README.md
./node_modules/.bin/textlint-scripts init
```

## Usage

See [textlint-scripts](https://github.com/textlint/textlint-scripts "textlint-scripts") for more details.

### Build

Builds source codes for publish to the `lib` folder.
You can write ES2015+ source codes in `src/` folder.

    npm run build
    
### Tests

Run test code in `test` folder.
Test textlint rule by [textlint-tester](https://github.com/textlint/textlint-tester "textlint-tester"). 

    npm test

### Publish

Publish your rule to [npm](https://www.npmjs.com/). 

    # Update version and git tag `patch` or `minor` or `major`
    npm version {patch|minor|major}
    npm publish

## How to write textlint rule?

See documentation.

- [Creating Rules · textlint](https://textlint.github.io/docs/rule.html)
