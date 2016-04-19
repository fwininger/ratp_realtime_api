Perturbations
===================

La méthode `getTrafficSituation` permet de récupérer les informations d'incident sur les lignes.

Paramètres
-------------

Obtenir les informations sur les différents groupes de lignes (métro, rer, tram...)
- `&networktype=groupoflines&network=1`

Obtenir les informations sur les différentes lignes individuellements
- `&networktype=line&network=1`


Exemples
-------------

**Les incidents sur l'ensemble des lignes de métro :**

> http://apixha.ixxi.net/APIX?keyapp=FvChCBnSetVgTKk324rO&cmd=getTrafficSituation&networktype=groupoflines&network=1&apixFormat=json

**Résultat :**
```json
{
	"events": [{
		"eventId": 53582,
		"startDate": "2016-05-20T00:00:00+02:00",
		"endDate": "2017-08-01T01:15:00+02:00",
		"startTime": "0000",
		"endTime": "0000",
		"type": "miscellaneousReason",
		"typeName": null,
		"cause": null,
		"description": null,
		"incidents": [{
			"incidentId": 136375,
			"description": "À partir du vendredi 20 mai 2016, tous les jours en raison de travaux, la station Chateau Rouge sera fermée sur la ligne 4 du Métro jusqu'au lundi 31 juillet 2017.",
			"lines": [{
				"id": 10,
				"codeStif": null,
				"message": "À partir du vendredi 20 mai 2016, tous les jours en raison de travaux, la station Chateau Rouge sera fermée sur la ligne 4 du Métro jusqu'au lundi 31 juillet 2017.",
				"shortMessage": "(M 4) du 20/05/16, Ts les jours la station Chateau Rouge sera fermée jusqu'au 31/07/17. (travaux)",
				"incidentSeverity": "medium",
				"consequence": null,
				"stopPoints": [12794],
				"stopPointsName": []
			}]
		}]
	}, {
		"eventId": 53272,
		"startDate": "2016-04-11T00:00:00+02:00",
		"endDate": "2016-07-01T01:15:00+02:00",
		"startTime": "0000",
		"endTime": "0000",
		"type": "miscellaneousReason",
		"typeName": null,
		"cause": null,
		"description": null,
		"incidents": [{
			"incidentId": 135491,
			"description": "À partir du lundi 11 avril 2016, tous les jours suite à des travaux de rénovation, l'arrêt n'est pas marqué à la station Concorde sur la ligne 8 du Métro jusqu'au jeudi 30 juin 2016.",
			"lines": [{
				"id": 15,
				"codeStif": null,
				"message": "À partir du lundi 11 avril 2016, tous les jours suite à des travaux de rénovation, l'arrêt n'est pas marqué à la station Concorde sur la ligne 8 du Métro jusqu'au jeudi 30 juin 2016.",
				"shortMessage": "(M 8) du 11/04/16, Ts les jours l'arrêt n'est pas marqué à Concorde jusqu'au 30/06/16. (travaux de rénovation)",
				"incidentSeverity": "medium",
				"consequence": null,
				"stopPoints": [12904],
				"stopPointsName": []
			}]
		}]
	}, {
		"eventId": 53271,
		"startDate": "2016-04-07T00:00:00+02:00",
		"endDate": "2016-07-01T01:15:00+02:00",
		"startTime": "0000",
		"endTime": "0000",
		"type": "miscellaneousReason",
		"typeName": null,
		"cause": null,
		"description": null,
		"incidents": [{
			"incidentId": 135490,
			"description": "À partir du jeudi 7 avril 2016, tous les jours suite à des travaux de rénovation, la station Assemblee Nationale est fermée sur la ligne 12 du Métro jusqu'au jeudi 30 juin 2016.",
			"lines": [{
				"id": 4,
				"codeStif": null,
				"message": "À partir du jeudi 7 avril 2016, tous les jours suite à des travaux de rénovation, la station Assemblee Nationale est fermée sur la ligne 12 du Métro jusqu'au jeudi 30 juin 2016.",
				"shortMessage": "(M 12) du 07/04/16, Ts les jours la station Assemblee Nationale est fermée jusqu'au 30/06/16. (travaux de rénovation)",
				"incidentSeverity": "medium",
				"consequence": null,
				"stopPoints": [12675],
				"stopPointsName": []
			}]
		}]
	}]
}
```

**Les incidents sur la ligne de métro 1 :**
> http://apixha.ixxi.net/APIX?keyapp=FvChCBnSetVgTKk324rO&cmd=getTrafficSituation&networktype=line&network=1&apixFormat=json

**Résultat :**
```json
{
	"events": []
}
```

