========================
Reporting or Fixing Bugs
========================

If you spot a bug (or have a feature request) and aren't sure what to do, feel free to liberally open GitHub issues!

If you spot a bug and are willing to fix it, then here's how to submit a pull request:

If you have made other changes and things are a bit messed up, you might want to use a fresh clone.
Alternatively, if in that particular file, this is the only change, no need to get a fresh clone.

Imagine we have spotted a bug in the dataloader which had the wrong variable for ``image_shape``::

  git checkout -b fixing-img-size-type # (creates a new branch for you to make changes in safely)
  git add <file you have changed>
  git commit -m 'meaningful explanation message for commit'
  git push --set-upstream origin fixing-img-size-type

Once this is done, go on GitHub:

1. Click on the top menu's option 'Pull Requests'
2. Click "new pull request"
3. Change  base repository to be ``bayeswatch-pytorch-experiments-template``
4. Choose base to be main
5. Make sure your ``HEAD`` is the new branch you made
6. Click "create pull request"

Done!
