# github_ssh_remember
Notes_ssh_git-linux_remember
#Biblio -> https://tutorials.codebar.io/version-control/set-up/tutorial.html

breaks Code (Block):
git config --global user.name "Your Name"
git config --global user.email "name@domain"

 ls -al ~/.ssh
 
 ssh-keygen -t rsa -b 4096 -C "your_email@here.com"
 
 eval "$(ssh-agent -s)"
 
 ssh-add ~/.ssh/id_rsa
 
 ssh-add -l
 
 #
 pbcopy < ~/.ssh/id_rsa.pub
 #Copy this on github ->> settings ->> SSH and GPG Key ->> "Add title" and Paste on Key
 
 ssh -T git@github.com
 
 git clone "SSH"
 
 git remote add origin <repository-url>
