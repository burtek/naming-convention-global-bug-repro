This is Repro for bug report https://github.com/typescript-eslint/typescript-eslint/issues/4781

Important files:
- `.eslintrc` containing rules config
- `non-failing.ts` showing [@typescript-eslint/naming-convention](https://typescript-eslint.io/rules/naming-convention) rule work as intended
- `failing.ts` being same as `non-failing.ts` but with `env` set to `node` (see eslint comment on the top of the file), showing rule failing to work

Also please try removing `global` modifier from rule config in `.eslintrc` and watch how `failing.ts` passes linter.
