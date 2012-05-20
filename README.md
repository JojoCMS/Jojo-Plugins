This repo forms an easy way to manage multiple repos in bulk.

After cloning this repo you need to initialise the submodules then fetch them:
```git submodule init
git submodule update --recursive```

To add a repo:
```git submodule add <url> <dirname>```

To update all repos:
```git submodule foreach git pull```

You can still work with individual repos as desired.
