# General Rules

## Semantic Commit Messages (All repos)

Format: `<type>(<scope>): <subject>`

`<scope>` is optional.

### Example
```
feat: added new bananas
^--^  ^---------------^
|     |
|     +-> Summary in present tense.
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