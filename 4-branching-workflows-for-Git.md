## Git Flow
The Git Flow is the most known workflow on this list. It was created by Vincent Driessen in 2010 and it is based in two main branches with infinite lifetime:
master — this branch contains production code. All development code is merged into master in sometime.
develop — this branch contains pre-production code. When the features are finished then they are merged into develop.

### Advantages
* Ensures a clean state of branches at any given moment in the life cycle of project
* The branches naming follows a systematic pattern making it easier to comprehend
* It has extensions and support on most used git tools
* It is ideal when there it needs to be multiple version in production
### Disadvantages
* The Git history becomes unreadable
* The master/develop split is considered redundant and makes the Continuous Delivery and the Continuos Integration harder
* It isn’t recommended when it need to maintain single version in production

## GitLab Flow
The GitLab Flow is a workflow created by GitLab in 2014. It combine feature-driven development and feature branches with issue tracking. The most difference between GitLab Flow and GitHub Flow are the environment branches having in GitLab Flow (e.g. staging and production) because there will be a project that isn’t able to deploy to production every time you merge a feature branch (e.g. SaaS applications and Mobile Apps)

### Advantages
* It defines how to make the Continuous Integration and Continuous Delivery
* The git history will be cleaner, less messy and more readable (see why devs prefers squash and merge, instead of only merging, on this article)
* It is ideal when it needs to single version in production
### Disadvantages
* It is more complex that the GitHub Flow
* It can become complex as Git Flow when it needs to maintain multiple version in production

## One Flow
The One Flow is a proposed alternative in article GitFlow considered harmful by Adam Ruka, written in 2015. The main condition that needs to be satisfied in order to use OneFlow is that every new production release is based on the previous release. The most difference between One Flow and Git Flow that it not has develop branch.
### Advantages
* The git history will be cleaner, less messy and more readable (see why devs prefers squash and merge, instead of only merging, on this article)
* It is flexible according to team decisions
* It is ideal when it needs to single version in production
### Disadvantages
* It isn’t recommended for projects with Continuous Delivery or Continuous Deploy.
* The feature branches make it harder the Continuos Integration
* It isn’t recommended when it needs to maintain single version in production
