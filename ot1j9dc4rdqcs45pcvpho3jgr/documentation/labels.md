# Labels
Every label consist of the category and the value and are in the lowercase format of \<category>:\<value> 

## Values of label types
Each category has a type and can take on a defined set of values:
| Type | Values | example |
| ---- | ------ | ------- |
| boolean | 1. true<br>2. false | is_done: true |
| integer | any integer | number_of_dependencies: 5 |
| real | any floating point number | progress: 0.82 |
| string | any text | name: example |
| enumeration | a fixed set of values provided in their respective description | scope: content |

## Categories
The values for enumeration type labels is provided in their corresponding description cell.
| Category | Type | Description |
| -------- | ---- | ----------- |
|scope|enumeration|The section that is changed.<br><br> &nbsp;&nbsp;&nbsp;&nbsp; 1. content: The actual content.<br> &nbsp;&nbsp;&nbsp;&nbsp; 2. docs: Documentation about this repository, i.e. meta-documentation (README, contributing, license, etc).<br> &nbsp;&nbsp;&nbsp;&nbsp; 3. workflow: Continuous Integration (CI) related.|
|type|enumeration|The type of ticket.<br><br> &nbsp;&nbsp;&nbsp;&nbsp; 1. bug: Incorrect information, broken links, typos or errata.<br> &nbsp;&nbsp;&nbsp;&nbsp; 2. suggestion: Proposed improvements or new ideas.|

