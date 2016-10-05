# test-author-override
This is a repository where I'll try to reproduce a possible bug in pull request merging and git commits meta data.

So after creating multiple commits and merged pull requests I've narrowed it down to when a pull request is squashed and merged in ui by another user. This was what I saw in our private company repository as well.

In addition I saw what was mentioned in the support response, which is that a standard merge in the ui will create a new commit which uses primary email address and public name. I could live with this.

What I don't like is that a squash and merge ignores the author from the commit and pulls my public name and primary email address. Expected behavior would be to use authors from commits that are squashed.

In this repository there is a file named gitlog that contains snapshots of the git log between the steps to reproduce this behavior. 
