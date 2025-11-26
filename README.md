# Connaitre la version actuellement installé sur l'ordinateur

    git --version                                                     
# Mettre a jour git sur windows : https://go.lightnode.com/fr/tech/how-to-check-and-update-git-version

    git update-git-for-windows         
ou         

    git update   
# Configurer le user en global dans sa configuration git 

    git config --global user.name "Darkzveller"
et 
   
    git config --global user.email "jsp@gmail.com"
# Affiche le name et l'email enregistré

    git config --list
    
# Permet d'écrire de long nom de fichier/dossier

    git config --global core.longpaths true 

# Permet d'envoyer de plus grosse donnée sur github

    git config --global http.postBuffer 524288000

#Stocker ton identifiant et token en clair dans ~/.git-credentials, pour avoir accès aux projets privés de ses congéneres

    git config --global credential.helper store           

ou  Dans le trousseau GNOME (Ubuntu / Debian / WSL)

    git config --global credential.helper libsecret

# Connaitre le contenu du token

Pour connaitre le contenu du token qui doit etre de la forme https://nom_utilisateur:ton_token@github.com le dossier n'existe pas pear défaut, donc il faut le créer sois meme au début en faisant  

    cat ~/.git-credentials                                           

et
    
    nano ~/.git-credentials  

# Permettre la création par défaut d'une branch main et non master

    git config --global init.defaultBranch main 


# Supprimer la configuration Git globale

## Sous linux debian
        
    rm ~/.gitconfig

## Sous windows 

- Aller dans C:\Users\<TON_UTILISATEUR>\.gitconfig
- Supprimer le dossier .gitconfig ou le contenu

