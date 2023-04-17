## generer une cle ssh 
    $ ssh-keygen -t rsa -C "MOHAMMED YASSINE"    <!-- -t : type rsa:l'algrithme de cyptage -->

    Enter passphrase (empty for no passphrase): //passphrase est cache
    Enter same passphrase again: //passphrase est cache il faut le rappeler
## recuperer id & public key 
    Your identification has been saved in /c/Users/Lenovo/.ssh/id_rsa // arborescence
    Your public key has been saved in /c/Users/Lenovo/.ssh/id_rsa.pub // arborescence


    $ cat /c/Users/Lenovo/.ssh/id_rsa.pub // cat affiche le contenu d'un fichier 
## verifier la connection avec le depot distant via SSH
    ssh -T git@github.com
    



