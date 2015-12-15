# SVN Setup
[Have Windows?](windows svn)
### Install X-Code
If you haven't already installed X-Code on your computer, open ```Terminal``` and run

```
xcode-select --install
```

### Install Homebrew
```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### XQuartz
It may tell you that you have to install [XQuartz](http://www.xquartz.org/)\.

### Install SVN
```
brew install svn
```

### Adding SVNs
Navigate to your desired folder location for the SVN files. See the Core Commands section [here](https://github.com/0nn0/terminal-mac-cheatsheet/wiki/Terminal-Cheatsheet-for-Mac-(-basics-))\.
Log into [Assembla](https://www.assembla.com/) and go to the directory that you would like to check out.
Once you have it, run
```
svn checkout [checkout url]
```
You may have to type ```p``` to accept the fingerprint.
Type in your computer password and then your login info for Assembla.
This may take a while. Don't close your computer or stop the internet connection or it will error out.

Checkout any other directories you'd like to have!

## Updating SVN
If you'd like the most up to date copy of a directory, cd into that directory's folder and run
```
svn update
```