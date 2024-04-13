Se mettre dans le répertoire du projet
```bash
cd ~/code/$YOURGITHUBNICKNAME/$YOURPROJECTNAME
```
Création du dépôt GitHub
```bash
git init
git add .
git commit -m "first commit"
```
Puis mode interactif
```bash
gh repo create
```
ou préconfiguré
```bash
gh repo create --public --source=.
```
puis push sur branche gh-pages
```bash
git co -b gh-pages
git push origin gh-pages
```
ton site web statique se trouvera sur
```bash
http://$YOURGITHUBNICKNAME.github.io/$YOURPROJECTNAME/
```
