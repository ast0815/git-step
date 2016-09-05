git-step
========

Check out commits between the current HEAD and a destination step-by-step.

USAGE
-----

    git step <DESTINATION>

Check out the next commit on the way to `<DESTINATION>`.
Works only if `<DESTINATION>` is a direct child of the current `HEAD`
and no merges happened in between:

    HEAD -> A -> B -> C -> DESTINATION

In this case `git step DESTINATION` will check-out `A`, `B`,
`C` and `DESTINATION` in turn.
