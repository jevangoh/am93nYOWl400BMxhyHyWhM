# am93nYOWl400BMxhyHyWhM
Documentation for setting up and contributing to source code repositories.

This readme file is not the actual documentation, but the documentation for this repository itself.

## How to use


## Dev
This section describes how to contribute to this documentation repository.

### prerequisites
These prerequisites are **required** in order to contribute to this repository:
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
2. follow the prompts (assign the relevant metadata, mainly the labels)

#### labels
| Label | Type | Description |
| ----- | ---- | ----------- |
|scope|enumeration|The section that is changed.<br><br> &nbsp;&nbsp;&nbsp;&nbsp; 1. content: The actual content.<br> &nbsp;&nbsp;&nbsp;&nbsp; 2. docs: Documentation about this repository, i.e. meta-documentation (README, contributing, license, etc).<br> &nbsp;&nbsp;&nbsp;&nbsp; 3. workflow: Continuous Integration (CI) related.|
|type|enumeration|The type of ticket.<br><br> &nbsp;&nbsp;&nbsp;&nbsp; 1. bug: Incorrect information, broken links, typos or errata.<br> &nbsp;&nbsp;&nbsp;&nbsp; 2. suggestion: Proposed improvements or new ideas.|

### contributing
