# How To Setup A Pip Environment
​
### Installing Pipenv For The First Time
- Check to make sure you have pipenv installed on your system
  - If the following command returns a value and not an error you're good to go.
```
$ pipenv --version
```
​
- If you got an error with pipenv --version please install
```
MAC
$ brew install pipenv
​
PC
$ pip install pipenv
```
​
### Setting up a new environment
- Traverse in your terminal to the folder that you want to turn into a pip environment
```
$ cd folder_name
```
​
- Run the following command
  - The -- part is telling the system what version of python you want to use
```
$ pipenv --three
```
​
​
### Installing Dependencies In Your Pip Environment
- Run the following command
  - Replace package name with the package you want to install
  - You can find a list of packages at https://pypi.org/
```
$ pipenv install packageName
```
​
### Running Your Programs
- You have to make sure to be inside a pipenv shell in order to run any files and programs within that environment/folder.  If you don't you won't have access to the python version, and packages that you installed into that environment/folder.
- Hop into the shell with the following command
```
$ pipenv shell
```
​
### Pip File Description
- [[source]]
  - This is the location for the environment to go install packages.
​
- [dev-packages]
  - These are packages that you will use during development but won't go to production.
  - Example: live server, testing
​
- [packages]
  - These are packages that your project require to properly work in the development stage and the production stage.
  - example: numpy, flask
​
### Pip File Lock Description
- Main reason for this file is to lock the versions of the packages that you want to have installed.
- You should really not modify this file.
Collapse



