Check list for [release-tasks](https://github.com/dealii/release-papers/blob/master/release-tasks)
=================================================================================

Release preparation steps:
--

- [ ] <b>-3</b>  Send out notice to the mailinglist if anyone has outstanding issues or patches.
- [ ] <b>-2</b>  Check all issues and pull-request on github. Create a list of things to fix before the release.
- [ ] <b>-1</b>  Update the list of publications. (Send standard e-mail)
- [ ] <b>-1a</b> Start release paper process with email to all current (principal) developers
- [ ] <b>-1b</b> Update the authors list on the homepage authors.html
- [ ] <b>-1c</b> Update the list of contributors in the release paper
- [ ] <b>0</b>   Do some basic testing as always
- [ ] <b>0a</b>  Rerun cppcheck across the source files
- [ ] <b>0b</b>  Check for doxygen formatting problems
- [ ] <b>0c</b>  Fix formatting bugs reported by various command line queries
- [ ] <b>0d</b>  Check that doxygen produces no errors when generating offline docs.
- [ ] <b>0e</b>  Run the copyright script
- [ ] <b>0f</b>  Update Trilinos and PETSc to the latest release on the tester and update documentation of supported version.
- [ ] <b>0g</b>  Run codespell

Release steps:
--

- [ ] <b>*</b>   Nominate a "release officer" that is in charge of (almost all) of the following steps
- [ ] <b>1</b>   Create new changes file
- [ ] <b>1a</b>  Adjust doc/users/doxygen.html to link to the to-be-created TAG file.
- [ ] <b>4</b>   Create a release branch
- [ ] <b>5</b>   Update the VERSION from 9.0.0-pre to 9.1.0-pre on master
- [ ] <b>6</b>   Update the official tester to test on the release branch dealii-9.0
- [ ] <b>6a</b>  On mainline, update deal.II dependencies of examples
- [ ] <b>7</b>   Create an AUTHORS file
- [ ] <b>7a</b>  Send prerelease announcement to dealii@googlegroups.com
- [ ] <b>8</b>   Remove unfinished tutorial programs.
- [ ] <b>9</b>   Write up a short release note and save it as announce-9.0
- [ ] <b>9a</b>  Write the release paper
- [ ] <b>10</b>  Test the branch thoroughly
- [ ] <b>10a</b> Do the same for the code gallery examples
- [ ] <b>11</b>  Create documentation and verify
- [ ] <b>11a</b> Check that .gitattributes is up to date. (Do quick tests work?)
- [ ] <b>12</b>  Push the button
    - Change VERSION to 9.0.0 for a release and to 9.0.0-rc1 for a pre-release
    - Create a signed tag of exactly this commit
    - Push changes to github
- [ ] <b>13</b>  Create the tar files
    - Download the source tarball from github, verify that its contents is what we expect
    - Cryptographically sign it (detached, armored signature)
    - Create full offline_doc tarball and sign it
- [ ] <b>14a</b> Create a pre-release on github and upload files (and detached signatures)
- [ ] <b>15</b>  Generate the documentation on the webserver.
- [ ] <b>16</b>  Adjust header.include on homepage
- [ ] <b>17a</b> Ask Luca for Mac packages
- [ ] <b>17b</b> Update dealii in [Spack](https://github.com/spack/spack/blob/develop/var/spack/repos/builtin/packages/dealii/package.py)
- [ ] <b>17c</b> Update dealii in [Candi](https://github.com/dealii/candi/blob/master/candi.cfg)
- [ ] <b>17d</b> Update dealii in [Gentoo Science overlay](https://gitweb.gentoo.org/proj/sci.git/tree/sci-libs/dealii)
- [ ] <b>17e</b> Update dealii in [Ubuntu/Debian](https://salsa.debian.org/science-team/deal.ii)
- [ ] <b>17f</b> Update dealii in [Archlinux AUR](https://aur.archlinux.org/packages/deal-ii/)
- [ ] <b>17g</b> Update dealii virtualbox images
- [ ] <b>18</b>  Finish writing the announcement
- [ ] <b>18b</b> Adjust news.html in the deal.II homepage repo
- [ ] <b>19</b>  Announce the release via e-mail
- [ ] <b>19a</b> Send a note to the Facebook and Google+ accounts
- [ ] <b>19b</b> Update the deal.II wikipedia page
- [ ] <b>19d</b> Send thank-you email and list the people already referenced in step -1b above
- [ ] <b>20</b>  Celebrate!
