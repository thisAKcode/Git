Dealing with non-fast-forward errors
===============================================
ERR1

# once I tried to push to github

$ git push origin content

# Got that message meaning push was refused.

 ! [rejected]        content -> content (non-fast-forward)
error: failed to push some refs to 'https://github.com/thisAKcode/thisAKcode.github.io'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.


SOLUTION

# get changes from remote into your local catalog:
`git fetch repourl`
`git merge origin/content` # since I was working with content branch
