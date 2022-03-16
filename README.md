Panaudojus `docker-compose up -d` - automatiškai pullinamas Docker image, paleidžiamas MySQL prieš paleidžiant patį Laravel.
Automatiškai vykdomos **serve** ir **migrate** komandos kartu su seed.

DB ir admin vartotojo konfiguracija .env faile.
Po paleidimo sukuriamas admin vartotojas ir personal access token, kuris išsaugomas **storage/app/token.txt**

API nuorodos eksportuotos per Postman. TOKEN nurodytas tarp kolekcijos parent **VARIABLES**