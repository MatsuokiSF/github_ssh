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
 
 git remote add origin 'repository-url'
 
 **Si deseas realizar un push el procedimiento es el siguiente**
  #Te ubicas en la ruta del proyecto. ej: cd /Users/mainuser/Desktop/Projects
 $ git status
  #Agregar los archivos donde se realizaron los cambios
 $ git add INFO241_tarea1/ Unidad\ 3\ _\ Tarea\ 1.pdf
 
 $ git commit -m 'Some message about the change'

 $ git push origin 'branch-name'
