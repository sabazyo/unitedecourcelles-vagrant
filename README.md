# Utilisation de vagrant
## Installation
### Windows

Il faut installer virtualbox trouvable ici -> https://www.virtualbox.org/wiki/Downloads
Ensuite il faut installer vagrantup trouvable ici -> http://www.vagrantup.com/downloads.html

Une fois que les 2 programmes sont installer il faut ouvrir un cmd.exe et verifier que cette ligne renvoie une reponse : 

``` vagrant version ```

Si cette ligne marche on va installer 2 plugins pour vagrant : 

``` vagrant plugin install vagrant-hostmanager ``` 

```  vagrant plugin install vagrant-vbguest ```

Une fois fais on peut cloner ce depot dans un dossier de notre choix, dans ce dossier il faudre cloner dépot unitedecourcelles
dans le dossier unitedecourcelles avec le branch dev

Ensuite on peut lancer dans le dossier ou on a cloner unitedecourcelles-vagrant (il doit avoir le fichier Vagrantfile) :

```  vagrant up ```
Attention la derniere commande permet de démarer la vm avec le projet MAIS sous windows la premiere fois il faut la
lancer en tant que admin.

Pour arreter la vm : 

```  vagrant halt ```

Pour se connecter en ssh à la vm : 

```  vagrant ssh ```

* Le projet sera accesible a cette adresse : http://unitedecourcelles.dev
* La gestion des table mysql avec l'user root et le mots de passe rootme est la : http://192.168.56.201/adminer
* Pour voire les mail que l'on envoie est la : http://192.168.56.201:1080

