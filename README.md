# git-pick-mine

It is a simple wrapper around the `git cherry-pick` command. This utility can be used to cherry pick certain commits from a source branch to a destination branch, interactively. It can be performed within any branches, irresepective of your current `HEAD`.

# Installation:

- Check for a suitable location in your `$PATH` variable, or create one. Place the file in it.
- Open git bash and simply type `git-pick-mine`. You should be ready to go.


# Usage:

`$git-pick-mine source-branch target-branch`

# Walkthrough:

To apply multiple commit points that the current git author has committed in the source branch to a target branch,

- open `git bash`
- `$git-pick-mine source-branch target-branch`
- Your current local changes would be stashed, once the command is done, it would be popped out of the stash and be re-applied.
- The source branch would be checked out.
- You will be listed a set of commit logs, prompted to choose from these commit points.
- The target branch would be checked out and these commit points would be applied on top of it.
- You may need to resolve the merge conflicts and continue, if any, else after the commit points are applied without conflicts, 
you would be taken to your initial state.

