# Git improtant commands

>## git init

>## git clone `HTTPS/SSH` name->origin

>## git status 

>## git log
>
 >### Git uses the command line pager, Less, to page through all of the information. The important keys for Less are: 
> 
>* to scroll down by a line, use `j` or `↓`
>
>* to scroll up by a line, use `k` or `↑`
>
>* to scroll down by a page, use the spacebar or the Page Down button
>
>* to scroll up by a page, use `b` or the Page Up button
>
>* to quit, use `q`
><br/>
>
>### **flags**
>* --oneline
>* --stat
>* -p
>* --graph

> ## git show `SHA`

>## git add
> git add **`.`** add all the files
> git add `filename` `filename`

>## git commit `-m"message"`

>## git diff
> show the diff between the uncommit file and the current workspace

>## .gitignore
> file created to ignore some files didn't want to be staged

>## git tag -a `tagName` SHA

>## git branch
> List all the branchs
> ## git branch `branchName`
> add the branch
> ## git branch -d `branchName`
> Delete the branch

## git checkout `branchName`

## git checkout -b `branchName`
>* to add new branch and switch to it

>## git merge `branchName`
>* fast-forward merge `just change the head point`
>* Normal merge
> ## Merge conflicts
> * When the change happens in the same line in both branches

## git commit --amend

## git revert `SHA`
>* will undo the changes that were made by the provided commit
> *creates a new commit to record the change

## git reset `commit`
>* move the HEAD and current branch pointer to the referenced commit
>*  erase commits with the `--hard` flag
>* moves committed changes to the staging index with the `--soft` flag
>* unstages committed changes `--mixed` flag

## git remote
>* It's possible to have links to multiple different remote repositories.
>* A shortname is the name that's used to refer to a remote repository's location. Typically the location is a URL, but it could be a file path on the same computer.
>* `git remote add` is used to add a connection to a new remote repository.
>* `git remote -v` is used to see the details about a connection to a remote.

## git push `remoteName` `branchName`

## git pull `remoteName` `branchName`
>* the commit(s) on the remote branch are copied to the local repository
>* the local tracking branch `(origin/master)` is moved to point to the most recent commit
>* the local tracking branch `(origin/master)` is merged into the local branch `(master)`

## git fetch `remoteName` `branchName`
>* fetching remote changes (which adds the commits to the local repository and moves the tracking branch to point to them)
>* and didn't merging the local branch with the tracking branch

## git shortlog
>* group commits by author

## git log --author="`Name`"

## git log --grep="`message`"

## git rebase -i `<base>`
>* to edit commits
