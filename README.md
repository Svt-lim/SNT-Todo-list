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
  

ajouter le code suivant à votre script : 
`function addToDoItem() {  
  alert("Clic reussi!");  
}`  

