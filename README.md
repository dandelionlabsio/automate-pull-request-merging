# Automatic merge of pull requests for single user file
Checks if the github pull request proposed modified its own file in the root directory.
The automated action checks that the file matches with its `${username}.json`.
Then merges the pull request if it matches.
