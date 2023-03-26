# projet
```
#!/bin/bash
```
# Définir l’URL du site web à surveiller
```
$(curl -o page.html https://www.boursorama.com/cours/AAPL/)
```
# Boucle infinie pour récupérer les informations périodiquement
```
while true
do
```
# Utiliser la commande curl pour récupérer les informations de l’URL
```
thevariable=$(grep ‘c-faceplate__indicative-value’ page.html | awk ‘{print $5}’)
```
    
# Afficher les informations récupérées
```
echo « Informations récupérées : »
echo $thevariable
```
# Attendre 1 minute avant de récupérer à nouveau les informations
```
sleep 60
done
```
