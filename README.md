# BD-Client
travail serveur client 


les 5 commandes pour chaque API : 

weather

_On peut obtenir la metéo par le nom de la ville
  *api.openweathermap.org/data/2.5/forecast?q=London,us&mode=xml
_On peut aussi obtenir la meteo par le l'id de la ville 
  *api.openweathermap.org/data/2.5/forecast?id=524901
_On peut aussi se servir des coordonnées geographique 
  *api.openweathermap.org/data/2.5/forecast?lat=35&lon=139 
_On peut aussi choisr de recevoir les données sous le format de notre choix en fonction de notre utulisation 
 *FORMAT JSON
  api.openweathermap.org/data/2.5/weather?q=London
 *FORMAT XML
  api.openweathermap.org/data/2.5/weather?q=London&mode=xml
 *FORMAT HTML
  api.openweathermap.org/data/2.5/weather?q=London&mode=html
_on peut aussi choisir de recoir les données des temperature en differentes unités de mesures 
 *KELVIN unité utilisée par defaut 
  api.openweathermap.org/data/2.5/find?q=London
 *CELSIUS 
  api.openweathermap.org/data/2.5/find?q=London&units=metric
 *FAHRENHEIT
  api.openweathermap.org/data/2.5/find?q=London&units=imperial
_on peut aussi choisir sous quelle langues recevoir nos données 
 api.openweathermap.org/data/2.5/forecast/daily?id=524901&lang=zh_cn
_ceci dit si on code en javascript et que l'on a besoin de données bien rangé dans un fichier json 
 *api.openweathermap.org/data/2.5/weather?q=London,uk&callback=test
 
 GitHub api v3
_pour une authentification basique
 $ curl -u "username" https://api.github.com
_pour une authentification avec une clé envoyé dans le lien 
 $ curl -H "Authorization: token OAUTH-TOKEN" https://api.github.com
_pour une authentification avec une clé envoyé en parametre
 $ curl https://api.github.com/?access_token=OAUTH-TOKEN
_pour une authentification avec une clé secrete
 $ curl 'https://api.github.com/users/whatever?client_id=xxxx&client_secret=yyyy'
_pour les requetes envoyant plusieur items ou d'autre page spécifiaue on precise la page ainsi que la taille de la police 
 $ curl 'https://api.github.com/user/repos?page=2&per_page=100'
 
2 DEUX JE CHOISI L'API WEATHER
 
  requêtes HTTP POST :
  _jai listé ces requetes car il s'agit de la meme donnée mais convertit ou modifié a la demande du client 
  
  api.openweathermap.org/data/2.5/find?q=London
  api.openweathermap.org/data/2.5/find?q=London&units=metric
  api.openweathermap.org/data/2.5/find?q=London&units=imperial
  api.openweathermap.org/data/2.5/forecast/daily?id=524901&lang=zh_cn
  api.openweathermap.org/data/2.5/weather?q=London,uk&callback=test
  api.openweathermap.org/data/2.5/find?q=London
  api.openweathermap.org/data/2.5/find?q=London&units=metric
  api.openweathermap.org/data/2.5/find?q=London&units=imperial
  api.openweathermap.org/data/2.5/forecast/daily?id=524901&lang=zh_cn
  api.openweathermap.org/data/2.5/weather?q=London,uk&callback=test
 
   requêtes HTTP GET:
  *api.openweathermap.org/data/2.5/forecast?q=London,us&mode=xml
  *api.openweathermap.org/data/2.5/forecast?id=524901
  *api.openweathermap.org/data/2.5/forecast?lat=35&lon=139
     

