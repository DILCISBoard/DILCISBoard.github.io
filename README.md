Branches
--------

## Permanent branches
For now we'll maintain the following permanent branches in the corpus repo:

- `master` should contain the latest release version of the test cases and corpus, obviously we have no current release. For now we'll use this to control editorial policy, only test case and corpus package sets that have been externally reviewed by the A2 group, will be merged here from the `csip/rel/2.0-draft` branch.
- `csip/rel/2.0-draft` This is the internally reviewed current working version and it's name has been chosen to match the current draft CSIP specification version we're working to.
- `integration` the branch against which all Pull Requests are made, it's used to ensure that the integrated whole works, i.e. package creation, documentation generation, etc. PRs merged here will have been reviewed by the A3 team in isolation, this branch ensures tests the automation steps on the merged whole. Once this QA has passed, integration can be merged to the `csip/rel/2.0-draft` branch.

## Working branches
In addition to the permanent branches the team will create working branches when producing test cases and corpus packages. These should follow a hierarchical naming convention, `<spec-name>/<spec-part>/<req-id>`. We don't need to be prescriptive about the value of `<spec-part>`, the intention is too allow logical grouping without agonising over classification. These branches will track all of the work done on a particular requirement from test case definition through corpus package creation and review. Once a test case branch has been reviewed by the A2 group and merged to master the working branch can be deleted.
