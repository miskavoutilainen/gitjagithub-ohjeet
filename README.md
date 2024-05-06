# Git ja GitHub

<img src="./gitgithub.png" width="300">

## Mikä on Git?
Git on monipuolinen työkalu, joka on suunniteltu toimimaan hajautettuna versionhallintana. Hajautettu versionhallinta tarkoittaa sitä, että jokainen kopio Gitin tietovarastosta toimii itsenäisesti. Git työkalu käsittelee kaikki muutokset paikallisesti. Muutokset voidaan myös työntää etätietovarastoon (remote repository) kun ne tahdotaan jakaa muiden ohjelmoijien kanssa tai sitten muutoin pistää talteen. 

## Mikä on GitHub?
GitHub tarjoaa paikan Git-versionhallintaa käyttäville ohjelmakehitysprojekteille. GitHub tarjoaa käyttöliittymän sekä tallennuskapasiteettia Gitillä hallittuihin tietovarastoihin.

## Git käyttö:
1. Otetaan Git käyttöön:
`git init`
2. Määritetään käyttäjänimi (jos käytetään ensimmäistä kertaa): `git config user.name "Etunimi Sukunimi"`
3. Määritetään käyttäjänimi (jos käytetään ensimmäistä kertaa): `git config --global user.email "nimi@sposti.com"`

## Tiedostojen käsittely Git:ssä
1. Lisätään luodut tiedostot Git indeksiin: `git add tiedostonnimi` tai `git add .` <- lisää kaikki tiedostot indeksiin
2. Luodaan commit lisäyksistä: `git commit -m "Tähän tietoja lisäyksistä/muutoksissa"`

## Git tilan ja logi
- Git tilan voi tarkistaa näin: `git status`
- Listan commiteista näkee komennolla: `git log`, mikäli haluaa selkeämmän listauksen: `git log --oneline` 

## Git ja GitHub yhdistäminen
1. Kytketään GitHub etärepositorio paikalliseen projektiin: `git remote add origin https://github.com/GitHubTunnus/GitHubRepositorio.git`
    - Etärepositorio kytkökset voi tarkistaa näin: `git remote -v`
2. Paikallisen työkansion tiedostot voi viedä lopuksi GitHubiin näin: `git push -u origin master`

## GitHubista synkronoiminen
1. GitHub repositorion ja paikallisen työkansion tilenteen erojen päivittäminen: `git fetch`
2. Tietojen lataaminen GitHub repositoriosta paikalliseen työkansioon: `git pull`

## Git haarat (branch)
- Uuden haaran lisääminen: `git branch haaran_nimi`
- Haaran tietojen yhdistäminen master päähaaraan: `git merge haaran_nimi`
- Haaran poistaminen: `git branch -d haaran_nimi`
- Git haarojen listaaminen: `git branch`
