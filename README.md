# Luha
 L'objectif <a href="https://luha.alwaysdata.net">du projet luha</a> est de fournir un traducteur collaboratif et évolutif du Shimaoré.<br>
				Avec l'api luha utiliser gratuitement les données qui sont disponible sur le projet luha dans vos projets.
        
## Traduction français vers shimaore 
### cURL :

curl -X GET \ : https://luha.alwaysdata.net/api.php?mot=marché

La réponse sera :

 ```
 { "resultat":{ "français":"marché", "shimaore":"bazari" } }
```

Si luha ne dispose pas encore de traduction pour ce mot la réponse sera :

curl -X GET \ : https://luha.alwaysdata.net/api.php?mot=gladiateur

 ```
{ "resultat":{ "français":"gladiateur", "shimaore":"pas de traduction disponible" } }
```

## Traduction shimaore vers français

### cURL :


curl -X GET \ : https://luha.alwaysdata.net/api.php?mot=bazari&langue=sh_to_fr

La réponse sera :
```
{ "resultat":{ "shimaore":"bazari", "français":"marché" } }
```

Si luha ne dispose pas encore de traduction pour ce mot la réponse sera :

curl -X GET \ : https://luha.alwaysdata.net/api.php?mot=kojo&langue=sh_to_fr

```
{ "resultat":{ "shimaore":"kojo", "français":"pas de traduction disponible" } }
```
