# Follow these steps while developing

1. Make sure you created a Jira Task with a detail description

2. Create a new branch with meaningful name

| Branch Name | Description | Example |
| ----------- | ----------- | ------- |
| feature/... | create a new feature | feature/export-to-csv |
| fixbug/... | reported bug which is added to Jira | fixbug/duplicate-transaction |
| hotfix/... | a little change, will not impact current features | hotfix/change-variable-name|

3. Update CHANGELOG, increase version

- a version (e.g: 1.2.4) includes 3 parts: `MAJOR.MINOR.PATCH`

| Level | Description |
| ----------- | ----------- | 
| `MAJOR` | If your pull request/code changes is one of the following cases: <br> - It is a new release in term of organization business feature. <br> - It has breaking change that causes incompatible at any level. *Eg: change authenticatio method from basic auth to OAuth 2.0; change attribute name of API; etc* |
| `MINOR` | If you add a new function or feature in. It will be likely the most often version that you need to increase for your development work. <br> **Important note: the code changes must guarantee backward compatibility.**.                                                                                     |
| `PATCH` | If you fix bug, or add some quick changes that do not impact any existing functionality. 

- CHANGELOG must include a list of updated functions


4. Create a Pull request

- has Jira task code in tittle (*e.g: AGRNHS-283 Tuning Job xuất giao dịch sang Oracle và ghi file*)
- has a short description about changes
- request needed reviewers

5. For Repo owner, remember to remove branch after merging it
