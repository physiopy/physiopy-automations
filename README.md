# physiopy-test-workflows
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

This repository has two purposes: 

- A place to test [github actions & workflows](https://docs.github.com/en/actions) for the first time, and perhaps also automation related to the project board.
- A place to document what each automated workflow/action is doing and why, for physiopy contributors to have a better understanding of their usage across the physiopy organisation. 

## Workflows implemented in this test repo :tada:
<!-- Some workflows exist in the physiopy repos that are not listed here -->

### [auto-author-assign.yml](.github/workflows/auto-author-assign.yml) 
This workflow automatically give the author of a PR or Issue the 'Assignee' label. Previously to this, you had to manually add the 'Assignee' label. If this was forgotten, a PR or Issue can sit there without an Assignee, and may not properly show up on project board (or when you filter Issues/PRs by Assignee). It seems sensible to make the author the assignee in the first instance, but this can be manually changed for situations where someone else should be the assignee, or if the assignee changes. This should facilitate integration with the project board, because the project board reads the 'Assignee' label in various ways.

### [auto-label.yml](.github/workflows/auto-label.yml) 
This workflow automatically assigns labels to a PR if the PR edits a specific file. For example, if the README file is edited, the 'Documentation' label will be automatically assigned. Previously to this, the author of the PR has to manually add labels (Note: some labels still need to be manually added, this just does the obvious ones). The mapping between file and label is defined in [labeler.yml](.github/labeler.yml) and this mapping/dictionary file can be expanded for each physiopy repo. 

### welcome bot, defined in [config.yml](https://github.com/physiopy/physiopy-test-workflows/blob/master/.github/config.yml)
This bot automatically posts welcome and thank you messages when a contributor posts their first issue, first PR, and merges first PR. This is a nice way to welcome and thank new contributors, but also acts as an opportunity to direct them towards the relevant contributor guidelines, as needed.

Example:

![image](https://github.com/user-attachments/assets/b5fa9565-851b-4c0a-8b97-e9e414276b7d)


## Are the workflows above implemented in other physiopy repos?
 
| Repo                         | auto-author-assign | auto-label | welcome bot |
| --                           | --                 | -- | -- |
| physiopy-repository-template | yes                |yes | no |
| physiopy.github.io           | [pending PR](https://github.com/physiopy/physiopy.github.io/pull/52) | [pending PR](https://github.com/physiopy/physiopy.github.io/pull/52) |no |
| physiopy-community-guidelines| yes                |yes |no |
| physiopy                     | [pending PR](https://github.com/physiopy/physiopy/pull/11)| [pending PR](https://github.com/physiopy/physiopy/pull/11) |no |
| phys2bids                    | yes                | yes     | [pending PR](https://github.com/physiopy/phys2bids/pull/476) |
| peakdet                      | yes                | yes |no |
| physioqc                     | yes                | yes |no |
| phys2denoise                 | yes                | yes |no |


## Contributors ✨

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification([emoji key](https://allcontributors.org/docs/en/emoji-key)). Contributions of any kind welcome!

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/RayStick"><img src="https://avatars.githubusercontent.com/u/50215726?v=4?s=100" width="100px;" alt="Rachael Stickland"/><br /><sub><b>Rachael Stickland</b></sub></a><br /><a href="https://github.com/physiopy/physiopy-test-workflows/commits?author=RayStick" title="Code">💻</a> <a href="#maintenance-RayStick" title="Maintenance">🚧</a> <a href="https://github.com/physiopy/physiopy-test-workflows/commits?author=RayStick" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/me-pic"><img src="https://avatars.githubusercontent.com/u/77584086?v=4?s=100" width="100px;" alt="Marie-Eve Picard"/><br /><sub><b>Marie-Eve Picard</b></sub></a><br /><a href="https://github.com/physiopy/physiopy-test-workflows/commits?author=me-pic" title="userTesting">📓</a></td>
    </tr>
  </tbody>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

