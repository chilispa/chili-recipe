# CHILI's Semantic Commit Messages

CHILI uses [GIT](https://git-scm.com/) as Version Control System.


#### The reasons for these conventions:

* automatic generating of the changelog
* simple navigation through git history (eg. ignoring style changes)

The commit message should be structured as follows:

`<jira reference> [type]: <description>`

Examples:

`NEXT-12345 [feat]: Add super incredible feature`

`NEXT-12345 [refactor]: Extract feature behaviour`

`NEXT-12345 [test]: Resource unit tests`


Allowed <type> values:

* feat (new feature)
* fix (bug fix)
* docs (changes to documentation)
* style (formatting, missing semi colonsetc; no code change)
* refactor (refactoring production code)
* test (adding missing tests, refactoring tests; no production code change)
* chore (updating grunt tasks etc; no production code change)
* migration (adding new migration)


#### Message body:

Uses the imperative, present tense: “change” not “changed” nor “changes”
Includes motivation for the change and contrasts with previous behavior
