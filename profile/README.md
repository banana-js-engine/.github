# General Rules

## Semantic Commit Messages (All repos)

Format: `<type>(<scope>): <subject>`

`<scope>` is optional.

### Example
```
feat: added new bananas
^--^  ^---------------^
|     |
|     +-> Summary in past tense.
|
+-------> Type: feat, fix, docs, qol, change.
```

**More Examples:**
- `feat`: (new feature or request, associated with the **Feature** label)
- `fix`: (minor or major bug fix, associated with the **Bug** label)
- `docs`: (changes to the documentation, associated with the **Documentation** label)
- `qol`: (refactoring production code, eg. cleaner code, performance, etc., associated with the **Quality of Life** label) 
- `change`: (changing an existing feature, associated with the **Change**)

## Creating pull requests

When you are done with an issue, open a pull request from your branch to `dev` or `development`.

> [!IMPORTANT]
> Never merge to the production (`main`) branch.

Once, you've done so you will see this pull request template:
```
# Changelog
## Features
- 
## Changes
- 
## Bugs
- 
## Quality of Life
- 
# Summary
## Overview
## Examples
```
Simply delete all the not needed headers and explain what you've done to solve the issue.

### Example
```
Issue: add new bananas
Labels: Feature
```

```
# Changelog
## Features
- added new bananas
# Summary
## Overview
I've done some insane changes to add new bananas.
## Examples
[Some examples of new bananas]
```

## Code Reviews
Any pull request should not be merged to `dev` branches without a code review from someone else.
if person A makes a pull request, another person B should review the code. If person B asks for changes,
person A should make the necessary changes and re-request review from person B. This cycle will continue 
until person B says `LGTM` which stands for `Looks good to me`.

> [!NOTE]
> If you push to your branch, the pull request should be automatically updated for the reviewer.

The rule of thumb is if you have contribution in a pull request, then a person that doesn't have contribution
in that pull request should do a review. This is just for having someone look at the pull request with fresh eyes.

> [!IMPORTANT]
> Code reviews are for merging to respective `dev` branches. If a pull request made it to the `dev` branch,
> it means it can potentially be merged with the production branch, but you shouldn't do so because merges
> `dev` -> `main` will be done together as a team.