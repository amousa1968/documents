![](https://octodex.github.com/plumber?1)

# documents

1. Create Project 
2. Create Repository
****  Need to figure out if can use git lfs 
3. Create Git Lfs 
4. Create .gitignore 
	- List all ignored files, directories, folders in the project not to be imported in github repository, see below
# Ignoring directories in Git repos
		.log
		.dat
		.updt
		.gitignore

# ignore clearcase unwanted directories & folders
		.git/
		example1/
		example2/
		example3/
5. Rebase clearcase snapshot by a label
6. Do not execute git init after creating the new repository
7. Create .gitattributes file to control accessing from Linux, Windows and OS X, contains some files with (CRLF line-endings).  

# Set the default behavior, in case people don't have core.autocrlf set it to (text=auto)
   - echo "* text=auto" >.gitattributes
   - On Windows, you simply pass true
   - Refreshing a repository after changing line endings
8. git lfs install  
9. git lfs install --local 
10.git config -f .gitconfig "URL for the Artifactory"
11.git lfs track  list of file extenstions to track sending to Artifactory
12.git add .gitconfig & .gitattributes 
13.push clearcase label_tag to github master remote repo
14.Add commit label and date
15.git log -z --reverse --pretty=format:%H%x01%B --first-parent master_ci..
16.Push the files to origin
17.git push origin master   https:/\name:password@domain.name\name/repo.git
18.Push the label_name to origin
19. End of steps...........
