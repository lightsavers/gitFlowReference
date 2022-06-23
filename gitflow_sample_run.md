
```
Author: lightsavers
Created: 06092022
```

# Git Workflow Sample Run

1. Initialize git repo in local directory (only done once)

```
git init
```

2. create feature branch from dev or main branch

```
git checkout -b <feature> <dev>
```


3. Check status in current branch

```
git status
```


4. Make changes to target files

```
<< you make changes to your files in this step >> 
```


5. use . (dot) to add all files in directory

```
git add .
```


> * Or, to add one file

> ```
> git add <specificFileName1>
> ```

> * Or. to add specific several files

> ```
> git add <specificFileName1> <specificFileName2> <specificFileName3>
> ```


> * Specify user.email of target git account or if first time commit

> ```
> git config --local user.name <username>
> ```

> * Specify user.email of target git account or if first time commit

> ```
> git config --local user.email <username@example.com>
> ```


6. Add commit comment

``` 
git commit -m "This is a commit comment" 
```


7. Add remote branch (if first time only)

```
git remote add origin https://github.com/targetUserName/targetBranchName.git
```


8. Push commits to remote branch <feature>

```
git push -u origin <feature> (if working from copy of <dev> branch)
```


9. Switch to <dev> branch

```
git checkout <dev>
```


10. Pull commits information

```
git pull
```

11. Send commits to <dev> origin 

```
git pull origin <dev>
```

12. Push commits to remote branch <dev>

```
git push
```

13. Remove unrelated files from remote github repo

```
git rm --cached SampleFile.MD
git commit -m "Removing unrelated files"
git push origin main
```