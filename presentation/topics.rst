Description:

Learn the basics of Git, used for recording the revision history of
computer code.  In this NNN-hour tutorial, you'll learn what revision
control is used for, create your first repository, make and record
changes in the repository, and publish your changes to Github.

For this session, some preparation is strongly recommended: 1) Create
an account on github.com.  2) Bring a laptop with GitHub Desktop
(https://desktop.github.com/) installed.



Topics to cover:

Introduction to version control
===============================

  Stores a bunch of text files
  Each change can be shown as a 'diff' or 'patch'
  Brief intro to reading patches (move this later?)
  Time-travel through them
  What if you travel back to an old revision, and then make a different change?
  An alternate timeline!  Introduce branches
  Three uses for branches:
  * Different versions
  * Develop and master branches
  * Feature branches
  * Multiple customers (a bad idea)

  Git supports distributed usage; you can copy the history up to a server, and pull
  down new changes.
  Github is the best known provider of a Git server, but there are
  alternatives (GitLab.com, BitBucket.org).

Tutorial
========

git clone
  Copies a repository from a server

Exercise:
  Check a copy of the git-tutorial repository
  Look at the history



git log
git show

git status
git diff
git checkout (to revert)

git add
git commit

git branch
git switch
git push
git pull


History
=======

Version control goes back to the 1970s; SCCS (Source Code Control System)
was written at Bell Labs in 1972.
https://basepath.com/aup/talks/SCCS-Slideshow.pdf

Git was originally written by Linus Torvalds.  (Image by Peter Adams from http://www.facesofopensource.com/)
Torvalds is famous for the Linux kernel (now used widely)
Explain open source software briefly.
He started it in 1991, and managed all the code himself.

By 1999 Torvalds was burning out.
The kernel began to use a proprietary software program called Bitkeeper.
In 2005 there began to be friction over the use of proprietary software to manage
a free-software project.

Torvalds wrote a first draft of git.
https://www.linux.com/news/10-years-git-interview-git-creator-linus-torvalds/

  You can actually see how it all took shape in the git source code
  repository, except for the very first day or so. It took about a day
  to get to be “self-hosting” so that I could start committing things
  into git using git itself, so the first day or so is hidden, but
  everything else is there. The work was clearly mostly during the
  day, but there’s a few midnight entries and a couple of 2
  a.m. ones. The most interesting part is how quickly it took shape ;
  the very first commit in the git tree is not a lot of code, but it
  already did the basics – enough to commit itself. The trick wasn’t
  really so much the coding but coming up with how it organizes the
  data.

  So I’d like to stress that while it really came together in just
  about ten days or so (at which point I did my first *kernel* commit
  using git), it wasn’t like it was some kind of mad dash of
  coding. The actual amount of that early code is actually fairly
  small, it all depended on getting the basic ideas right. And that I
  had been mulling over for a while before the whole project
  started. I’d seen the problems others had. I’d seen what I wanted to
  avoid doing.

Since then Git is maintained by a community, with Junio C Hamano
(pronunciation?) who now works for Google.
Development is also supported by a non-profit, the Software Freedom Conservancy.


Further References
==================

Git web page: https://git-scm.com/

Pro Git: https://git-scm.com/book/en/v2

O'Reilly Version Control with Git

Interview with Junio Hamano: https://www.youtube.com/watch?v=qs_xS1Y6nGc
