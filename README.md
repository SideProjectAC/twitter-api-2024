# Dev Initial Setup

# Git Flow

## download git flow

(mac)

```
brew install git-flow
```

## fork & clone

## Initialize

```
cd my/project
git remote add upstream https://github.com/ALPHACamp/twitter-api-2020.git  # 建立上游連線
git commit -am "Initial commit"
git push -u origin master
```

## Prepare Repository for Development

```
git checkout -b develop
git push -u origin develop
```

## Setup Git Flow

```
git flow init
```

## Start to dev on your feature

```
git flow feature start <feature_name>
```

start your feature work -> add -> commit

## done the feature

merge to develop branch and delete the <feature_name> branch

```
git flow feature finish <feature_name>
```

## push develop branch to remote

```
git push origin
```

## release a version from develop branch

```
git flow release start "<version>
```

## done the release

merge into master (tagged)
back-merged into develop branch
delete the release/<version> branch

```
git flow release finish "<version>"
```
