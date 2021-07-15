## Automated pull request merging or deleted based on modified files
\
Automatic merge if the github user modified its own file in the root directory doing a pull request.\
Automatic close pull request and delete branch if the github user modified a different file.\
\
Find the action yml files at `.github/workflows`.

### How it works?
- Checks if the github pull request proposed modified its own file in the root directory.
- The automated action checks that the file matches with its `${username}.json`.
- Then approve (if new contributor), merges the pull request, and delete the new branch if it matches.

### When it fails?
- Fails if the filename is different than `${username}.json`.
- Fails if more than one file is commited in the same pull request.
- Close pull request and deletes branch.

### What if I cannot make it work?
- Contact me at leon@dandelionlabs.io
