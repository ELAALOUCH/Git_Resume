
# les commandes Git      
 ## git add 
    -git add : sert a ajouter le fichier a Staging area 
    -git add . pour ajouter tous les fichiers .
 ## git add *.ext
    sert a ajouter touts les fichier de ext x
        exp : git add *.html
 ## git       
 ## git ls-files 
    sert a afficher les fichiers tracker
 ## git restore --staged <files>  
    pour supprimer un track   
 ## pour supprimer une modification dans working repo 
    git restore <file name >  
 ## Creer une Branche 
    git branch <branch name>
 ## Changer la branche 
    git checkout <branch name>
 ## Supprimer une branche 
    git branch -d <branch name>  
 ## La liste des branches 
    git branch 
 ## afficher l'historique (log)
    git log 
    git show 
       -> git log --oneline
 ## Creer un tag
    git tag <tag name> <branch name : fucultatif>   // on peut specifier le tage pour la branche  
       -> git show <le nom de tag > pour visualiser le code de tag     
 ## liste des tags 
    git tag --list 
 ## Supprimer un tage 
    git tag -d <tag name >  
 ## Retourner en arriere (Reset) 
    git reset  --hard  id (physique)
 ## Visualiser historique en cas de reset hard 
    git reflog 
 ## les commandes de la liaison entre git et github est donne par github
      …or create a new repository on the command line
            echo "# tttt" >> README.md
            git init
            git add README.md
            git commit -m "first commit"
            git branch -M main
            git remote add origin git@github.com:ELAALOUCH/tttt.git
            git push -u origin main
      …or push an existing repository from the command line
            git remote add origin <git@github.com:ELAALOUCH/tttt.git>
            git branch -M main
            git push -u origin main.
 ## Afficher les repos distants
    git remote -v
 ## envoyer le dipot local a github 
    git push -u origin master (main)
 ## configurer push par default 
    git config --global push.default simple
       ----> git push 
    or  git push --set-upstream origin dev     
   
   ### NB:
     impossible de pusher le depot si les deux depots sont diffs (ils doivent etre identiques)
     avant de faire pusher il faut faire le pull 
 ## Pull & fetch
     git pull 
     
     pull = fetch + merge

 ## changer remote repot 
     git remote set-url origin <remote url>  
 ## supprimer qlq chose de distant en local 
     git push origin :<branch par exemple >
     : sert  a supprimer
 ## commit + close issue
     git commit -m "message , close <#id_issue>  " 
#GitFlow
  ## initialiser GitFlow 
     git flow init
  ## creation d'une nouvelle fonctionnalite
     git flow feature start <feature name> 
  ## feature finish and merge to develop branch 
     git flow feature finish <feature name> 
 
