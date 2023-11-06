## spring api

1- La désérialisation est le processus inverse de la sérialisation. Il transforme les données d'un fichier ou d'un flux d'octets en un objet pour votre application. 

. La sérialisation et la désérialisation fonctionnent ensemble pour transformer/recréer des objets de données vers/depuis un format portable. Le format de données le plus populaire pour la sérialisation des données est JSON.

2-  Le but d’une API RESTful (Application Programming Interface) est de gérer l’état de ces Ressources.
on considère « l'état » comme une « valeur » et la « représentation de la ressource » comme un « objet » ou une « chose ». Par conséquent, REST n’est qu’un moyen de gérer les valeurs des choses. Ces éléments sont accessibles via une API et sont souvent stockés dans un magasin de données persistant, tel qu'une base de données.

3- CRUD  « Créer, lire, mettre à jour et supprimer ».

4- Les composants de la demande et de la réponse sont :

Demande

Méthode (également appelée Verbe)
URI (également appelé point de terminaison)
Corps
Réponse

Code d'état
Corps
Si vous souhaitez approfondir les méthodes de requête et de réponse, consultez la norme HTTP .

La puissance de REST réside dans la façon dont il fait référence à une ressource et à quoi ressemblent la demande et la réponse pour chaque opération CRUD. Jetons un coup d'œil à ce à quoi ressemblera notre API lorsque nous aurons terminé ce cours :
For CREATE: use HTTP method POST.
For READ: use HTTP method GET.
For UPDATE: use HTTP method PUT.
For DELETE: use HTTP method DELETE.


Le tableau ci-dessous contient plus de détails sur les opérations RESTful CRUD.

Opération	  Point de terminaison de l'API	   Méthode HTTP	   Statut de la réponse
Créer	      /cashcards	                   POST	           201 (CRÉÉ)
Lire	      /cashcards/{id}	               GET	           200 (D'accord)
Mise à jour	  /cashcards/{id}	               PUT	           204 (PAS DE DONNÉES)
Supprimer	  /cashcards/{id}	               DELETE	       204 (PAS DE DONNÉES)





Operation	   API Endpoint	HTTP         Method	         Response Status
Create	       /cashcards	             POST	         201 (CREATED)
Read	       /cashcards/{id}	         GET	         200 (OK)
Update	       /cashcards/{id}	         PUT	         204 (NO DATA)
Delete	       /cashcards/{id}	         DELETE	         204 (NO DATA)





## Le corps de la requête
Lorsque nous suivons les conventions REST pour créer ou mettre à jour une ressource, nous devons soumettre des données à l'API. C'est ce qu'on appelle souvent le corps de la demande . Les opérations CREATEet UPDATEnécessitent qu'un corps de requête contienne les données nécessaires pour créer ou mettre à jour correctement la ressource. Par exemple, une nouvelle carte de paiement peut avoir un montant initial en espèces et une UPDATEopération peut modifier ce montant.