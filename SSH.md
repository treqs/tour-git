# Tour SSH

If you use Git enough that you get tired of entering your username and password often, it might be worth doing a bit of extra work to configure a safe connection. 
For this method, we'll create a set of SSH key pairs - the public one will be held in the cloud, and the private one will be kept on your machine. 
By configuring our key pairs, we can avoid having to enter passwords when tranferring content. 

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
