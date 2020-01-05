# SNT-Todo-list  
-----------------------------------------  
# Pré-requis  
rendez vous sur le fichier de base : [trinket](https://trinket.io/html/c9641e2773)  
-----------------------------------------
# Etape 1 : Créer des actions pour les boutons  
Le code de base inclu 3 fichiers (sous la forme de 3 onglets) :  
* _index.html_ - le squelette de la page  
* _style.css_ - le fichier de style de votre page  
* _script.js_ - le fichier pour le javascript  
-------------------------------------------
Le squelette et le style ayant été préparés pour vous, vous allez surtout interagir avec _script.js_ .  
vous avez 4 boutons : _Add_,_Clear Completed_,_Empty List_;_Save List_.  
La première chose à faire est de relier les boutons au script. 
ajoutez le code suivant à votre script  
![image](https://github.com/Svt-lim/SNT-Todo-list/blob/master/to%20do%20list%20images/1-addbutton.jpg)  
avec ce code vous avez :  
* créez une variable qui a le nom de votre bouton  
* Liez votre variable à l'élément HTML "add-button"  
il faut maintenant que votre variable soit liée à une fonction qui se déclenchera quand on cliquera sur le bouton.  
ajoutez le code suivant apres votre variable  
![image](https://github.com/Svt-lim/SNT-Todo-list/blob/master/to%20do%20list%20images/2-listen%20to%20click.jpg)  
Vous avez :  
* la fonction `addEventListener` attend un click sur votre variable addButton  
* Quand le click arrive, cela lance la fonction `addToDoItem` (fonction que vous n'avez pas encore écrite)  

* ajouter le code suivant à votre script : 
`function addToDoItem(){    
  alert("Clic reussi!");  
}`  
-------------------------------------------
# Défi 1 : écrire le code pour les 3 autres boutons.  
* liez le bouton _Clear Completed_ qui a l'Id *clear-completed-button* à une fonction *clearCompletedToDoItems*  
* liez le bouton _Empty List_ qui a l'Id *empty-button* à une fonction *emptyList*  
* liez le bouton _Save List_ qui a l'Id *save-button* à une fonction *saveList*  
-------------------------------------------  
# Etape 2 : Ajouter des évenements à la liste :  
il s'agit maintenant de faire fonctionner les boutons correctement.  
## Les listes en HTML  
Vous allez utliser un peu d'HTML ici. Dans notre cas, pour manipuler les listes, il y a deux balises : `<ol>` quand la liste est ordonnée (i.e. numérotée) et `<li>` pour identifier individuellement les listes. la balise `<ol>` est déjà placée correctement dans la page HTML, il vous suffit d'écrire une fonction pour que l'utilisateur puisse créer des listes.  
## Défi 2 : Création de deux variables toDoEntryBox et toDoList  
en vous inspirant du défi 1, ajoutez à votre code les deux variables du défi pour les lier à leur Id respectif:  
* toDoEntryBox : Id = todo-entry-box
* toDoList     : Id = todo-list  
ajoutez la fonction suivante pour permettre la création d'une liste  
![image](https://github.com/Svt-lim/SNT-Todo-list/blob/master/to%20do%20list%20images/4-list.jpg)  
## Lier le bouton à l'action.  
modifier votre fonction addToDoItem() comme suit:  
![image](https://github.com/Svt-lim/SNT-Todo-list/blob/master/to%20do%20list%20images/5-list.jpg)  
# Etape 3 : Marquer les choses à faire comme étant fait  
Pour permettre de déclarer une élément comme étant fini il faut une fonction qui fasse le tri entre les éléments "complétés" et ceux qui ne le sont pas encore.  
ajouter le code suivant:  
![image](https://github.com/Svt-lim/SNT-Todo-list/blob/master/to%20do%20list%20images/6-this.jpg)  
# Etape 4 : enlever des éléments de la liste.  
il y a 2 boutons non exploités, "Clear Completed" et "Empty list", prévus pour cette étape.  
la notion de boucle conditionnelle en javascript n'étant pas au programme de SNT vous allez faire un peu de [culte du cargo](https://fr.wikipedia.org/wiki/Culte_du_cargo#En_informatique) en modifiant votre fonction `clearCompletedToDoItems()` de l'étape 1 grace à ce bloc de code:  
![image](https://github.com/Svt-lim/SNT-Todo-list/blob/master/to%20do%20list%20images/7-remove.jpg)  
puis modifiez la fonction `emptylist()` avec ce bloc ci :  
![image](https://github.com/Svt-lim/SNT-Todo-list/blob/master/to%20do%20list%20images/8-remove.jpg)  
# Etape 5 : Sauver ses listes.  
pour sauver une liste il faut la stocker dans la mémoire de l'ordinateur. En JavaScript, on appelle cette "case" un array et cela est symabolisé par des [].  
modifiez votrz fonction `saveList` comme suit :  
![image](https://github.com/Svt-lim/SNT-Todo-list/blob/master/to%20do%20list%20images/11-savethelist.jpg)  






  


