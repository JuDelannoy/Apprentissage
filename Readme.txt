Depuis le tutoriel de : 
https://readwrite.com/2013/09/30/understanding-github-a-journey-for-beginners-part-1/


Il s'agit d'une explication pour utiliser github et github

CREATION DOSSIER (non existant sur web et existant en local)

- ouvrir le bash git dans le bon dossier (repository)
- si repository git non créé: git init
- information sur le statut : git status
- on ajoute le fichier modifié : git add Readme.txt
- on enregistre une copie instantané : git commit -m "Ajout Lisez-moi.txt"

astuce : si le fichier a déjà été ajouté à l'index on peut condenser ces deux étapes :
- on met à jour le fichier et on en enregistre une copie instantané : git commit -a -m "Ajout Lisez-moi.txt"


on push ce qu'on a modifié en local sur github.com : 
- si on n'a pas encore fait le lien : 
	git remote add origin https://github.com/username/myproject.git
	git remote -v (to confirm)
- git push ou git push --set-upstream origin master (master étant la branche principale)
Maintenant tout se trouve sur votre github !!!


RECUPERATION DOSSIER (existant sur github mais pas en local)
- git init
- git clone git://git.renater.fr/nom_projet.git pour récupérer le dossier
- Ensuite on peut faire les modifications en local puis les ajoutr, commiter et pousser.


PROBLEMES :
Si vous avez un conflit de push-forward car il y a eu une modification sur internet :
git pull --rebase origin master


