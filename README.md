Reduced test case for potential [stylelint-no-unsupported-browser-features](https://github.com/ismay/stylelint-no-unsupported-browser-features) bug.

**Steps to reproduce**

1. `yarn`
2. `yarn run lint`

Example output:
```
PS C:\Users\<user>\Desktop\stylelint-test-case> yarn run lint
yarn run v1.0.1
$ stylelint src/**/*.less
Error: Unkonwn node type import
    at C:\Users\<user>\Desktop\stylelint-test-case\node_modules\doiuse\lib\detect-feature-use.js:152:19
    at Root.each (C:\Users\<user>\Desktop\stylelint-test-case\node_modules\postcss-less\node_modules\postcss\lib\container.js:114:22)
    at Detector.node (C:\Users\<user>\Desktop\stylelint-test-case\node_modules\doiuse\lib\detect-feature-use.js:137:13)
    at Detector.process (C:\Users\<user>\Desktop\stylelint-test-case\node_modules\doiuse\lib\detect-feature-use.js:163:12)
    at Object.postcss (C:\Users\<user>\Desktop\stylelint-test-case\node_modules\doiuse\lib\doiuse.js:40:23)
    at postCssPlugin (C:\Users\<user>\Desktop\stylelint-test-case\node_modules\stylelint-no-unsupported-browser-features\index.js:35:27)
    at Promise.resolve.then (C:\Users\<user>\Desktop\stylelint-test-case\node_modules\stylelint\lib\lintSource.js:161:9)
error Command failed with exit code 1.
info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.
```
