$ git clone https://github.com/moxe228/KotlinAsFirst2020

$ git remote add upstream-my https://github.com/moxe228/KotlinAsFirst2021

$ git fetch upstream-my

$ git rebase --onto master 661ee4adb31f9955817a1257a3588800fa464d64 upstream-my/master

$ git branch backport

$ git checkout master

$ git merge backport

$ git remote add upstream-theirs https://github.com/qvchoq/KotlinAsFirst2021

$ git fetch upstream-theirs

$ git merge -s ours upstream-theirs/master

$ git remote -v > remotes

$ git add remotes

$ git commit -m "Add remotes file"

$ touch howto.md

$ git add howto.md

$ git commit -m "Add howto.md"

$ git push

$ git checkout backport

$ git push --set-upstream origin backport