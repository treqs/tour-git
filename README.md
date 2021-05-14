# Tour Git

> Learn about this powerful way to manage evolving files (code, data, text, and more)

## Working with Code

Git is a **distributed version control system** that allows developers to work together on common projects and collaborate effectively with people around the world.

This project 'tour-git' is stored in a repository (or "repo") in GitHub. GitHub is a hosting service that uses Git for managing changes to these files. 

Code stored in the cloud is safe - cloud hosting providers keep backups and allow us to share code from anywhere. 

Sometimes, we want the project files on our local machines. Local machines might have special tools installed - and enable us to work on the code files while we are offline (not connected to the internet). 

## What is a Repository (or "Repo")? 

A **repository** is a place to store content. This project is kept in a public repository at <https://github.com/denisecase/git-started-windows>.

Repositories may also be private - visible only to yourself or to a team.

## Cloud Storage Providers

There are many places to store your content while you collaborate. You may be asked to set up free accounts with popular providers:

- [GiHub](https://github.com/)
- [BitBucket](https://bitbucket.org)

Both are widely used and it can be helpful to have accounts in both places. As you create new repositories for yourself or a team, you can decide which one is a better choice for each project.

If you're a student, check both sites for the most recent education options.

- [GitHub Education](https://education.github.com/)
- [BitBucket Education](https://bitbucket.org/product/education)

## Git Connects Cloud & Local Repos

When you clone a cloud repo down to your machine, the two repos are linked. The cloud repo has a URL (e.g. https://github.com/treqs/tour-git) and cloning will create a new folder on your machine with the same repo name ('tour-git'). When we clone a repo, Git creates an alias called 'origin' to refer to the URL which simplifies our commands. 

## Transferring Files

There are two methods for transferring files from our computer to the cloud: HTTP and SSH. They offer two different ways of providing authentication and authorization.

- HTTP - to exchange files, we enter an email and password with each transfer. This is easiest.
- SSH - (optional) - we set up a public/private key pair between our computer and cloud account once at the begining and do not need to type a password with each transfer. SSH is not recommended when first getting started. If you find you use Git a lot, it might be worth exploring [SSH](./SSH.md). 

---

## Terms

- Cloud storage provider
- BitBucket
- GitHub
- Git
- TortoiseGit
- Repository/repo
- HTTP
- SSH
- SSH key pairs
- Private key
- Public key
- PuTTyGen - a graphical tool to create SSH keys

