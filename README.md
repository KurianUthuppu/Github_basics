# Github_basics
_Capturing the basics of Github including setup and sync_


### Basic requirements
* Git
  - Download Git from this link https://git-scm.com/downloads and install as per the guidelines
* Visual Studio
  - Download and install visual studio code editor from https://visualstudio.microsoft.com/downloads/

### Resources
* Useful youtube video from freeCodeCamp.org - https://youtu.be/RGOj5yH7evk

### Setting up your account in Github
- This is relatively simple and straightforward once you arrive at https://github.com/
- You may either refer to the above youtube video or use this link https://docs.github.com/en/get-started/onboarding/getting-started-with-your-github-account for further guidance

### Setting up your profile
- Select 'Your Profile' in the menu that pops up after clicking the top-right corner profile image
- Add relevant details along with a 'dashing photo' of yours! :wink:

### Cheat code for creating profile page
(Ref: https://aboutmonica.com/blog/how-to-create-a-github-profile-readme/)
* Create a new repository with the same name (including casing) as your GitHub username
* Create a README.md file inside the new repo with content (text, GIFs, images, emojis, etc.)
* Commit your fancy new README!
  - If you're on GitHub's web interface you can choose to commit directly to the repo's main branch (i.e., master or main) which will make it immediately visible on your profile)
  - Push changes to GitHub (if you made changes locally i.e., on your computer and not github.com)

### Creating SSH (Secure Shell) key and upload to github
- Create public/private keys using the below command which delineates the requisite encryption format and encryption strength
- ssh-keygen -t rsa -b 4096 -C “email-id” (Registered email-id as given in github)
- The public/private key is generated in files with default name - id_rsa.pub & id_rsa
- Click profile image on github page on top right-corner, click settings -> SSH & GPG keys -> New SSH key
- Copy, paste the public key starting with 'ssh-rsa' in the above tab and save
- Open github bash terminal & initiate ssh agent using coomand -> eval "$(ssh-agent -s)"
- Add private key to the ssh agent in local machine using the command -> ssh-add ~/.ssh/id_rsa

### Creating a repo and github and cloing to local machine
- Click 'new' on top left-corner of your github homepage
- Give the requisite details including repo-name, public/private etc:-
- Include readme file to the same and create the repo
- Open git command terminal and go the requisite folder where you want to clone the repo from github
- Clone the repo using the command - git clone <ssh key> (You can get the ssh key of the respective folder by pressing the green button labelled 'Code' inside each repo)
  

