# vim-auto-commit-lint
Automatically commit linting changes when a file is saved.

## Rationale
As a developer, sometimes I modify files that are not within the linting
standards of the auto-linters that I employ.  When this happens, my changes to
the logic of my program are smashed in with the linting updates, and this is
irritating.  It would be nice if I could write a file and the linting updates
that are found were stored in a different commit.

## Stories
When I write a file, all the changes to that file that I made are saved.

Then all the linters that are going to run will run.

Then any changes that occur because of the linters are stored on a commit that
is ammended with all future changes as well.

## To DO:
Figure out the state machine underlying vim that would allow hooking into the
correct states for the above stories.
