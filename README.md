# physiopy-actions-workflows
A place to test github actions & workflows, and perhaps also automation related to the project board 

## Workflows implemented in this test repo
<!-- Some workflows exist in the physiopy repos that are not listed here -->

### [auto-author-assign.yml](.github/workflows/auto-author-assign.yml) 
- this workflow automatically makes the author of a PR or Issue the assignee of it. This should facilitate integration with the project board, because the project board reads the 'Assignee' label
- this workflow has been implemented in these physiopy repos:
   - phys2bids
   - physiopy-repository-template [pending](https://github.com/physiopy/physiopy-repository-template/pull/1)
   - peakdet [pending](https://github.com/physiopy/peakdet/pull/65)
   - physiopy [pending](https://github.com/physiopy/physiopy/pull/11)
   - physiopy-community-guidelines [pending](https://github.com/physiopy/physiopy-community-guidelines/pull/6)
   - physiopy.github.io [pending](https://github.com/physiopy/physiopy.github.io/pull/52)
   - physioqc [pending](https://github.com/physiopy/physioqc/pull/18)
   - phys2denoise [pending](https://github.com/physiopy/phys2denoise/pull/52)

### [auto-label.yml](.github/workflows/auto-label.yml) 
- this workflow automatically assigns labels to a PR if the PR edits a specific file. The mapping between file and label is defined in [labeler.yml](.github/labeler.yml) and this mapping/dictionary file can be expanded for each physiopy repo 
- this workflow has been implemented in these physiopy repos:
   - phys2bids
   - physiopy-repository-template [pending](https://github.com/physiopy/physiopy-repository-template/pull/1)
   - peakdet [pending](https://github.com/physiopy/peakdet/pull/65)
   - physiopy [pending](https://github.com/physiopy/physiopy/pull/11)
   - physiopy-community-guidelines [pending](https://github.com/physiopy/physiopy-community-guidelines/pull/6)
   - physiopy.github.io [pending](https://github.com/physiopy/physiopy.github.io/pull/52)
   - physioqc [pending](https://github.com/physiopy/physioqc/pull/18)
   - phys2denoise [pending](https://github.com/physiopy/phys2denoise/pull/52)
