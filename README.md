## Automated pull request merging based on modified files
\
Automatic merge if the github user modified its own file in the root directory doing a pull request.\
\
Find the action yml file at `.github/workflows`.

### How it works?
- Checks if the github pull request proposed modified its own file in the root directory.
- The automated action checks that the file matches with its `${username}.json`.
- Then merges the pull request if it matches.

### When it fails?
- Fails if the filename is different than `${username}.json`.
- Fails if more than one file is commited in the same pull request.

### What if I cannot make it work?
- Contact me at leon@dandelionlabs.io
