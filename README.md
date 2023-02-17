# Git:in käyttöönotto

Git käyttöönotetaan komennolla
```git init```

Git komennolla ```git status```näytetään gitin nykyinen tila. Näyttää jos tiedostoja on muutettu.

Git komennolla esim. ```git add README.md``` lisätään tiedosto "tallennusvaiheeseen"

Git komennolla ```git commit -m '#625 Added readme information'``` tallennetaan muutos tietokantaan

# .gitignore

Gitignore tiedosto kansion päätsolla kertoo mitä kansioita ja tiedostoja ei tallenneta git:in varastoon. Esimerkki nodejs: (https://github.com/github/gitignore/blob/main/Node.gitignore)
```
.gitignore
--
node_modules/
```

# Commit messaget

Commit message koostuu useiten seuraavista asioista ```#754 Fixed SQL injection in login form```

#754 = Tehtävän/Task:in ID minkä muutosta ollaan tallentamassa

Fixed SQL injection in login form

# Commit messaget

Commit message koostuu useiten seuraavista asioista ```#123 Create product form```

#123 = Taskin ID minkä muutosta ollaan tallentamassa

Create product form = Taskin nimi

# Loogiset versiot branchit

* Main
    * Ohjelmiston pääversio
* Test
    * Ohjelmiston esituotanto/testaus versio 
* Development
    * Ohjelmiston ajantasainen kehitysversio
* Feature
    * Uusien ominaisuuksien kehitykseen avataan uudet feature haarat
* Bugfix
    * Bugien korjaamiseen uusi bugikorjaus haara

# Brancien hallinta

Komento ```git branch```näyttää eri versiot ja aktiivisen * merkillä.

Uuden branchin luonti ```git branch test```

Siirtyminen toisen branchin alle ```git checkout development``

Kun siirrytään toiseen branchiin, varmista ettei working directoryssä ole muutoksia kesken.

# Merget eli liitokset

Siirry Branchiin johon haluat liittää sisällön. Esim. development. Liitä esim feature haara developmenttiin ```git merge feature123 --squash```