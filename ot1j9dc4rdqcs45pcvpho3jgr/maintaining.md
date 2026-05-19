# Maintaining
Ensure the pre-requisites of [contributing.md](<!-- insert link -->) are met before doing any maintenance.

## Merging Pull Requests
```bash
pixi run -e dev gh pr merge --squash --delete-branch
```
>If there are more than 1 pr, an interactive prompt will appear to allow selection

This will squash and merge the pr, automatically delet the issue branch and check out to main branch.

## Versioning
If the pull request bumps the version, tag the commit:
```bash
pixi run -e dev git tag -a v<version> -m "release version <version>"
```
where \<version> is the version after released. It should contain only numbers and decimals.

For example, if the version to be released is 1.3.3, you will run:
````bash
pixi run -e dev git tag -a v1.3.3 -m "release version 1.3.3"
```