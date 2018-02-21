# Initialize GitHub

## Tutorial
[Interactive Git Tutorial][1]
[GIT Command Line Basics][2]

## Install Git

Install
```
$ sudo apt-get install git-all
```

Check installation
```
$ git --verison
```

set global parameters
```
$ git config --global user.name $NAME
$ git config --global user.email $EMAIL
```

check parameters
```
$ git config --list
```

setup github clone
first make repository on [github][3]

```
git clone <url> .
```

initialize git repository
```
$ git init
$ git status
```

create list of ignore files
```
$ touch .gitignore
```

commiting
```
$ git add -A
$ git reset
$ git commit 
```

useful commands
```
$ git diff
$ git status
$ git branch
$ git merge $FILE
```

[1]: https://learngitbranching.js.org/
[2]: https://www.youtube.com/watch?v=HVsySz-h9r4
[3]: https://github.com/
