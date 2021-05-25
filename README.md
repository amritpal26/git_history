# Git History

Rewrite git commit history to update the username and email on contributions. This script will update the entire history of the repository so make sure everyone collaborating on this repository will need to fetch rewritten history.

1. Create a fresh bare clone of the repository:
	```
	git clone --bare [https://github/](https://github/)
	<username>/<reponame>.git
	```
2. Copy the provided script.sh into the repository.
3. Run the script in bash: 
	```
	bash ./script.sh
	```
4. Review the git history using `git log`.
5. Push new history to remote:
	```
	git push --force --tags origin 'refs/heads/*'
	```
