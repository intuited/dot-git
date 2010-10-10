dot-git
=======

A repository of git repository contents.

The idea is to create a git repository in the .git directory of a git repository.

This "meta-repo" can then be used to track and propagate changes to hooks and other repository configuration files.

The `baseline` branch of this repository should match up with the set of files created by git in a fresh repository.


Setup
-----

The easiest way to use this system is to follow these steps:

-   In the directory where you will create your main repository, clone this one as `.git`.
-   Run `git init`.

If you want to apply this system to an existing repository, these instructions might work:

-   `cd` into your main repo's `.git` directory
-   `git clone` the `initial` branch of this repo.
    That branch includes just the .gitignore file.
-   `git add` the repository contents and `git commit`.
-   At this point you should be able to `merge` in a different configuration branch.
