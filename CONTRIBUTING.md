= HyScala General Contributing Guide

If you would like to contribute to any of HyScala community projects, follow this document.

== Prerequisites

* To contribute to any HyScala projects you need a GitHub account.

== Git & Github Help

The following should help you in coming up to speed with git and github.

* https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf[Github Git CheatSheet]
* https://try.github.io/levels/1/challenges/1[Try Git commands]
* https://git-scm.com/book/en/v2[Pro Git]
* https://git-scm.com/download[Download Git]
* https://help.github.com[Github Help]

NOTE: Many of Java/Kotlin IDEs do support Git as well as GitHub out of the box.

Please read README page of any project to know the prerequisites of the project.

== Source-code Repo

Repositories of all the projects in KotlinHyderabad are at GitHub.
Link to our Github organization is http://github.kotlinhyderabad.in

== GitHub WorkFlow

KotlinHyderabad uses the following Git Workflow. This is mandetory since it utilises best practices.

* To start contributing to any project, start by `fork`ing the repository. This creates your
own copy of the code. Your changes have to go to your fork of the repository before being
integrating to the official one.

=== Clone and Config

* `clone` your fork on your local machine:

     git clone git@github.com:username/project-name.git

* [Optional] In case you have downloaded the source as a zip, add the primary
  project of your forked project as the `upstream` repository 

     git remote add upstream git@github.com:username/project-name.git

* Before you start coding, always `pull` the latest changes from the upstream branch.

     git pull upstream branch-name

=== Working on Issues
     
* When you start working on any issue, first create a branch. Name should have the
format of `repo-issueid`

     git checkout -b repo-issueid
     
* When you add the changes to staging, keep the changes modular, i.e.
- files for a single change should be part of a single commit, and not spread across commits.
- code should compile between commits without breaking any existing functionality.

     git add <filenames>

* When commiting use the IssueID and a clear commit message.

     git commit -m '<repoid>-<issueid>: <proper change description>'

* Send the changes to the upstream

     git push -u upstream HEAD
     
* Once all your changes are grouped as commits, send a pull request with your changes.


=== Thinks to keep in mind

* Provide meaningful, clear and concise descriptions.
* In any of your review discussion in github do not write mail.

Instead of

---

Dear Kumar

this function is added because ...

Thank you
Suresh

---

type

---

This function is added because .... 

---

* Use simple English, no need to write like the Shakespeare :)
* Give a couple of days for the repo owners to review and provide feedback 
* Feedback will be discussed only in github pull-request
* Once all changes/review are done, your code will be accepted. 

=== License

Each project carries its own licence which can be found in the LICENSE.md file
in the project root.


