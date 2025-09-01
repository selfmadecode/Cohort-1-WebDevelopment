# Story: Developers, Git, and GitHub

Meet three developers: **Alice**, **Bob**, and **Charlie**. They want to build a small app together.  
Alice is adding a login page, Bob is creating a dashboard, and Charlie is making the app look nice.

At first, they just share files by emailing them to each other.  
But soon they notice problems:

- Alice accidentally deletes part of Bob's dashboard.
- Charlie makes changes to the login page that Alice is also working on.
- They have multiple copies of files: *app-final*, *app-final-2*, *app-really-final* ??

Everyone is confused. They don’t know who changed what, and they can’t easily go back to fix mistakes.  
This is where **Git** comes to the rescue!

---

## What is Source Control?

Source control is like a **super organized notebook** for your project.  
It keeps track of every change, who made it, and lets you go back to any previous version.

Some tools for source control are:

- **Git**
- Subversion (SVN)
- Mercurial

Today we will focus on **Git**, which is the most popular.

---

## What is Git?

Git is a **tool installed on your computer** that keeps a history of your files.  
Think of it like a diary. Every time you finish some work, you write a note:  
*“Added login page”* or *“Fixed typo in dashboard”*.

Git allows you to:

- See what changed
- Go back to earlier versions
- Work safely with teammates

---

## What is GitHub?

GitHub is a **website** where developers can store their Git projects online.  
If Git is your notebook at home, GitHub is like a **shared library** where your team can read and edit your notebook together.

On GitHub, Alice, Bob, and Charlie can:

- Share their code
- See what everyone else is working on
- Back up their project safely

---

## The Problem Git Solves

Without Git, developers often save files with names like:  
*app-final*, *app-final-2*, *app-really-final* ??

With Git:

- All versions are saved in one place (a repo)
- You can add notes (commits) to remember what you did
- You can go back to any previous version
- Everyone can work together safely

---

## What is a Repository (Repo)?

A repository, or **repo**, is like a **box** that holds your project and its history.  
Inside the box, Git keeps track of all the changes.

Developers can have:

- A **local repo** on their computer
- A **remote repo** on GitHub to share with others

---

## How Developers Start Using Git

1. **Initialize a Repo**  
   Start tracking your project:
   ```bash
   git init
   ```
This creates a hidden folder that Git uses to store history.

**Track Files**
Tell Git which files to watch:
```bash
   git add filename.txt
   ```
**Or track everything:**
```bash
   git add .
   ```

**Commit Your Work**
A commit is like writing in your notebook:
```bash
   git commit -m "Added login page"
   ```
It records your work along with a message describing what you did.

**Push to GitHub**
Send your work online so the team can see it:
```bash
   git push origin main
   ```

How Git Tracks Changes

Git takes snapshots whenever you commit.
If only a few lines of code changed, Git saves just that part.

This makes it fast and easy for everyone to collaborate.

Story Wrap-Up

So remember:

Git = your local diary of changes
GitHub = the online library for your team
Repo = the box holding your project and history
Commit = a note in your diary
Push = sending your diary online
With Git and GitHub, Alice, Bob, and Charlie can work together, keep their changes safe,
and never worry about losing their work.

Assignments
Explain in your own words: What is the difference between Git and GitHub?
Create a new folder on your computer and initialize it with git init.
Create a file app.txt, write something, and track it with git add.
Commit the file with a message.
Change the file and commit again. Observe what happens.
Create a GitHub account and a new repository.
Push your local repo to GitHub and confirm it appears online.