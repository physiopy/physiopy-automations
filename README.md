# physiopy-actions-workflows
A place to test github actions & workflows, and perhaps also automation related to the project board 

## Workflows implemented in this test repo
<!-- Some workflows exist in the physiopy repos that are not listed here -->

### [auto-author-assign.yml](.github/workflows/auto-author-assign.yml) 
- this workflow automatically makes the author of a PR or Issue the assignee of it. This should facilitate integration with the project board, because the project board reads the 'Assignee' label
- this workflow has been implemented in these physiopy repos:
   - [phys2bids](https://github.com/physiopy/phys2bids)

### [auto-label.yml](.github/workflows/auto-label.yml) 
- this workflow automatically assigns labels to a PR if the PR edits a specific file. The mapping between file and label is defined in [labeler.yml](.github/labeler.yml) and this mapping/dictionary file can be expanded for each physiopy repo 
- this workflow has been implemented in these physiopy repos:
   - [phys2bids](https://github.com/physiopy/phys2bids)
