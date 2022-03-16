Panaudojus `docker-compose up -d` - automatiškai pullinamas Docker image, paleidžiamas MySQL prieš paleidžiant patį Laravel.
Automatiškai sutvarkomos reikiamos teisės (chown, chmod), iššaukiamos **serve** ir **migrate:fresh --seed** komandos.

DB ir admin vartotojo konfiguracija .env faile.
Po paleidimo sukuriamas admin vartotojas ir personal access token, kuris išsaugomas **storage/app/token.txt**

API nuorodos eksportuotos per Postman. TOKEN nurodytas tarp kolekcijos parent **VARIABLES**

2 modeliai - orders ir users, kuriems sukurtos CRUD funkcijos.
Paprastas REST API su token auth (Laravel Sanctum).
orderscount vartotojui atnaujinamas sukuriant/ištrinant su juo surištą order.