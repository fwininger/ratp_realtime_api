Documentation de l'API Real Time de la RATP
===================

Bonjour ! La RATP publie dans le cadre de l'Open Data les horaires de l'ensemble des lignes sur le site http://data.ratp.fr/. Cependant l'accès aux données temps réel disponible via l'API utiliser par l'application mobile par exemple reste mal documenté pour les utilisateurs finaux.

Ce dépôt permet fourni l'ensemble de la documentation nécessaire pour utiliser l'API temps réel.

----------

Spécifications de l'API
-------------

L'api temps réel de la RATP est disponible via l'url suivante :

> http://apixha.ixxi.net/APIX

(l'url offre une documentation minimaliste)

La clé d'Api est la suivante :

> FvChCBnSetVgTKk324rO

L'api fourni une réponse XML au requête par défaut. Il est possible d'ajouter une paramètre `apixFormat=json` pour utiliser un format JSON plus facile à utiliser dans de nombreux contextes.

Exemple de requête pour avoir les horaires de la station Châtelet :

> http://apixha.ixxi.net/APIX?keyapp=FvChCBnSetVgTKk324rO&cmd=getNextStopsRealtime&stopArea=7&apixFormat=json

----------

Liens utiles
-------------
Une api est également disponible pour les lignes gérées par la SNCF :
> http://monrer.fr
> https://ressources.data.sncf.com
