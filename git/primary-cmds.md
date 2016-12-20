
Generating a new SSH key

`$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"# Creates a new ssh key, using the provided email as a labelGenerating public/private rsa key pair.`


Adding your SSH key

```
$ eval "$(ssh-agent -s)"Agent pid 59566
$ ssh-add ~/.ssh/id_rsa
```

Config

```
$ git config --global user.name "bentan2013"
$ git config --global user.email "aa@bb.com"
```



Create a new repository

```
echo "# test" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:bentan2013/test.git
git push -u origin master
```

Push an existing repository

```
git remote add origin git@github.com:bentan2013/test.git
git push -u origin master
```


Work with Git

````

$ git clone ${repo_url}

$ git branch -a
$ git branch dev
$ git checkout dev

$ git add filename
$ git add .

$ git status
$ git commit -a -m "add 3 files"
$ git push origin dev:dev

$ git diff dev master

$ git checkout master
$ git merge -m "msg" dev

$ git branch -d dev #remove branch

```
Tips

Use .gitignore to ignore files

```
text.txt

*html

!test.html

*.[oa]
```








Examples:

https://github.com/skywinder/github-changelog-generator#output-example

