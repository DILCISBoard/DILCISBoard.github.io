DILCIS Board Git & GitHub Policy
================================

The DILCIS Board use [GitHub](https://github.com/) and [Git](https://git-scm.com/)
as a version and change control system for specifications and software. This document
describes the board's conventions for Git branch usage and a guide for contributors.
It doesn't provide help for Git, a command line version control tool, or
GitHub, a source code hosting platform based on Git.

Reader's wanting help on Git should start with the [official Git documentation](https://git-scm.com/doc/).
Likewise GitHub provide a extensive documentation on [their help pages](https://help.github.com/).
There are numerous third party tutorials for Git and GitHub but personal preference
is a strong factor as to what may prove most useful for you. Google is your friend
here. We do provide a list of getting started resources later in this document.

## GitHub Repositories

### Specifications
Each specification has it's own git repository hosted on our
[GitHub organisation page](https://github.com/DILCISBoard/). These are:

- The E-ARK Common Specification for Information Packages, [E-ARK-CSIP](https://github.com/DILCISBoard/E-ARK-CSIP)
- The E-ARK Specification for Submission Information Packages, [E-ARK-SIP](https://github.com/DILCISBoard/E-ARK-SIP)
- The E-ARK Specification for Archival Information Packages, [E-ARK-AIP](https://github.com/DILCISBoard/E-ARK-AIP)
- The E-ARK Specification for Dissemination Information Packages, [E-ARK-DIP](https://github.com/DILCISBoard/E-ARK-DIP)
- The E-ARK Specification Electronic Record Management Systems, [E-ARK-ERMS](https://github.com/DILCISBoard/E-ARK-ERMS)

## Contributing the specification process
We use [GitHub](https://github.com/) to organise, assign and review the work of
the specification group. This means that to participate you'll need to sign up
to [GitHub and get a GitHub id](https://github.com/join).

### GitHub tools and references
This is intended as a guide to GitHub, there are plenty of good online resources.
[GitHub's official guides](https://guides.github.com/) are the best place to start.
Here's a brief overview of the most important concepts and the resources available.

### Writing on GitHub
Most of your interaction with GitHub itself will be via it's online forms, which
are generally simple. Most forms provide a free text box for comments and/or a
description. While plain text is fine it lacks even rudimentary formatting. Most
places where you can enter free text on GitHub support [Markdown](https://daringfireball.net/projects/markdown/), specifically [GitHub flavoured Markdown](https://guides.github.com/features/mastering-markdown/).
This document is also written in Markdown.

### Providing feedback using GitHub issues
The simplest way of contributing is to provide feedback on the specification using
[GitHub Issues](https://guides.github.com/features/issues/). Each project has it's
own issue tracker which can be found using the Issues tab on the GitHub project page
or appending `/issues` to the projects GitHub URL. As a quick example the GitHub
issues page for the Common Specification project is available here:
https://github.com/DILCISBoard/E-ARK-CSIP/issues. The GitHub instructions for
[creating an issue are here](https://help.github.com/en/articles/creating-an-issue).

### Versioning and branching
We control change to the specification and track versions using git [branches](https://git-scm.com/book/en/v1/Git-Branching-What-a-Branch-Is) and [tags](https://git-scm.com/book/en/v2/Git-Basics-Tagging).
Each repository contains two named branches that aren't associated with a particular
version of the specification:

- `master` is the latest officially released version of the specification.
This is the designated as the main branch for the repository making it the default
branch viewed on GitHub. The information in this branch is authoritative as it has
been reviewed and approved by the DILCIS Board. If you're looking for a version of
the specification to use in your organisation or are unsure as to which branch to
use you're advised to start here.
- `integration` holds the work been done on the upcoming version of the specification.
While the work here has been reviewed by the DILCIS Board it may be subject to change
as the new specification version evolves. If you're interested in reviewing or
contributing to future versions of the specification you should start here.

Each repository also contains specific release branches named `rel/<version-no>`.
These are used to:

- allow the board and users to easily view previous versions of the specification; and
- make editorial changes to a specific version, usually correcting spelling issues or
fixing typos.

In addition specific release points are tagged and added to a project's GitHub releases
page. Tags provide a simple bookmark to a specific version of the specification.

### Providing a contribution
The branch arrangement described above allows changes to be made to a specific
version of a specification. These can then be reviewed by a member of the DILCIS
Board before publication. Changes are submitted as [GitHub pull requests](https://help.github.com/en/articles/about-pull-requests). A pull request
is simply a set of edits made to a specification. Each pull request is made against
a specific branch. It can be tricky working out which branch to use when submitting
a pull request. Here are a few guidelines:

- pull requests should rarely, if ever, be made against the master branch. This is
the officially released branch and doesn't contain the latest changes;
- pull requests should usually be created using the branch that represents the
version you wish to amend, for instance changes to version 2.0 of the CSIP should
be made agains the `rel/2.0` branch; and
- if you submit a PR against the wrong branch don't worry, there's no harm done and
a member of the review team will get in touch and help.

In order to create a pull request it's usually best to create your own copy of the
[repository on GitHub](https://help.github.com/en/articles/cloning-a-repository).
You can then make the changes you want, either on a working copy of the repository
on your own machine, or [using GitHub's web editor](https://help.github.com/en/articles/editing-files-in-your-repository). Once
your changes are ready you can [submit them as a pull request](https://help.github.com/en/articles/creating-a-pull-request), been sure to
select the appropriate branch. Again if you make a mistake someone will get in touch
to help.
