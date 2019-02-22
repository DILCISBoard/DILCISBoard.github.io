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

### Versioning and branching
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
