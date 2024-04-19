# physiopy-actions-workflows
A place to test github actions & workflows, and perhaps also automation related to the project board 

Added the label `automation` to the project board to capture some of these type of activities there - because they do not belong to one repo only! This overlaps with the labels `internal` and `testing` so perhaps they should be used instead, but label does not come up as a field when making a draft Issue on the project board. 

## Workflows implemented in this test repo

*These can be implemented in other physiopy repos, if desired*

- [auto-author-assign.yml](.github/workflows/auto-author-assign.yml) automatically makes the author of a PR or Issue the assignee of it. This should facilitate integration with the project board, because the project board reads the 'Assignee' label
- [auto-label.yml](.github/workflows/auto-label.yml) automatically assigns labels to a PR if the PR edits a specific file. The mapping between file and label is defined in [labeler.yml](.github/labeler.yml) and this mapping/dictionary file can be expanded for each physiopy repo 
