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

## Les contrôleurs
- Les contrôleurs Web Spring sont conçus pour gérer et répondre aux requêtes HTTP


## architecture de Spring Data.

- Architecture contrôleur-référentiel
- Le référentiel est l'interface entre l'application et la base de données et fournit une abstraction commune pour toute base de données, facilitant ainsi le passage à une autre base de données en cas de besoin.

## Idempotente 
- Le terme "idempotence" fait référence à une propriété dans laquelle une opération ou une fonction produit le même résultat, peu importe combien de fois elle est appliquée. En d'autres termes, si une opération idempotente est exécutée plusieurs fois, le résultat final sera le même que si elle avait été exécutée une seule fois.

- Dans le contexte des services web ou des API, l'idempotence signifie que l'appel à une même requête ou à une même action multiple fois ne produira pas d'effets secondaires indésirables ou de changements supplémentaires. Cela permet de garantir la cohérence et la prévisibilité des opérations, même en cas de répétition.

- Par exemple, si une requête de création (POST) est idempotente, cela signifie que vous pouvez l'appeler plusieurs fois avec les mêmes paramètres sans créer plusieurs fois la même ressource. Chaque appel supplémentaire aura le même effet que le premier, c'est-à-dire créer la ressource une seule fois.

- Il convient de noter que toutes les opérations ou fonctions ne sont pas idempotentes par nature, et cette propriété doit être conçue et mise en œuvre spécifiquement pour chaque cas d'utilisation.


## spring api
- REST (Representational State Transfer) est un style d'architecture logicielle utilisé pour concevoir des services web. Il repose sur le protocole HTTP (Hypertext Transfer Protocol) et définit un ensemble de contraintes et de principes pour la création d'interfaces web simples, évolutives et interopérables. Les services RESTful permettent aux clients d'accéder et de manipuler des ressources en utilisant des opérations standardisées telles que GET, POST, PUT et DELETE. Cela facilite l'intégration et l'interaction entre différentes applications et plateformes.



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

## Les contrôleurs
- Les contrôleurs Web Spring sont conçus pour gérer et répondre aux requêtes HTTP


## architecture de Spring Data.

- Architecture contrôleur-référentiel
- Le référentiel est l'interface entre l'application et la base de données et fournit une abstraction commune pour toute base de données, facilitant ainsi le passage à une autre base de données en cas de besoin.


## Idempotente 
- Le terme "idempotence" fait référence à une propriété dans laquelle une opération ou une fonction produit le même résultat, peu importe combien de fois elle est appliquée. En d'autres termes, si une opération idempotente est exécutée plusieurs fois, le résultat final sera le même que si elle avait été exécutée une seule fois.

- Dans le contexte des services web ou des API, l'idempotence signifie que l'appel à une même requête ou à une même action multiple fois ne produira pas d'effets secondaires indésirables ou de changements supplémentaires. Cela permet de garantir la cohérence et la prévisibilité des opérations, même en cas de répétition.

- Par exemple, si une requête de création (POST) est idempotente, cela signifie que vous pouvez l'appeler plusieurs fois avec les mêmes paramètres sans créer plusieurs fois la même ressource. Chaque appel supplémentaire aura le même effet que le premier, c'est-à-dire créer la ressource une seule fois.

- Il convient de noter que toutes les opérations ou fonctions ne sont pas idempotentes par nature, et cette propriété doit être conçue et mise en œuvre spécifiquement pour chaque cas d'utilisation.





## Le corps de la requête
Lorsque nous suivons les conventions REST pour créer ou mettre à jour une ressource, nous devons soumettre des données à l'API. C'est ce qu'on appelle souvent le corps de la demande . Les opérations CREATEet UPDATEnécessitent qu'un corps de requête contienne les données nécessaires pour créer ou mettre à jour correctement la ressource. Par exemple, une nouvelle carte de paiement peut avoir un montant initial en espèces et une UPDATEopération peut modifier ce montant.

## Put et Patch
- Les deux PUTet PATCHpeuvent être utilisés pour la mise à jour, mais ils fonctionnent de différentes manières. Essentiellement, PUTcela signifie « créer ou remplacer l'enregistrement complet », alors que PATCHcela signifie « mettre à jour seulement certains champs de l'enregistrement existant » - en d'autres termes, une mise à jour partielle.
 
- Pourquoi voudriez-vous faire une mise à jour partielle ? Les mises à jour partielles évitent au client d'avoir à charger l'intégralité de l'enregistrement, puis de renvoyer l'intégralité de l'enregistrement au serveur. Si l'enregistrement est suffisamment volumineux, cela peut avoir un impact non négligeable sur les performances.

## PUT et POST

En général, dans le contexte des communications en ligne, la principale différence entre un "PUT" et un "POST" réside dans leur utilisation et leur intention.

- "POST" est une méthode HTTP utilisée pour envoyer des données à un serveur afin de créer une nouvelle ressource. Lorsque vous effectuez un "POST", vous envoyez des données au serveur pour qu'il les enregistre et crée une nouvelle entité.

- "PUT", en revanche, est une méthode HTTP utilisée pour mettre à jour une ressource existante sur le serveur. Lorsque vous effectuez un "PUT", vous envoyez des données au serveur pour qu'il mette à jour une entité déjà existante avec les nouvelles informations fournies.

En résumé, "POST" est utilisé pour créer de nouvelles ressources, tandis que "PUT" est utilisé pour mettre à jour des ressources existantes.


