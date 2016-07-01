# Developer Onboarding Roadmap

## Day 1 - Learning DVCS concepts and GIT

Pre-requisites: 
* Jeavio Github Account with an organization setup 
	* All repositories will have to be public so ensure this organization is used only for training purpose
	* Do not use product code based for GIT training
* Personal Github Account created and attached to the Jeavio organization.
* You can use http://www.sonatype.com/books/mvnex-book/mvnex-examples.zip as a project on which you want to do the training exercises.

Activities:
* Understand the concepts of DVCS - https://betterexplained.com/articles/intro-to-distributed-version-control-illustrated/ - 60 mins
* Follow http://www.tutorialspoint.com/git/index.htm 
    - Basic Concepts, Environment Setup - 60 mins
        + Use https://www.youtube.com/watch?v=aGadIA-WCy0 for setting up GIT client on Mac
        + Prefer the `brew` way of installing GIT
        + Generate SSH Keys and register your SSH key in the Github profile - https://www.youtube.com/watch?v=TCcWwUgQe8s
        + 15 mins overview of GIT operations - https://try.github.io/levels/1/challenges/1 
    - Life Cycle, Create, Clone, Change and Review, Commit, Push - 30 mins
    - Update, Stash, Move, Rename, Delete - 30 mins
    - Fixing Mistakes, Tag, Patch - 30 mins
    - Branching, Conflict management - 2 hour
        + Merge vs Rebase
        + Pull vs Fetch vs Remote Update
    - Read man pages for git-clone, git-commit, git-log, git-checkout, git-branch, git-remote - 60 mins
* Git Workflows - https://www.atlassian.com/git/tutorials/comparing-workflows/ - 30 mins
* Advanced Tips - https://www.atlassian.com/git/tutorials/advanced-overview - 30 mins
* Github vs Gitlab - https://about.gitlab.com/2016/01/27/comparing-terms-gitlab-github-bitbucket/

Further Reading:
* https://git-scm.com/book/en/v2 (Must Read)

## Day 2 (More GIT and Testing Practices)
Activities:
* Understanding semantic versioning [60 mins]
    - http://semver.org
    - https://www.sitepoint.com/semantic-versioning-why-you-should-using/
* Understanding `git-flow` process models [120 mins]
    - http://nvie.com/posts/a-successful-git-branching-model/ original post that started it all
    - http://jeffkreeftmeijer.com/2010/why-arent-you-using-git-flow/ nice intro
    - https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow
    - http://danielkummer.github.io/git-flow-cheatsheet/ (scroll whole page)
* Setting up AVH-Edition of `git-flow`
    - Note: It is recommended to not use the "nvie" original author’s tooling around git-flow commands, since they’re not maintained anymore and are buggy. Instead, the AVH-Edition is actively developed and maintained - so don’t use Homebrew or any apt-get style installers, instead opt straight for AVH version: https://github.com/petervanderdoes/gitflow-avh
* Git GUI tools [90 mins]
    - Git-Tower ????
* Testing Practices
    - Understanding BDD [60 mins]
        + https://en.wikipedia.org/wiki/Behavior-driven_development
        + http://www.satisfice.com/blog/archives/638
    - Understanding Integration Tests [30 mins]
        + https://en.wikipedia.org/wiki/Integration_testing
        + http://softwaretestingfundamentals.com/integration-testing/
    - Understanding Smoke Tests [15 mins]
        + https://en.wikipedia.org/wiki/Smoke_testing_(software)
        + http://www.tutorialspoint.com/software_testing_dictionary/smoke_testing.htm
        + http://softwaretestingfundamentals.com/smoke-testing/
    - Unit testing
        + Very big topic
        + Requires practicing programming so that your code is testable
        + Requires solid understanding of SOLID principles - especially *Single Responsibility Principle*

## Day 3 - Understanding Docker

Activities:
* Start your day reading "Docker for Beginners" http://prakhar.me/docker-curriculum/ [120 mins]
    - Should we skip "Docker on AWS"?
    - Don't try building the image if you are not comfortable with python
    - Use http://zeroturnaround.com/rebellabs/docker-for-java-developers-how-to-sandbox-your-app-in-a-clean-environment/ to create an image of a Java web application
* Understanding docker ecosystem by "Digital Ocean" https://www.digitalocean.com/community/tutorials/the-docker-ecosystem-an-introduction-to-common-components [35 mins]
* Understanding docker ecosystem by "Codeship" https://dzone.com/articles/understanding-the-docker-ecosystem-via-codeship [30 mins]
* Learn how a Dockerfile is used to build a Docker image
* Learn how you can mount external volumes into a container to achieve file system (storage) persistence 
* Learn about how containers are stateless
* Learn about how container images are "layer"able
* Learn about docker-compose
* Learn about docker-network
* Learn about the different file storage systems (BTRFS, AUFS, ZFS, etc)
* Learn about the reasons different storage systems are better or worse for Docker images
