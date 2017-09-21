# Demo script for Git/GitHub.com from Meeting on 9/20/2017
## Authored by : Greg Doud - Max Technical Training

Create a new folder on the disk

	mkdir <foldername>

Change directory to make it the current folder

	cd <foldername>

Create a file in the folder

	touch <filename>

Edit the new file adding a line: `Production v1.0`

	edit <filename> - add text line to <filename>

Save the file

	save <filename>

Initialize the folder as a git repository

	git init

Check the status of files

	git status

Stage the new file with change for commit

	git add <filename>

Commit the file to the repository with a message of `inital commit`.

	git commit -m 'initial commit'

Create a new branch for a big enhancement

	git branch enhancement

Make the new branch our current branch

	git checkout enhancement

Edit the same file and add an additional line to it to represent the enhancement

	edit <filename>

Save the file after changes

	save <filename>

Stage the changed file to be committed

	git add <filename>

Commit the file to the repository with the message

	git commit -m 'finished enhancement request'

Switch to the `master` branch

	git checkout master

Make a new branch for an emergency bug fix

	git branch bugfix

Switch to the bugfix branch

	git checkout bugfix

Edit the file adding an additional line to represent the bug fix code

	edit <filename>

Save the file changes

	save <filename>

Stage the changed file for commit

	git add <filename>

Commit the changes to the repository with the message `finished bugfix`.

	git commit -m 'finished bugfix'

Switch back to the master branch

	git checkout master

Merge the bugfix branch into the master branch. This works fine.

	git merge bugfix

Attempt to merge the enhancement branch into the master branch. This causes a merge conflict.

	git merge enhancement

Edit the file to manually merge the code from the enhancement branch and master branch.

	edit <filename>

Stage the file with the manually merged changes

	git add <filename>

Commit the file

	git commit -m 'fixed merge conflict'

This results in both the enhancement and bugfix branchs code be integrated into the production (master) branch.