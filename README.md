#learning git

Let's learn how to branch, merge, push, pull, and all that fun stuff!

##SETUP
(create git repo on our computer, push it to github)

```
git init
git remote add origin <github_url>
git commit -m "First commit."
git push -u origin master
```


##BRANCH
(create development branch, push to github)

```
git checkout -b develop master
git push origin develop
```


##BRANCH
(create new feature branch, push to github)

```
git checkout -b new_feature develop
git push origin new_feature
```


##MERGE
(switch back to development branch, then merge in the new feature, push to github)

```
git checkout develop
git merge --no-ff new_feature
git branch -d new_feature
git push origin develop
```