### todo
- régler le pb gulp EBUSY
  + gulp Error: EBUSY, open 
- all done guy !!!

##r sauvegarde sur clef usb

- sur la clef
  + git clone --bar ~/le/projet/git/a/cloner
- sur master (PC-A)
  + git remote add origin e:/portail
  + git st ok (add -A & git co -m "com")
  + git push origin master
- supp remote si boulette
  + git remote rm origin

### nettoyage du cache .gitignore
- git rm -r --cached
  + archiver tous les fichier Ã  conserver
  + supprime tous de l'index
- git add .
  + reimporte tout dans l'index (.gitignore est pris en compte)
- git co -m ".gitignore est maintenant fctlle"
  + archiver (pour supprimer tous ce qui est ignorÃ©)
 
### revenir sur un commit
- sur le dernier commit
  + git commit --amend
- revenir sur un vieux commit
  + git rebase -i @~9
    * reviens sur les 9 derniers commit
    * dans vim se plcer sur le commit Ã  modifier :
    * ctrl+w pour changer de fenetre, i pour inserer caracter
  + passer la ligne de pick Ã  e (edit)
  + enrg depuis vim> :wq
  + modifier le commit 
    * git commit --amend
  + valider le commit
    * git rebase --continue
  + une fois corrigÃ© :
    * git push --force origin master

function alertFct(e){
  e.target.href = 'javascript:void(0)';
  console.log(e.target.getAttribute("onclick"));
  
}
if(addEventListener)
  window.addEventListener('click',alertFct,false)
else
  window.attachEvent('onclick', alertFct)
