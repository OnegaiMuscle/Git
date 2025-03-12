Version de Windows :
- Appuyer sur `Windows` + `R`
- Saisir `winver`
- Appuyer sur `Enter`

Windows Update :
- Appuyer sur `Windows` + `R`
- Saisir `ms-settings:windowsupdate`
- Appuyer sur `Enter`
- Cliquer sur « Rechercher les mises à jour »

ou
- Appuyer sur `Windows` + `R`
- Saisir `services.msc`
- Appuyer sur `Enter`
- Double-cliquer sur `Windows Update Service`
- Définir `Startup` sur `Automatic`
- Cliquer sur `Start`
- Cliquer sur `Ok`

Virtualisation :
- Appuyer sur `Windows` + `R`
- Saisir `taskmgr`
- Appuyer sur `Enter`
- Cliquer sur l’onglet `Performance`
- Cliquer sur `CPU`

Windows sous Linux (WSL) :

:warning: Dans les instructions suivantes, utiliser la combinaison de touches `Ctrl` + `Shift` + `Enter` pour exécuter **Windows Terminal** en tant qu’administrateur au lieu de cliquer simplement sur `Ok` ou d’appuyer sur `Enter`

- Appuyer sur `Windows` + `R`
- Saisir `wt`
- Appuyer sur **`Ctrl` + `Shift` + `Enter`**

:warning: Accepter la confirmation UAC concernant l’octroi des droits d’administrateur

Une fenêtre de terminal apparaîtra :
- Copier la commande suivante et la coller dans la fenêtre du terminal
- appuyer sur `Enter`

```
wsl --install
```
- Après avoir redémarré l'ordinateur, une fenêtre de terminal indique que WSL poursuit le processus d'installation d'Ubuntu. Lorsque c'est terminé, Ubuntu va se lancer

Ubuntu Premier Lancement :
- Choisir un **nom d’utilisateur** :
  - un mot
  - en minuscules
  - sans caractères spéciaux
  - par exemple : `jarvis` ou ton `prenom`
- Choisir un **mot de passe**
- Confirmer ton mot de passe

:warning: Lors de la saisie du mot de passe, rien ne s’affichera à l’écran ; **c’est normal**. Il s’agit d’une mesure de sécurité permettant de masquer ton mot de passe et sa longueur
- Saisir simplement ton mot de passe, puis appuyer sur `Enter`
- Bien se souvenir de son mot de passe, il sera demandé lors de chaque commande administrateur
- Ubuntu est installée sur l'ordinateur, la fenêtre de Terminal peut être fermée

Vérifier la version de WSL sous Ubuntu :
- Appuyer sur `Windows` + `R`
- Saisir `cmd`
- Appuyer sur `Enter`
Saisir la commande suivante :

```bash
wsl -l -v
```
:heavy_check_mark: Si la version de WSL sous Ubuntu est la 2, c’est bon

Vérifier que la locale soit bien en **anglais** dans le terminal :

```
locale
```
Si la commande ne renvoie pas quelque chose qui contient `LANG=en_US.UTF-8`, lancer ceci dans un terminal Ubuntu :

```
sudo locale-gen en_US.UTF-8
```
Si après, un avertissement apparait (`bash: warning: setlocale: LC_ALL: cannot change locale (en_US.utf-8)`) dans le terminal, exécuter ces lignes dans le terminal
  
```
sudo update-locale LANG=en_US.UTF8
sudo apt-get update
sudo apt-get install language-pack-en language-pack-en-base manpages
```
Fermer la fenêtre de terminal


