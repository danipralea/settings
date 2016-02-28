# settings
My tools &amp; settings that I use in iOS Development

#Xcode#

**Evidentiate cursor** : curl -L https://raw.githubusercontent.com/egold/better-xcode-ibeam-cursor/master/install.sh | bash together with 
**Solarized Dark** theme : https://github.com/ArtSabintsev/Solarized-Dark-for-Xcode

**Auto-increment build number** script: 

```terminal
#!/bin/bash
buildNumber=$(/usr/libexec/PlistBuddy -c "Print CFBundleVersion" "$INFOPLIST_FILE")
buildNumber=$(($buildNumber + 1))
/usr/libexec/PlistBuddy -c "Set :CFBundleVersion $buildNumber" "$INFOPLIST_FILE"
```

**Add existing project to git**:

```terminal
git init
git add .
git commit -m “First commit”
git remote add origin <remote respository URL>
git remote -v
git push origin master
```

**Add .gitignore to an existing project**:

```terminal
Commit all pending changes, then run this command:

git rm -r --cached .
This removes everything from the index, then just run:

git add .
Commit it:

git commit -m ".gitignore is now working"
```

#Terminal#

**iTerm2** : https://www.iterm2.com/

**Theme** : agnoster (add ZSH_THEME=agnoster in your .zshrc file in your home folder --->>> /Users/user_name)

**Solarized Dark Theme**: 

```
Download and unzip the latest version of the Solarized .zip file (it contains the iTerm2 preset files you’ll need):

http://ethanschoonover.com/solarized/files/solarized.zip

In iTerm2, open “iTerm2 > Preferences > Profiles > Colors”, and click “Load Presets…” to load the Solarized color schemes (light and dark) that are found in the .zip in “solarized/iterm2-colors-solarized/”

For more info see the iTerm2 README from solarized.zip - the path to it in the zip file is:

solarized/iterm2-colors-solarized/README.md
```

**Font** : `Menlo for Powerline` size 14
