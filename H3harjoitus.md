# h3 Versionhallinta

Tämä harjoitus on tehty osana Tero Karvisen palvelinten hallinta kurssia. Harjoitukset tehtiin VirtualBoxille asennetulla Debian 11 Bullseye virtuaalikoneella.

## z) Lue ja tiivistä

[Lähde](https://commonmark.org/help/)

- Artikkelissa kerrotaan markdownin käyttöön liittyvät tärkeät komennot.

- Tyhjä rivi tekee kappalejaon, nämä ranskalaiset viivat tulevat samalla tavalla kuin muuallakin, mutta myös *-merkkiä voi käyttää listojen tekemiseen.

- Nettisivun linkkaus tapahtuu 	`[Link](nettisivun osoite)` komennolla.

- Risuaita/Hashtag eli # luo otsikon, kaksi risuaitaa ## luo otsikko kakkosen.

- Sisennys luominen tabulaattorilla merkitsee koodin kirjoittamista.

- Otsikko jonka kirjoitin boldilla, onnistuu kirjoittamalla kaksi tähteä * boldattavan sanan molemmille puolille.

## a) MarkDown. Tee tämän tehtävän raportti MarkDownina. Helpointa on tehdä raportti GitHub-varastoon, jolloin md-päätteiset tiedostot muotoillaan automaattisesti. Tyhjä rivi tekee kappalejaon, risuaita '#' tekee otsikon, sisennys merkitsee koodinpätkän.

Aloitin tehtävän teon luomalla uuden repositoryn githubiini nimellä `PalvHalH3`. Lisäsin sinne tiedoston nimellä `H3harjoitus.md`.

Tämän jälkeen asetin git config tiedostoon käyttäjänimekseni taanttila kuten GitHubissa, sekä sähköpostiosoitteeni komennoilla `git config --global user.name "taanttila"` sekä `git config --global user.email "sähköpostini"`.

Loin ssh-avaimet komennolla `ssh-keygen ecdsa` , jotta saisin yhteyden GitHubiin. Asetin luodun public keyn GitHubiin, ja kirjoitin komennon `git remote add origin git@github.com:taanttila/PalvHalH3.git` joka loi yhteyden.

Kirjoitin kotihakemistossani komennon `git clone https://github.com/taanttila/PalvHalH3.git` joka kopioi luomani repositoryn koneelleni.

Tämän jälkeen kirjoitin komennon git pull joka päivitti hakemiston tiedoilla, jotka ovat repositoryssani. Sen jälkeen aloin editoimaan H3harjoitus.md tiedostoa nano tekstieditorilla komennolla `nano H3harjoitus.md`.

Tähän asti kirjoittamani raportin tallensin, ja kirjoitin komennot `git add README.md` sekä `git commit`.

## b) Pull first. Tee useita muutoksia git-varastoosi. Tee muutama muutos, jossa yksi commit koskee useampaa tiedostoa. Anna hyvä kuvaukset (commit message), yksi englanninkielinen lause imperatiivissa (määräysmuodossa) "Add top level menu to Foobar synchronizer"

Tein muutoksia H3harjoitus.md tiedostoon sekä README.md tiedostoon. Lisäsin osia harjoitukseen, sekä muutin tietoa README.md:ssä vastaamaan repositoryn sisältöä. Loin myös uuden kansion nimellä screenshots komennolla `mkdir screenshots` ollessani github hakemistossa, jotta saan kuvia asetettua helpommin tähän raporttiin. Tähän löysin apua [Tuuli Huhtasen raportista](https://github.com/tuuli-huhtanen/palvelintenhallinta/blob/main/h3-versionhallinta.md), hän oli löytänyt ohjeita siihen [täältä](https://careerkarma.com/blog/git-create-folder-in-github/).

Kansiot eivät ole tyhjänä näkyvissä GitHubissa, joten loin myös screenshots kansioon tyhjän tiedoston komennolla `touch screenshots/.gitkeep`.

![Image](https://raw.githubusercontent.com/taanttila/palvelintenhallinta/main/screenshots/gitadd.PNG)

![Image](https://raw.githubusercontent.com/taanttila/palvelintenhallinta/main/screenshots/gitcommit.PNG)

## b) Kaikki kirjataan. Näytä omalla git-varastollasi esimerkit komennoista 'git log', 'git diff' ja 'git blame'. Selitä tulokset.

Kokeilin komentoa `git log` joka näyttää kaikki muutokset mitä on tehty. Siitä näkee Authorin, eli kuka on tehnyt muutokset, päivämäärän sekä tekijän kommentit.

![Image](https://raw.githubusercontent.com/taanttila/palvelintenhallinta/main/screenshots/gitlog.PNG)

Löysin samalta kurssitoteutukselta olevalta [Tuomas Lintulalta ja hänen tekemästään raportista](https://github.com/tuomaslin/palvelintenhallinta/blob/main/MarkDown.md) komennon `git log --pretty=oneline` joka tulostaa historian lyhyemmässä muodossa. Kokeilin myös tätä komentoa.

![Image](https://raw.githubusercontent.com/taanttila/palvelintenhallinta/main/screenshots/gitlogpretty.PNG)

Kokeilin myös komentoa `git blame`. Tämä komento kertoo kuka on tehnyt muutoksia valitsemaasi tiedostoon. Ajoin komennon `git blame README.md` jolloin näkyviin tuli muutoksen tekijä, SHA avain, päivämäärä ja mikä muutos tehty.

![Image](https://raw.githubusercontent.com/taanttila/palvelintenhallinta/main/screenshots/gitblame.PNG)

## c) Huppis! Tee tyhmä muutos gittiin, älä tee commit:tia. Tuhoa huonot muutokset 'git reset --hard'. Huomaa, että tässä toiminnossa ei ole peruutusnappia.






 

