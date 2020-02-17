<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/GIT%20TITLE%20ICON%20QUICK%20HELP.png" alt="Title Git Quick Help" class="center">


  ### Contents
- [1. Objective](#1-objective)
- [2. Versioning](#2-versioning)
- [3. About Git](#3-about-git)
- [4. 3 Stages](#4-3-stages)
- [5. Steps](#5-steps)
  - [5.1. First-Time Git Setup](#51-first-time-git-setup)
  - [5.2 SSH](#52-ssh)
  - [5.3 Copy SSH Key](#53-copy-ssh-key)
- [6. Clone Repo](#6-clone-repo)
- [7. Commiting](#7-commiting)


## Hands-on learning

 ### 1. Objective
**Quick Help git** is so you can do the initial **git steps** faster.

### 2. Versioning
Git is not a version controller centralized, Git is a distributed version control system.

The development of the copy on the workstation, will be on every workstation, not only in the repository, that is, all versions are distributed on all workstations when committed.

### 3. About Git
GIT IS A VERSION CONTROLLER, BASIC THINKING!

Illustration:
<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/illustration.jpg" class="center">

*(image created by: Weslen Almeida, with part obtained by other authors preserving their work and image rights, not for sale or shared with third parties)*

### 4. 3 Stages
- Stage Description:
<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/stages-description.jpg" class="center">

*(image created by: Weslen Almeida, with part obtained by other authors preserving their work and image rights, not for sale or shared with third parties)*

- Graphic vision stage
<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/graphic-vision-stage.jpg" class="center">

*(image created by: Weslen Almeida, with part obtained by other authors preserving their work and image rights, not for sale or shared with third parties)*

### 5. Steps
  - #### 5.1. First-Time Git Setup
**Your Identity**
The first thing you should do when you install Git is to set your user name and email address. This is important because every Git commit uses this information, and it’s immutably baked into the commits you start creating:

`$ git config --global user.name "John Doe"`

`$ git config --global user.email johndoe@example.com`

Again, you need to do this only once if you pass the --global option, because then Git will always use that information for anything you do on that system. If you want to override this with a different name or email address for specific projects, you can run the command without the --global option when you’re in that project.
Many of the GUI tools will help you do this when you first run them.

- #### 5.2. SSH
1. Open Git Bash.
2. Paste the text below, substituting in your GitHub email address.
3. `ssh-keygen -t rsa -b 4096 -C "your_email@example.com"`

<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/5-2-ssh-iii.jpg" class="center">
  
This creates a new ssh key, using the provided email as a label.
  
<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/5-2-ssh-img01.jpg" class="center">

4.	When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.

---
*Not necesseray passphrase or passward, only press enter, but if you want you can use pass, because we are going to configure SSH and for me this is enough, up to you, by the way, the more protection the better.*
***
 
<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/5-2-ssh-v.jpg" class="center">

6.	At the prompt, type a secure passphrase. For more information, see "Working with SSH key passphrases".
  
<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/5-2-ssh-vii.jpg" class="center">

- #### 5.3. Copy SSH Key
Adding a new SSH key to your GitHub account

1.	Copy the SSH key to your clipboard.
If your SSH key file has a different name than the example code, modify the filename to match your current setup. When copying your key, don't add any newlines or whitespace.

```console
clip < ~/.ssh/id_rsa.pub
# Copies the contents of the id_rsa.pub file to your clipboard
```

2.	In the upper-right corner of any page, click your profile photo, then click *Settings*.

<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/5-3-cp-ssh-ii.png" class="center">

3.	In the user settings sidebar, click *SSH and GPG keys*.

<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/5-3-cp-ssh-iii.png" class="center">

4.	Click *New SSH* key or *Add SSH key*.

<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/5-3-cp-ssh-iv.png" class="center">

5.	In the "Title" field, add a descriptive label for the new key. For example, if you're using a personal Mac, you might call this key "Personal MacBook Air".

6.	Paste your key into the "Key" field.
<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/5-3-cp-ssh-vi.png" class="center">

7.	Click Add SSH key.
<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/5-3-cp-ssh-vii.png" class="center">

8.	If prompted, confirm your GitHub password.
<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/5-3-cp-ssh-viii.png" class="center">


### 6. Clone Repo
Cloning a repository

1.	On GitHub, navigate to the main page of the repository (<>code).

2.	Under the repository name, click Clone or download.

<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/6-clone-ii.png" class="center">

3.	In the Clone with SSH section, click to copy the clone URL for the repository.

<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/6-clone-iii.png" class="center">

4.  Change the current working directory to the location where you want the cloned directory to be made.

5.	Type git clone, and then paste the URL you copied in Step 2 and 3.

`$ git clone git@github.com/YOUR-USERNAME/YOUR-REPOSITORY`


<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/6-clone-v.png" class="center">

6.	Press Enter. Your local clone will be created.
<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/6-clone-vi.png" class="center">

### 7. Commiting
$ `git add .`
$ `git commit -m "your message"`
$ `git push`

<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/7-commiting.png" class="center">


### 8. Reference
Last access 2020-02-16.

- https://git-scm.com/book/en/v2
- https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup
- https://help.github.com/en/github/authenticating-to-github/working-with-ssh-key-passphrases
- https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
- https://help.github.com/en/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account
- https://help.github.com/en/github/using-git/which-remote-url-should-i-use
- https://git-scm.com/docs/git-add


> **PS:** *All of this material is for the sole and exclusive purpose of sharing knowledge; the images used here are mine or those of others; they are not intended to be shared for personal gain, but to better clarify the information sharing process.
I apologize with English, this is a new path in which I am working hard to learn, if you noticed something wrong, out of context and it doesn't make sense, please fork and help me build this basic material better, like this we will have a quick help of knowledge well elaborated.*

<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/tks.png" class="center">

by:

<img src="https://github.com/weslen02/git-quick-help-to-start/blob/master/img/assWeslen2.png" class="center">

> A good **knowledge** is **shared knowledge**!
