Depuis le tutoriel de : 
https://readwrite.com/2013/09/30/understanding-github-a-journey-for-beginners-part-1/


Il s'agit d'une explication pour utiliser github et github

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


problèmes :
Si vous avez un conflit de push-forward car il y a eu une modification sur internet :
git pull --rebase origin master