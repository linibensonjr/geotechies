# Contribution Guidelines

This document contains the guide for how to contribute using git and github. Please make sure you follow the guidelines so things do not get broken and so that your PRs would be accepted and merged.

## Git Workflow
Here is the proposed git flow for contributors:

For every feature, bug or chore, you must create a branch.

**Example for a feature**  
Create a new branch, your branch name must follow this convention: 

naming: feat/user-login 
```
git checkout -b feat/user-login 
```
**Use lower case and separated by dashes**  

**Example of a bug**  
Say you have a Home Page Typo:  
branch naming: bug/homepage-typo

**Example of a chore**  
To Update Read Me:  
Your branch naming: chore/update-readme

Once you are assigned an [issue](https://github.com/Geotechies-Uniuyo/geotechies/issues) or wants to work on a feature, create a branch on your local git and only push to that branch.  

A typical way to do so:  
run:  
```git pull origin develop``` - You must pull from develop before or after checkout
git checkout -b feat/user-login - You are in the feat/user-login branch now


### Pushing to Github
To push to github;  
```
git add . 
git commit -m "feat: implemented user login
git push origin feat/user-login - note how it ends with a branch. 
```


on github, you must make a PR to the develop branch, any PR to the master branch must be closed with immediate alacrity.

When making a PR, your PR is expected to have the following:
What is the task completed ?
What the PR actually does  ?
How can this PR be manually tested ?
Any background contexts ? (maybe something a tester might not notice and be useful for testing)
Screenshots (of your implementation - a web page, a mobile app screen or an API payload

Your commit messages should follow a consistent pattern:
Remember, chore, feature, bug
So i do not want to see stuff like I tried my best in your commit messages;
For a feature: git commit -m "feat: implemented user log-in
For a bug: git commit -m "bug: fixed inconsistency in log in screen"
For a chore: git commit -m "chore: updated read me to include API endpoints"