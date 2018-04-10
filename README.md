# oomph-ux-buildkit
The buildkit is platform idependant, we should be able to include it on all our
Drupal and WordPress projects.

All tests are run on the precommit hook but can be overidden using a --noverify flag (not yet)

## Requirements
* Node 8.9+
check out nvm...
for accessibility testing tht needs some configuartion and added to a task,
or can be added as a seperate task
gulp buld tasks vs lint/test tasks
add copy tasks

## Tools
### Stylelint
under the hood for scss testing we use stylelint, styles are broken up into 3
major categories:
* Possible Errors,
* Limit Language Features
* Stylistic Issues
more can be found here: stylelint link.

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

## Roadmap
* accessibility testing
* sass doc - all our stuff should be formated to create auto documentation
* kss - living styleguide builder
* lighthouse - automated performance testing
* basic html/css testing (browser compat)
* precommit testings
* add travis

https://www.npmjs.com/package/pre-commit
https://www.npmjs.com/package/pre-push
https://www.npmjs.com/package/copy

## Issues
https://thinkoomph.jira.com/projects/OUXE
