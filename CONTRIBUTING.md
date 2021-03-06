<!--
Copyright (c) 2019, Amazon.com, Inc. or its affiliates. All Rights Reserved.
DO NOT ALTER OR REMOVE COPYRIGHT NOTICES OR THIS FILE HEADER.

This code is free software; you can redistribute it and/or modify it
under the terms of the GNU General Public License version 2 only, as
published by the Free Software Foundation. Amazon designates this
particular file as subject to the "Classpath" exception as provided
by Oracle in the LICENSE file that accompanied this code.

This code is distributed in the hope that it will be useful, but WITHOUT
ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License
version 2 for more details (a copy is included in the LICENSE file that
accompanied this code).

You should have received a copy of the GNU General Public License version
2 along with this work; if not, write to the Free Software Foundation,
Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301 USA.
-->
Contributing to Amazon Corretto
================================

Thank you for taking the time to help improve OpenJDK and Corretto.

If your pull request concerns a security vulnerability then please do not file it.
Instead, report the problem by email to aws-security@amazon.com.
(You can find more information regarding security issues at https://aws.amazon.com/security/vulnerability-reporting/.)

Otherwise, if your pull request concerns OpenJDK 8
and is not specific to Corretto 8,
then we ask you to redirect your contribution to the OpenJDK project.
See http://openjdk.java.net/contribute/ for details on how to do that.

If you wish to contribute to Corretto 8,
then you are in the right place.
Please read below about how you should document your issues and pull requests.


Getting Started
---------------

+ Make sure you have a [GitHub account](https://github.com/signup/free).
+ Submit a [GitHub Issue](https://github.com/corretto/corretto-8/issues) for your issue, assuming one does not already exist.
  + Clearly describe the issue including steps to reproduce when it is a bug.
  + Make sure you fill in the earliest version that you know has the issue.
+ [fork](https://help.github.com/articles/fork-a-repo/) your repository and check out your forked repository.

Making Changes
--------------

+ Create a topic branch from where you want to base your work (this is usually the master branch).
+ Make commits of logical units.
+ In your commit message make sure it starts with `#XXX -` where "`#XXX`" represents the number of the github issue you created for tracking purposes. Note the syntax that you can use follows:
    + fix #xxx
    + fixes #xxx
    + fixed #xxx
    + close #xxx
    + closes #xxx
    + closed #xxx
    + resolve #xxx
    + resolves #xxx
+ resolved #xxx
+ Respect the original code style:
  + Only use spaces for indentation.
  + Create minimal diffs - disable on save actions like reformat source code or organize imports. If you feel the source code should be reformatted create a separate PR for this change.
  + Check for unnecessary whitespace with git diff --check before committing.
+ Make sure your commit messages are in the proper format. Your commit message should contain the key of the GitHub issue.

Making Trivial Changes
----------------------

The GitHub Issues are used to generate the changelog for the next release.

For changes of a trivial nature to comments and documentation, it is not always necessary to create a new issue in GitHub.
In this case, it is appropriate to start the first line of a commit with '(doc)' instead of a ticket number.


Submitting Changes
------------------

+ Push your changes to a topic branch in your fork of the repository.
+ Submit a _Pull Request_ to the corresponding repository in the `apache` organization.
  * Verify _Files Changed_ shows only your intended changes and does not
  include additional files like `target/*.class`
+ Update your GitHub Issue and include a link to the pull request in the ticket.

If you prefer to not use GitHub, then you can instead use
`git format-patch` (or `svn diff`) and attach the patch file to the GitHub issue.


Additional Resources
--------------------

+ [General GitHub documentation](https://help.github.com/)
+ [GitHub pull request documentation](https://help.github.com/articles/creating-a-pull-request/)
