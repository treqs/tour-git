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
- SSH - (optional) - we set up a public/private key pair between our computer and cloud account once at the begining and do not need to type a password with each transfer.

## Creating SSH Keys

To enable the SSH option, we need to be able to generate a pair of keys. One public key that is kept in our account in the cloud and a private key that is kept on our machine.

A common tool is PuTTY. PuTTY includes PuTTYgen, a utility program that helps create SSH key pairs.

### SSH Public-Private Key Pairs

When I work, I use:

- Different emails
- Different computers
- Different cloud storage providers

I create a public-private key pair for every email-computer-cloud combination. For each combination, I'll create a .ppk (private key) and a .pub (public key) pair. The .pub keys are optional - if you use PuTTYgen to open your .ppk, it will show you the public key. You'll copy and paste the public key into your cloud account / settings / ssh keys.

For example, with a desktop and a laptop, I might have keys named:

```PowerShell
denisecase-pc1-bitbucket.ppk
denisecase-pc1-bitbucket.pub
denisecase-lappie1-bitbucket.ppk
denisecase-lappie1-bitbucket.pub
denisecase-pc1-github.ppk
denisecase-pc1-github.pub
denisecase-lappie1-github.ppk
denisecase-lappie1-github.pub
dcase-lappie2-github.ppk
dcase-lappie2-github.pub
```

This naming convention keeps keys organized.

### Create SSH Key Pairs & Add Public Keys To Cloud Accounts

Use Windows start to run PuTTYgen. Follow the instructions from the link below to create private keys that will be stored in your .ssh folder and corresponding public keys to be added to your BitBucket or GitHub accounts.

- <https://github.com/RedWingedJerbear/GitSSHTuttorial>

Make sure your computer is set up for developers and that you can see hidden files [1].

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

