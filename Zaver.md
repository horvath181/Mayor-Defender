Mojou časťou ročníkového projektu bolo vytvoriť hru v GameMaker Studiu. Najprv som študoval tento framework na tvorbu hier (prechádzal si tutoriály, čítal dokumentáciu). Následne som začal zháňať zdrojové súbory: obrázky, hudba, zvuky, ... . Potom som to spojil dokopy.

Najprv len pohyb, streľbu šerifa a postavu starostu. Potom som pridal nepriateľov (banditov) a počítadlo skóre. Potom som sa dostal do bodu, kedy som to chcel skúsiť spustiť na mobile. Tak som si našiel čo všetko potrebujem stiahol a nastavil. Neskôr som mal problém, keď vyšiel nový Android, pretože mi to zrazu nešlo, no problém som vyriešil.

Tu približne skončil prvý semester. Mal som spustiteľnú aplikáciu s uvítacím Menu, pohyblivým pozadím, hudbou v pozadí a animáciou pohybu postáv. Navyše, keď hra skončila, zobrazilo sa skóre hráča a správa "Mayor is dead!". V Menu mal hráč dve možnosti:
* "Play" - presunie hráča do miestnosti kde sa automaticky spustí hra
* "Quit" - ukončí hru

V druhom semestri som pridal len pár drobností. Najprv animáciu smrti starostu, aby bol koniec trochu zaujímavejší. Potom som pridal Tutorial, aby si mohol hráč najprv vyskúšať do čoho ide. Pôvodne Tutorial končil vytvorením 15 inštancií objektu nepriateľa, čo je ťažké prežiť (neviem neskúšal som). No keďže to nebolo veľmi príjemné uvítanie do hry, tak som to zmenil. Aktuálne sa na konci Tutoriálu spawnú 2 nepriatelia, starostu nejde zabiť a banditi nepribúdajú. Tu si môže hráč vyskúšať, ako hra funguje (safe mode). Do hlavného menu sa potom vrátite stlačením tlačidla Main Menu v pravom dolnom rohu. Následne som upravil aj návrat do Menu po ukončení hry. Pôvodne sa hráč vrátil po ťuknutí kamkoľvek. Keďže sa hráč jednoducho preklikne a do Menu sa vráti bez toho aby vedel aké mal skóre, tak aj sem som pridal tlačidlo Main Menu na návrat do Menu a zrušil dovtedy aplikovaný spôsob presunu. Poslednou vecou, ktorú som tento semester implementoval je Highscore, tabuľka top 10 hráčov. Po smrti starostu sa hra opýta, "Pod akým menom chceš byť známy?", po anglicky (ako celá hra). Tabuľku Highscore sa dá aj resetovať. Heslo pre resetovanie je "Answer". Toto heslo sa nedá meniť a je ho vidno, keď ho píšete. Navyše som narazil na problém, ktorý som nevedel vyriešiť a ani som nenašiel, ako ho vyriešiť. Vždy keď žiadam vstup od hráča (zápis do Highscore, resetovanie tabuľky Highscore), tak na mobile mi prestane hrať hudba v pozadí. Tento problém som však nikde nenašiel ani spomenutý a tak som sa tým viac nezaoberal.

Aktuálne sú v hlavnom menu štyri možnosti:
* "Play"
* "Highscore" - presunie hráča do miestnosti, kde mu ukáže tabuľku top 10. Tu sa dá resetovať stav tabuľky. Ak tabuľka neobsahuje dostatok záznamov, zobrazuje "<Nobody>" s 0 bodmi.
* "Tutorial" - presunie hráča do miestnosti kde mu spustí tutoriál. Ten obsahuje popis hry, popis možností (pohyb, streľba), popis postáv a následne safe mode.
* "Quit"

Keďže môj kolega, s ktorým pracujem na tomto projekte mal zložitejší framework, postupoval pomalšie a tak som naňho často s vývojom čakal. Pôvodne sme mali hru vyvíjať viac menej súbežne. 

# GameMaker Studio 1.4

## Výhody:
* Má veľa predprogramovaných funkcií. Takmer vždy (ak nie vždy), keď som niečo potreboval, našiel som na to po chvíli funkciu.
* Kód sa vytvára priamo v objektoch formou udalostí s možnosťou Drag&Drop funkcií. Vďaka tomuto je softvér prístupnejší pre začiatočníkov, no obsahom môže osloviť aj skúsenejších.
* Po prejdení si pár tutoriálov som sa vedel vcelku dobre zorientovať v rozhraní.
* Možnosť upravovať a tvoriť obrázky priamo vo framework-u.

## Nevýhody:
* Softvér je z väčšej časti platený. Spoplatnené sú všetky formáty, okrem Windowsu (tým sa myslí tvorba hier pre Android, iOS, konzoly, ...). Niektoré funkcie sú v bezplatnej verzii tiež nedostupné.
* Vždy pred spustením hry všetko kompiluje. Na mojom notebooku to vždy chvíľu trvá.
