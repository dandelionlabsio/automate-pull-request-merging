# Automatic merge if the user modified its own file in the root directory
Checks if the github pull request proposed modified its own file in the root directory.
The automated action checks that the file matches with its `${username}.json`.
Then merges the pull request if it matches.
Fails if the file is different.
Fails if more than one file is commited in the same pull request.
