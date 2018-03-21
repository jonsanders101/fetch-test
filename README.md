# fetch-test

Exercise to confirm how `git fetch` works.

1) Clone this repo
2) Clone this repo again in a different directory
3) Make a change to the README in directory one
4) Commit and push the change
5) `cd` into directory two
6) Checkout a new branch
7) `$ git fetch master`
8) `$ git merge master` - this command shouldn't do anything, as the local master doesn't contain the latest commit
9) `$ git merge remote/master` - this command should merge in the latest commit made in directory one
10) Checkout master - branch should not include the remote change
11) `$ git pull master` - should pull in changes from the remote
