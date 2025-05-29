# physiopy-automations
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END --> 
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10581500.svg)](https://zenodo.org/records/14753284)

❗Help❗the bots are everywhere. 

Don't worry, on GitHub there are many ways to automate manual tasks that users commonly do. The maintainers of the GitHub repo have chosen to add these automations in order to save time and to ensure accuracy and consistency in the execution of a task. This automation is commonly done by writing workflows made up of [GitHub Actions](https://docs.github.com/en/actions), and with the use of third-party GitHub Apps which utilises the GitHub API. 

This `physiopy-automations` repository has two purposes: 

- A place to test github automations
- A place to document what each automation is doing and why, for physiopy contributors to have a better understanding of their usage across the physiopy organisation. 

## Automations implemented in this repo :tada:

> **Please note:** there are many more workflows used within physiopy repos, [we are working towards documenting them all in this README](https://github.com/physiopy/physiopy-test-workflows/issues/16). Check out the 
[physiopy-repository-template](https://github.com/physiopy/physiopy-repository-template) to see some core repo set-up.

### 1 - [AllContributors](https://github.com/apps/allcontributors) app

This app helps recognise diverse contributions to physiopy repos, using this [emoji key](https://allcontributors.org/docs/en/emoji-key). How it works:
- Manually comment on an issue or pull request with: `@all-contributors please add @username for code and documentation`
- This will automatically open up a pull request for you to review
- Review and merge this pull request and see that the [Contributors section](#contributors-) at the bottom of the README is updated

### 2 - [auto-author-assign.yml](.github/workflows/auto-author-assign.yml) 
This workflow automatically gives the author of a PR or Issue the 'Assignee' label. This should facilitate integration with the project board, because the project board reads the 'Assignee' label in various ways. Previously to this, you had to manually add the 'Assignee' label. If this was forgotten, a PR or Issue can sit there without an Assignee, and may not properly show up on project board (or when you filter Issues/PRs by Assignee). It seems sensible to make the author the assignee in the first instance, but this can be manually changed for situations where someone else should be the assignee, or if the assignee changes. 

### 3 - [auto-label.yml](.github/workflows/auto-label.yml) 
This workflow automatically assigns labels to a PR if the PR edits a specific file. For example, if the README file is edited, the 'Documentation' label will be automatically assigned. Previously to this, the author of the PR has to manually add labels (Note: some labels still need to be manually added, this just does the obvious ones). The mapping between file and label is defined in [labeler.yml](.github/labeler.yml) and this mapping/dictionary file can be expanded for each physiopy repo. 

### 4 - welcome bot app, defined in [config.yml](https://github.com/physiopy/physiopy-test-workflows/blob/master/.github/config.yml)
This bot automatically posts welcome and thank you messages when a contributor posts their first issue, first PR, and merges first PR. This is a nice way to welcome and thank new contributors, but also acts as an opportunity to direct them towards the relevant contributor guidelines, as needed.

Example:

![image](https://github.com/user-attachments/assets/b5fa9565-851b-4c0a-8b97-e9e414276b7d)

### 5 - Zenodo with [CFF file](https://github.com/physiopy/physiopy-automations/blob/master/CITATION.cff)
We use the third-party data archiving tool Zenodo to create a DOI that can be used for archiving and citing content. To set-up Zenodo on this GitHub we followed [these steps](https://docs.github.com/en/repositories/archiving-a-github-repository/referencing-and-citing-content). Every time a new release is created, a new DOI will be issued and the [Zenodo page](https://zenodo.org/records/14753284) will be automatically updated. See the badge at the top of this README, that visitors can easily click on to reach this Zenodo page. Zenodo makes some guesses based on repo information, to populate title and authors etc. However, it is better to define this in the [CFF file](https://github.com/physiopy/physiopy-automations/blob/master/CITATION.cff) so Zenodo reports this accurately and in the way we would like. 

## Which automations above are implemented in other physiopy repos?
 
|                              | 1 | 2 | 3 | 4 |
| --                           | - | - | - | - |
| physiopy-repository-template | yes? | yes |yes | no |
| physiopy.github.io           | no | [pending PR](https://github.com/physiopy/physiopy.github.io/pull/52) | [pending PR](https://github.com/physiopy/physiopy.github.io/pull/52) |no |
| physiopy-community-guidelines| yes | yes | yes | no |
| physiopy                     | no | [pending PR](https://github.com/physiopy/physiopy/pull/11)| [pending PR](https://github.com/physiopy/physiopy/pull/11) |no |
| phys2bids                    | yes | yes | yes | yes |
| peakdet (now prep4phys?)     | yes | yes | yes |no |
| physioqc                     | yes | yes | yes |no |
| phys2denoise                 | yes | yes | yes |no |
| physiopy-governance          | no | no | no | no | 
| physutils                    | x | x | x |x |

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

