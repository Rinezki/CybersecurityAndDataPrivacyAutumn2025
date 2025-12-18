# Auth Test Report

## Guest
- Sivulla vierailijat eivät pysty sivun antamista napeista varaamaan tai lisäämään resursseja.
- Vieraat kuitenkin voivat nähdä käyttäjätiedot, varaustiedot ja resurssit. esimerkiksi näin.
![evidence1](.//pics/as_a_guest.png)
![evidence2](.//pics/as_a_guest2.png)
![evidence3](.//pics/as_a_guest3.png)
Nämä api polut löysin käyttämällä gobusteria tekemälläni linux vm:llä.
![evidence4](.//pics/found_apis.png)
- vierailijana en päässyt /adminilla tekemään mitään sivu ilmoitti tämmöistä.
- vierailijana /profile tekee myös saman ilmoituksen kuin /adminilla, ei pääse.
![evidence5](.//pics/adminguest.png)
- Vierailijana pääsee login sivulle ja näkee julkisen listan varauksista.

## Reserver
- reserverinä pääsee ja näkee /resources
- reserverinä pääsee ja näkee /reservation
- voi tehdä varauksia
- reserverinä ei voi mennä /admin/users antaa samaa vika ilmoitusta kuin viimeisessä kuvassa vierailija listassa
- ei pysty poistamaan käyttäjiä /api/admin/users/:id kautta antaa tämmöistä vastausta.
![evidence6](.//pics/reserver.png)
- reserverinä pystyy muokkaamaan resources sivua
![evidence7](.//pics/resources.png)
- pystyy muokkaamaan reservationeja
![evidence8](.//pics/zapinjalkeen.png)

## Admin
- Admin voi lisätä resursseja
- Admin voi poistaa reserverin
- Admin voi muokata kaikkia varauksia
![evidence9](.//pics/adminpov.png)

# Huomio
## Kaikki käyttäjät voivat nähdä samoja juttuja mitä vieraskin näkee jos laittaa samat urlit hakukenttään!

