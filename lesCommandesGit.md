# les commandes linux de bases 
 ## ls 
    sert a afficher les dossiers et les fichiers du repertoire pointe
  les options :
    -r : affichera non seulement les fichiers et dossiers du répertoire actuel, mais aussi de tous les sous-répertoires inclus dans le    répertoire actuel.
    -l : pour afficher les fichiers et les répertoires sous forme détaillée
    -a : pour afficher les dossies caches
 ## rm 
    sert a suprimer les fichiers et les repertoires .
    Pour les fichiers il faut ajout les deux options suivant :
    -r 
    -f : forcer la supression sans  demander de confirmation, même s'il est protégé contre l'écriture ou s'il contient des fichiers en lecture seule. 
# les commandes Git      
 ## git add 
    -git add : sert a ajouter le fichier a Staging area 
    -git add . pour ajouter tous les fichiers .
 ## git add *.ext
    sert a ajouter touts les fichier de ext x
        exp : git add *.html
 ## git       
 ## git commit -am " message"
    si le fichier est deja tracker, cette methode marche bien  (deconseiller)
 ## git ls-files 
    sert a afficher les fichiers tracker
 ## git restore --staged <files>  
    pour supprier un track   
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
 ## Creer un tag
    git tag <tag name>      
 ## liste des tags 
    git tag --list 
 ## Supprimer un tage 
    git tag -d <tag name >  
 ## Retourner en arriere (Reset)
    git reset <id>  --soft    (logique)
    git reset <physique> -- hard (physique)
 ## Visualiser historique en cad de reset hard 
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
            git push -u origin main
 ## Afficher les repos distants
    git remote -v
