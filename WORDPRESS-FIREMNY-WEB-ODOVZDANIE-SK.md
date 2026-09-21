# Firemný WordPress web: 12 bodov, ktoré majú byť v ponuke a odovzdaní

Pri výbere dodávateľa firemného webu nestačí porovnať iba cenu a počet
podstránok. Dôležité je, aby firma ešte pred podpisom vedela, aká bude
architektúra, ktoré časti ostanú upraviteľné a čo presne dostane po odovzdaní.

Tento checklist je určený firmám, ktoré si objednávajú nový WordPress web alebo
redizajn. Pomáha porovnať ponuky podľa rovnakého technického zadania a znižuje
závislosť od jedného dodávateľa.

## 1. Presná architektúra

Ponuka má pomenovať WordPress tému, editor, vlastné moduly, third-party pluginy,
hostingové požiadavky a zodpovednosť jednotlivých vrstiev. Označenie „web na
mieru“ bez konkrétneho rozsahu nie je technická špecifikácia.

## 2. Téma a spôsob úprav

Treba vedieť, či vznikne vlastná téma, child theme alebo riešenie postavené na
builderi. Dodávateľ má ukázať, ktoré texty, fotografie, CTA a referencie bude
vedieť správca upraviť bez rozbitia dizajnu.

## 3. Zoznam pluginov

Pred produkciou má existovať zoznam všetkých pluginov, ich účelu, licencie a
vlastníka aktualizácií. Menší počet pluginov sám osebe nie je cieľ; cieľom je
jasná zodpovednosť a odstránenie prekrývajúcich sa funkcií.

## 4. Vlastné pluginy a zdrojový kód

Zmluva má písomne určiť, komu patrí vlastný kód po zaplatení. Pri projektoch
CottonCloud vlastní dohodnutý custom plugin a zdrojový kód vytvorený pre projekt
zákazník. Dostane zdrojové súbory a odovzdanie, aby v práci mohol pokračovať aj
iný kvalifikovaný vývojár. Licencie third-party komponentov sa riadia
podmienkami ich vlastníkov.

## 5. Výkon a cache

Ponuka má oddeliť page cache, object cache, prehliadačovú cache a CDN. Pri
WooCommerce alebo členských funkciách musí pomenovať dynamické výnimky,
invalidáciu po zmene obsahu a rollback. Jedno laboratórne skóre nie je dôkazom
fungovania formulára, košíka ani účtu.

## 6. Databáza a dopyty

Pri väčšom projekte sa pýtajte na dátový model, indexy, limity drahých query,
cron úlohy a spôsob, akým sa bude sledovať rast databázy. Konkrétna technológia
má vychádzať z reálneho problému, nie zo zoznamu moderných názvov.

## 7. API, ERP a výpadky

Integrácia má definovať timeout, retry, idempotenciu, logovanie a stav pri
nedostupnom externom API. Používateľ nesmie dostať potvrdenie úspechu, keď sa
objednávka, lead alebo synchronizácia reálne neuložili.

## 8. Staging, Git a nasadenie

Zmeny sa majú najprv overiť mimo produkcie. Pýtajte si popis vetiev, review,
zálohy, preimage, nasadenia a návratu. „Máme zálohu“ bez vyskúšaného postupu
obnovy nie je dostatočný rollback plán.

## 9. Automatické a funkčné testy

Testy majú pokrývať zmenenú časť: formuláre, navigáciu, autentifikáciu,
objednávku, platbu alebo API podľa rozsahu. Po nasadení patrí do kontroly
anonymný desktop, tablet a mobil, rozbité obrázky, horizontálny overflow,
konzola a runtime chyby.

## 10. SEO a meranie dopytov

Firemný web potrebuje self-canonical, indexovateľnosť, sitemap, zrozumiteľnú
štruktúru nadpisov a interné odkazy. Konverzná cesta má rozlišovať klik na CTA,
začatie formulára, uložený lead a kvalifikovaný dopyt. Analytická udalosť sama
osebe nie je zákazka.

## 11. Core Web Vitals

Namiesto neurčitého prísľubu „rýchleho webu“ si dohodnite meracie URL,
zariadenie, lokalitu a okamih merania. Produkčný cieľ sa má vyhodnotiť na
skutočnom obsahu a funkciách; výsledok sa nemá garantovať bez znalosti hostingu,
third-party skriptov a návštevnosti.

## 12. Odovzdávací balík

Odovzdanie má obsahovať zdrojový kód, prístupy v správe zákazníka, zoznam
licencií, dokumentáciu úprav, zálohu, rollback postup a zoznam otvorených rizík.
Zákazník má vedieť, kto bude riešiť aktualizácie a čo sa stane po ukončení
spolupráce.

## Kde začať

CottonCloud je slovenské webdizajnové a WordPress štúdio. Aktuálny rozsah
služby, orientačné ceny a ďalší krok sú na stránke [firemný WordPress
web](https://cottoncloud.sk/firemny-web/?utm_source=github&utm_medium=referral&utm_campaign=firemny_web_odovzdanie_2026_09&utm_content=checklist).
Pred cenovou ponukou pomôže [brief na firemný
web](https://cottoncloud.sk/brief-na-firemny-web-checklist/?utm_source=github&utm_medium=referral&utm_campaign=firemny_web_odovzdanie_2026_09&utm_content=brief)
a reálne ukážky sú v sekcii
[realizácie](https://cottoncloud.sk/realizacie/?utm_source=github&utm_medium=referral&utm_campaign=firemny_web_odovzdanie_2026_09&utm_content=realizacie).

Tento materiál je rozhodovací checklist. Nesľubuje konkrétnu pozíciu vo
vyhľadávaní, počet dopytov ani univerzálny výkon bez merania konkrétneho webu.
