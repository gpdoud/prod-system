# Demo script for Git/GitHub.com from Meeting on 9/20/2017

Create a new folder on the disk

	mkdir <foldername>

Change directory to make it the current folder

	cd <foldername>

Create a file in the folder

	touch <filename>

Edit the new file adding a line: `Production v1.0`

	edit <filename> - add text line to <filename>
	save <filename>
	git init
	git status
	git add <filename>
	git commit -m 'initial commit'
	git branch enhancement
	git checkout enhancement
	edit <filename> - add additional line to <filename>
	save <filename>
	git add <filename>
	git commit -m 'finished enhancement request'
	git checkout master
	git branch bugfix
	git checkout bugfix
	edit <filename> - add additional line to <filename>
	save <filename>
	git add <filename>
	git commit -m 'finished bugfix'
	git checkout master
	git merge bugfix - works flawlessly
	git merge enhancement - causes merge conflict
	edit <filename> - manually fix merge
	git add <filename>
	git commit -m 'fixed merge conflict'

