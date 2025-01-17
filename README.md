# physiopy-test-workflows
This is a place to test [github actions & workflows](https://docs.github.com/en/actions), and perhaps also automation related to the project board.

## Workflows implemented in this test repo :tada:
<!-- Some workflows exist in the physiopy repos that are not listed here -->

### [auto-author-assign.yml](.github/workflows/auto-author-assign.yml) 
- This workflow automatically give the author of a PR or Issue the 'Assignee' label.
- This should facilitate integration with the project board, because the project board reads the 'Assignee' label in various ways.
- Previously to this, you had to manually add the 'Assignee' label. If this was forgotten, a PR or Issue can sit there without an Assignee, and may not properly show up on project board (or when you filter Issues/PRs by Assignee). It seems sensible to make the author the assignee in the first instance, but this can be manually changed for situations where someone else should be the assignee, or if the assignee changes. 

### [auto-label.yml](.github/workflows/auto-label.yml) 
- This workflow automatically assigns labels to a PR if the PR edits a specific file.
- For example, if the README file is edited, the 'Documentation' label will be automatically assigned.
- Previously to this, the author of the PR has to manually add labels (Note: some labels still need to be manually added, this just does the obvious ones)
- The mapping between file and label is defined in [labeler.yml](.github/labeler.yml) and this mapping/dictionary file can be expanded for each physiopy repo

### welcome bot, defined in [config.yml](https://github.com/physiopy/physiopy-test-workflows/blob/master/.github/config.yml)
- In progress - https://github.com/physiopy/physiopy-test-workflows/issues/13
- This bot automatically posts welcome and thank you messages when a contributor posts their first issue, first PR, and merges first PR
- This is a nice way to welcome and thank new contributors, but also acts as an opportunity to direct them towards the relevant contributor guidelines, as needed. 

## Are the workflows above implemented in other physiopy repos?
 
| Repo                         | auto-author-assign | auto-label | welcome bot |
| --                           | --                 | -- | -- |
| physiopy-repository-template | yes                |yes | no |
| physiopy.github.io           | pending PR         | pending PR |no |
| physiopy-community-guidelines| yes                |yes |no |
| physiopy                     | pending PR         | pending PR |no |
| phys2bids                    | yes                | yes     |no |
| peakdet                      | yes                | yes |no |
| physioqc                     | yes                | yes |no |
| phys2denoise                 | yes                | yes |no |

