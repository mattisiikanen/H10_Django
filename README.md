# h9_Sequel


## Ympäristö

Hyper-V kotikoneella (Host):

- CPU: i5-9600K
- RAM: 16Gb
- HDD: 120Gb
- Win 11 Pro x64

Virtuaalikoneen speksit:

- 2 x CPU
- 4 Gb RAM
- 50 Gb HDD
- Generation 2 (Hyper-V pyytää määrittelemään)


## Aloitus 
Tehtävän tarkoituksena oli tehdä tunnilla käyty harjoitus Djangosta. Aloitin tehtävät 17.2.2023 klo 17:30 käynnistämällä Hyper-V:llä pyörivän palvelimen.
Minulta ei löytynyt etukäteen osaamista Pythonista tai Djangosta, joten olin täysin ohjeiden varassa tehtävien osalta. Luin ensiksi läpi opettajamme Tero Karvisen ohjeen Djangon käyttöön otosta nimeltä "Django 4 Instant Customer Database Tutorial".

## a) Kannattavaa. Tee oma tietokantasovellus. jossa on weppiliittymä


### Django asennus

Käytin tehtävään ainoastaan omalla koneella olevaa virtuaalikonetta. Aloitin tehtävän päivittämällä repositoriot komennolla ```sudo apt-get update```, jonka jälkeen siirryin asentamaan Virtualenv paketin ```sudo apt-get -y install virtualenv```</br>
![Kuva1](https://user-images.githubusercontent.com/122887740/219697917-2ff10854-3433-49de-add2-73d1a839d891.png)</br>

Asennus näytti menevän nätisti sisään. Seuraavaksi oli vuorossa luoda uusi virtuaalinen ympäristö, jonka avulla asennettiin viimeisimmät versiot Pythonin paketeista.
Käytin tähän komentoa ```virtualenv --system-site-packages -p python3 env/```, joka näytti myös onnistuvan ongelmitta: </br>
![Kuva2](https://user-images.githubusercontent.com/122887740/219698339-83e4a081-7e83-4a2b-a3b6-24d6653822c3.png) </br>


Kun virtuaaliympäristö oli luotu, oli aika aktivoida se ```source env/bin/activate``` ja aktivoinnin jälkeen tuli tarkistaa, että mihin komennolla ```pip``` viitataan, jottei asennus mene väärään ympäristöön:</br>
![Kuva3](https://user-images.githubusercontent.com/122887740/219699272-fdf00d95-77a8-4ceb-b3e6-a9916cc5e1cb.png)</br>

Tässä tapauksessa minulla oli oikea ympäristö aktivoituna, joten pystyin jatkamaan Djangon asennukseen. Asennusta varten minun tuli kuitenkin ensin luoda määritysiedosto Microlla, jotta ```pip``` osasi asentaa oikean paketin käyttööni:</br>
![Kuva4](https://user-images.githubusercontent.com/122887740/219700090-dd46dfcb-6a1a-470b-8d45-37467e6f5da7.png)</br>


Määritystiedoston jälkeen siirryin lopulta asentamaan Djangon komennolla ```pip install -r requirements.txt```: </br>
![Kuva5](https://user-images.githubusercontent.com/122887740/219700677-207a936f-74fc-4e9c-a4d9-a70d2a5e20d3.png) </br>


Määritystiedosto oli selvästikin määritetty oikein, koska Django asentui koneelle mutkitta. Tein kuitenkin vielä varmistuksena versio tarkistuksen Djangoon, jotta viimeisin oli asentunut koneelle: </br>
![Kuva6](https://user-images.githubusercontent.com/122887740/219701006-987e45e8-47f7-44a1-adea-8216145ba787.png)


Lopetin hommat tältä erää tähän, homma jatkuu myöhemmin.

### Djangon konfigurointi
Klo 17:50 </br>

Asennuksen jälkeen oli vuorossa 



## Lopetus
Lopetin tehtävien teon klo 21:57. Kyseinen tehtävä avasi hyvin tietokantoja sekä SQL-kielen käsittelyä. Töihin meni tällä erää n. 2h.

## Lähteet:
Karvinen, Tero, 2022 - Django 4 Instant Customer Database Tutorial (https://terokarvinen.com/2022/django-instant-crm-tutorial/)
