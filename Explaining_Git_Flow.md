# What is GitFlow?
GitFlow is a robust framework for managing large projects. It was developed by Vincent Driessen and helps with continuous software development.

## What are the major benefits of GitFlow?
* **Parallel Development**: GitFlow makes parallel development easy by isolating current development from the finished work.
* **Collaboration**: Two developers can see and follow what the other one is doing, provided they are working on the same feature.
* **Release Staging Area**: Before release, all completed features are merged into the develop branch, so it always remains updated. 
* **Support For Emergency Fixes**: GitFlow supports hotfix branches. This means that you can make an emergency fix without merging it with the current development.

## How does GitFlow work?
* **Develop and Master Branches**: The 'master branch' stores the release history, and the 'develop branch' is used to integrate all the features of the project.
* **Feature Branches**: A new feature resides in its own branch which can be pushed to the central repository for backup or collaboration. They should never interact directly with the master.
* **Release Branches**: Once develop has enough features, it should be forked. Henceforth, a new feature cannot be added and only release-oriented tasks can be performed. It is then merged into the master with a tag number for future reference.
* **Hotfix Branches**: These are like release and feature branches with the only difference being that they are forked off of master.

![GitFlow Workflow](https://miro.medium.com/max/2800/1*9yJY7fyscWFUVRqnx0BM6A.png)

[Click here for more information](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)