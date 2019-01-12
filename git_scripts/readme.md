An attempt to make GIT contribution just a little more comfortable

### Once you made a local clone of your fork

Please execute *git_add_upstream.bat* ONCE
which will run the following commands for you:
```
git remote -v
git remote add upstream https://github.com/rusefi/kicad-libraries.git
git remote -v
```
Now your local clone of your personal fork of rusEfi knows where it's originating from.

### Reset to current version of rusEfi with loss of your local changes
*git_reset_to_upstream.bat* would get your local copy and remote clone of rusEfi fork to latest rusEfi state by executing following commands for you:
```
git fetch upstream
git checkout master
git reset --hard upstream/master
git push origin master -f
``` 

See also https://git-scm.com/downloads