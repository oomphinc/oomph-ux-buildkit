# oomph-ux-buildkit
The buildkit is platform idependant, we should be able to include it on all our
Drupal and WordPress projects.

All tests are run on the precommit hook but can be overidden using a --novery flag

## Requirements
* Node 8.9+

## Tools

## Linting
Linting tests can be run using NPM Scripts. If you are not fimialr with this
concept please take time to review it. NPM Scripts allows us to have one set of
wrapper scripts that we can interchangeably use should we ever decide to move
to another tool.

See the main gulpfile.js for a full list of tests that can be run.

### Scss
The two main factors behind linting our files are 1, for consistency 2, for readability.
We use the recommened guidelines from [sass-guidelines](sass-guidelin.es) as well
as a few others to maintain this philosophy.

Another benefit is automation, we should not spending time repeating tasks that
can be automated, such as code reviews. Code reviews can offer vailble feedback
best on the vest practices and the viability of our code but reviewers should not
have to worry about the granular details of things like indentation - this is
what linters are for!

## Issues
https://thinkoomph.jira.com/projects/OUXE
