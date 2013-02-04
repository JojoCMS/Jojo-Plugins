This repo forms an easy way to manage multiple repos in bulk.

You can still work with individual repos as desired.

##Setup
After cloning this repo you need to initialise the submodules then fetch them:
```bash
git submodule init
git submodule foreach git pull origin master
```

To update all repos:
```bash
git submodule foreach git pull origin master
```

##Adding a repo
Add an new external repo using the following command:
```bash
git submodule add <url> <dirname>
```
Then commit and push.

##File modes on Linux
Easily update filemodes on all submodules using the following in the parent repository:
```bash
git submodule foreach git config core.filemode false
```
