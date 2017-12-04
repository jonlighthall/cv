# latex
## Contents
### cv
Ciriculum Vitae
### ltr
Letter Template
### src
Default packages, macros, and bibliography.
### wmu
Western Michigan University thesis template.

## Installation
### Git
To check out the entire repository, use the following commands
````
git clone https://github.com/jonlighthall/latex.git
git submodule init
git submodule update
````

or

````
git clone --recursive https://github.com/jonlighthall/latex.git
````

### SVN
To check out a particular folder, use the following command
`svn co https://github.com/jonlighthall/latex.git/trunk/<dir> <name>`

## Submodules
to update the submodules, use the command
````
git submodule update --remote
````


to reset the submodules to the commit saved in the master project (super-repo)  use the command
````
git submodule update
````
this will checkout the submodules in a detached HEAD state.

To switch back to the master branch of the submodules, use the command
````
git submodule foreach 'git checkout master'
````

to save the new submodule commits (the new SHA) into the super-repo, use the command
````
git add <path> && git commit
````