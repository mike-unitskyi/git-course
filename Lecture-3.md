Tutorial for pull requests and collaboration workflow:
- Pull requests
- Workflows
- Homework
- Useful links

# 1. Pull requests: 
Pull requests make it easier for developers to collaborate. They provide a user-friendly (web) interface for discussing
proposed changes before integrating them into the official project.
In the simplest form, pull requests are means for a developer to notify a team member that they have completed a feature. But the pull-request is more than just a notification. It's a dedicated forum where teammates can post feedback, push follow-up commits.

## What does a pull request contain:
When you create a pull request, you want another developer to pull a branch from your repository into their repository. This means that you need to
provide 4 pieces of information to create a pull request:
- the source repository
- the source branch
- the destination repository
- the destination branch

# 2. Git Workflows
## Forking Workflow
In the Forking workflow, a developer pushes a completed feature to their own public repository instead of a shared one.
After that, they create a pull request to let the project maintainer know that it's ready for review.

Since each developer has their own public repository, the pull request's source repository will differ from its destination repository.
The source repository is the developer's public repository and the source branch is the one that contains the proposed changes.
If the developer is trying to merge the feature into the main codebase, then the destination repository is the official project and 
the destination branch is "master".

Steps in Forking Workflow:
- You fork a public repository
- You clone the repository (so that you have a working copy on your machine)
- You create a (feature) branch and make some commits
- You push the branch in your repository
- You create a pull request by navigating to your forked repository

## [Centralized Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows#centralized-workflow)
## [Feature-branch workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow)
## [Gitflow workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)
## [Forking workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow)
## [Github flow](https://guides.github.com/introduction/flow/)

# 3. Homework
- Integrate Jenkins with repo(create jenkins file), run build/tests on PRs, tag/release new version of code.

# 4. Useful links
- [git handbook](https://guides.github.com/introduction/git-handbook/)
- [github courses](https://lab.github.com/courses)
- [tutorials](https://www.atlassian.com/git/tutorials)
- [jenkinsfile](https://jenkins.io/doc/book/pipeline/jenkinsfile/)
- [jenkins github plugin](https://wiki.jenkins.io/display/JENKINS/Github+Plugin)

