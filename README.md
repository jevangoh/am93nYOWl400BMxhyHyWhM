# am93nYOWl400BMxhyHyWhM
Documentation for setting up and contributing to source code repositories.

## How to use
\<to do>

## Dev
These prerequisites are **required** for development work:
1. install [pixi](https://pixi.prefix.dev/latest/)
2. install [git](https://git-scm.com/)

### clone repository
First, clone the repository to your local machine using Git:
```bash
git clone https://github.com/javerngoh/am93nYOWl400BMxhyHyWhM.git
```
Then cd into the cloned repository:
```bash
cd am93nYOWl400BMxhyHyWhM
```

### ticket
Raise a ticket to provide feedback.
#### creation
1. create a github issue
```bash
pixi run -e dev gh issue create
```
2. Follow the prompts.
   Name of issue should be in sentence case (meaning first character of the entire name is capitalised).
   Assign the relevant metadata, mainly the labels.


#### labels
Each label consist of the category and the value and are in the format of \<category>: <value>. All labels are in lowercase and the values for each enumeration type labels is provided in their description cell.
| Category | Type | Description |
| -------- | ---- | ----------- |
|scope|enumeration|The section that is changed.<br><br> &nbsp;&nbsp;&nbsp;&nbsp; 1. content: The actual content.<br> &nbsp;&nbsp;&nbsp;&nbsp; 2. docs: Documentation about this repository, i.e. meta-documentation (README, contributing, license, etc).<br> &nbsp;&nbsp;&nbsp;&nbsp; 3. workflow: Continuous Integration (CI) related.|
|type|enumeration|The type of ticket.<br><br> &nbsp;&nbsp;&nbsp;&nbsp; 1. bug: Incorrect information, broken links, typos or errata.<br> &nbsp;&nbsp;&nbsp;&nbsp; 2. suggestion: Proposed improvements or new ideas.|
#### labels type
The values for each type:
| Type | Values | example |
| ---- | ------ | ------- |
| boolean | 1. true<br>2. false | is_done: true |
| integer | any integer | number_of_dependencies: 5 |
| real | any floating point number | progress: 0.82 |
| string | any text | name: example |
| enumeration | a fixed set of values provided in their respective description | scope: content |
### contributing
1. Raise a ticket on github issue to obtain the issue id.
2. Run `pixi run -e dev gh issue develop <issue id>`.
   This will create and checkout to the issue branch.
   The branch name will be the issue id followed by the issue title, the branch name is in kebab and lower case.
3. When changes are done, open a pull request: `pixi run -e dev gh pr create`
   PR title should be the gh issue name and followed by \# issue id in parentheses.
   For example, if the issue id is 1 and the title of the issue is "Initial test", the pr title would be "Initial test (\#1)".
   For the body of the PR, write "Closes \#<issue id>" to automatically close the issue. Using the same example, it would be "Closes \#1".
4. Pull the main branch by running `git pull origin main`.
5. Run: `pixi run -e dev gh pr merge --squash --delete-branch`
   This will squash and merge the pr, automatically deleting the issue branch and checking out to main branch.


