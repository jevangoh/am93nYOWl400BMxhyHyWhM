# Contributing

Please read through the following guidelines before contributing to the project.

## Issues and feature requests

Visit [support]() <!-- insert link --> for issues and feature requests.

## Repo contribution

When contributing to the repository, please follow the [code of conduct]()<!-- insert link -->. Look for tickets in Github Issues that you are confident to take on and assign it to yourself.

### Prerequisites

These prerequisites are **required** for development work:

1. install [pixi](https://pixi.prefix.dev/latest/)
2. clone the repo locally by using [git](https://git-scm.com/) in a pixi environment (recommended) or install it locally.

    a. If using local git, run

    ```bash
    git clone <repo_url>
    ```

    b. if using pixi environemnt, first create directory, then cd into the directory and init the pixi environment in the directory:

    ```bash
    pixi init
    ```

    Add git as a dependency to the dev feature

    ```bash
    pixi add git --feature dev
    ```

    clone the repository:

    ```bash
    pixi run -e dev git clone <repo_url>
    ```

    c. if you already have the repo locally, ensure the main branch is up to date.
    First checkout to the main branch:

    ```bash
    pixi run -e dev git checkout main
    ```

    Then pull the latest version from the remote repo:

    ```bash
    pixi run -e dev git pull origin main
    ```

### Development

1. Ensure you are at the root of the repository
2. Run `pixi run -e dev gh issue develop <issue_id>`.
   This will create and checkout to the issue branch.
   The branch name will be the issue id followed by the issue title, the branch name is in lower kebab case.
3. When changes are done, open a pull request: `pixi run -e dev gh pr create`
   PR title should be the gh issue name and followed by \# issue id in parentheses.
   For example, if the issue id is 1 and the title of the issue is "Initial test", the pr title would be "Initial test (\#1)".

   For the body of the PR, include "Closes \#<issue id>" to automatically close the issue automatically when the PR is merged. Using the same example, it would be "Closes \#1".
