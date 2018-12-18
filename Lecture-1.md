This tutorial has following sections:
- Git
- GitHub
- Using Git
- Homework
- Useful links

# 1. Git : 

## 1.1 What is Git, Etymology and a short history.
* [Version Control](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control) (aka Revision control, source control, Distributed version control system)
* [SVN vs git](https://svnvsgit.com/)

## 1.2 Installing Git
 For a RedHat based Linux (Like CentOS)
```
 sudo yum install git
```

 For a Debian based Linux (like Ubuntu)
```
 sudo apt-get install git 
```

 For a MAC, open Terminal and execute following command
```
 brew install git
```
## 1.3 Install Git autocomplete

# 2. GitHub: 

## 2.1 What is GitHub 
 GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

 Registering/Creating the account on GitHub
 You need
* A valid Email address
* An SSH key-pair


## 2.2 Generating the ssh keypair

 For Linux/MAC, use
```
ssh-keygen -C "username@email.com" -t rsa
```

Supply your Github email address instead of this fake one. 
Accept the default location storage (default file) for the keys. When prompted for a passphrase, make up one, and don't forget it ! This is your private key, do not share it with anyone.
You will have `id_rsa` and `id_rsa.pub` files in the directory at the following path `/Users/<your_user_name>/.ssh/`

 You want to copy the contents of the id\_rsa.pub (open it with a simple text editor or use the command cat in the Bash)
 After you copy the contents of the id\_rsa.pub file, Go to the GitHub account, go to the settings find SSH and GPG keys option and add New SSH key.

## 2.3 [Global config](https://www.git-scm.com/book/en/v2/Customizing-Git-Git-Configuration)

 configure your email and username of Github in the git
 ```
$git config --global user.email "username@email.com"
$git config --global user.name "username"
```
The username does not have to be same as your GitHub username.

## 2.4 Creating a repository

Using your GitHub account, create a repository to which you can add files. 
Name the repository as hello-world. 
Create a public repository and check the box to create a README file. 
After you created the repository, the URL of your web page would be something like https://github.com/$username/hello-world.git . 

# 3. [Using Git](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository)

## 3.1 Creating the repository
```
Create a new directory in your home directory or any other suitable location using
$mkdir hello-world
Enter it
$cd hello-world
and create a new git repository using 
$git init
```

You can clone a repository with `git clone <URL>` command. This copies the repository from a remote machine and initializes it on your machine. You can try to clone some public repositories on github.com


## 3.2 Workflow
 Working Directory -> Index -> HEAD
 your local repository consists of three "trees" maintained by git. 
 the first one is your Working Directory which holds the actual files. 
 the second one is the Index which acts as a staging area and finally the HEAD which points to the last commit you've made.


## 3.3 Add and commit
```
 #You can propose changes (add it to the Index) using
 $git add <filename>
 #This is the first step in the basic git workflow.
 
 #To actually commit these changes use
 $git commit -m "Commit message"
```

## 3.4 Pushing changes
```
#If you have not cloned (Our case) an existing repository and want to connect your repository to a remote server, you need to add it with

$git remote add origin https://github.com/$username/hello-world.git
Replace the URL with the repository you created in step 2.3

 Now you are able to push your changes to the selected remote server i.e. your remote repository on GitHub.
 Your changes are now in the HEAD of your local working copy. To send those changes to your remote repository, execute 
 $git push -u origin master
```

# 4. Homework
- Get practice with [katacoda](https://www.katacoda.com/courses/git)

