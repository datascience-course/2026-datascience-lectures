# Introduction to Data Science – Lecture Material
Course website: [http://datasciencecourse.net](http://datasciencecourse.net)

This repository will contain the material used in the lectures. For
Jupyter-based lectures, we will upload before class, so you can follow along
in Jupyter. For slide-based lectures, we upload after class to avoid spoiling
answers for in-class activities.

You can manually download the files for each lecture, but we recommend that you use git to clone and update this repository.

You can use [GitHub Desktop](https://desktop.github.com/) to update this repository as new lectures are published, or you can use the following commands (recommended):

## Initial Step: Cloning

When you clone a repository you set up a copy on your computer. Run:

```bash
git clone https://github.com/datascience-course/2026-datascience-lectures
```

This will create a folder `2026-datascience-lectures` on your computer, with the individual labs in subdirectories.

## Playing Along in Class & Updating

When you make changes to Jupyter notebooks, including simply running them, the
Jupyter notebook itself changes. This creates a discrepancy between the
version hosted on Github and the one your personal machine. If you try to
update later (see below), git will warn you about the collisions. To avoid
this, its best to save your version in its own git branch.

**Note, these instructions assume you are in the directory named
`2026-datascience-lectures`.**

First, create a branch for in class. You can name it whatever you want, but we
will name it `in-class` in this example.

```bash
git checkout -b in-class
```

The `-b` tells git to create a new branch.

Then, whenever you want to alter the lecture notebooks, make sure you are on
that branch, by checking out without newly creating:

```bash
git checkout in-class
```

To save your classwork, commit the changes in the branch:

```bash
git add [notebookname]
git commit -m "[message]"
```
Where you fill in your own notebook name and message.



## Updating

As we release new lectures or update lectures, you'll have to update your repository. Once again, you need to be in the `2026-datascience-lectures` directory.

First, make sure you are on the main branch:

```bash
git checkout main
```

Then, you can pull the newest version from the Github repository:

```bash
git pull
```

That's it – you'll have the latest version of the lectures. If you're using a
different branch to run the lectures, don't forget to checkout your in-class
branch!
