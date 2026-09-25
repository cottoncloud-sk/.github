# Firemný web alebo marketplace: kedy už projekt potrebuje samostatný frontend

Nie každý projekt s ponukou služieb potrebuje Next.js alebo vlastnú aplikačnú
vrstvu. Klasický firemný web má návštevníkovi rýchlo vysvetliť ponuku, ukázať
dôkazy a viesť ho k dopytu. Marketplace rieši iný typ úlohy: musí udržať
prehľadnú cestu medzi väčším množstvom položiek, vyhľadávaním, filtrami,
detailmi a samostatnými používateľskými tokmi.

Tento materiál je rozhodovacia mapa pre firmy pred tvorbou web stránky alebo
redizajnom. Nie je to argument, že každé riešenie má byť postavené na Next.js.
Technológia má nasledovať rozsah produktu a zodpovednosť za jeho fungovanie.

## Kedy zvyčajne stačí firemný web

Firemný WordPress web je vhodný, ak hlavnou úlohou je:

- vysvetliť služby, odbornosť a spôsob spolupráce;
- prezentovať realizácie, referencie, tím alebo cenníkové východiská;
- viesť návštevníka k jednému jasnému kontaktu, briefu alebo dopytu;
- nevyžadovať verejné hľadanie vo veľkom katalógu ani vlastné účty používateľov.

V takom prípade je dôležitejšia zrozumiteľná ponuka, dôkaz, mobilné UX,
indexovateľnosť a spoľahlivý formulár než komplikovanejšia architektúra.

## Signály, že rozsah prerastá klasický firemný web

Samostatný aplikačný frontend treba zvážiť, keď produkt potrebuje kombináciu
viacerých z týchto vlastností:

1. verejný katalóg s mnohými položkami, kategóriami a detailmi;
2. vyhľadávanie, filtre, prázdne výsledky a návrat z detailu do výsledkov;
3. rozdielne cesty pre bežného návštevníka, prihláseného používateľa a správcu;
4. pridávanie obsahu, účet, platbu alebo iný stav, ktorý nemožno zameniť za
   obyčajný kontaktný formulár;
5. jasné oddelenie verejnej vrstvy od citlivých alebo autentifikovaných tokov.

Tieto signály samy osebe nepredpisujú konkrétny framework. Znamenajú však, že
do zadania musí pribudnúť dátový model, hranice API, chybové stavy, monitoring,
testy a konkrétny rollback plán.

## Verejný príklad: PredámKúpim.sk

[PredámKúpim.sk](https://cottoncloud.sk/pripadova-studia-predamkupim-nextjs-marketplace/?utm_source=github&utm_medium=referral&utm_campaign=firemny_web_marketplace_decision_map_2026_09&utm_content=case_study)
je verejný príklad marketplace s novým Next.js rozhraním nad existujúcim živým
aplikačným jadrom. Verejne overiteľný rozsah zahŕňa kategórie, lokálne
hľadanie, filtre, detail inzerátu, mobilné ovládanie a oddelenie verejného
prehliadania od prihlásenia, pridania inzerátu a platobných tokov.

Prípadová štúdia nezverejňuje členské údaje, správy, tajomstvá ani proprietárny
zdrojový kód. Netvrdí ani konkrétnu návštevnosť, konverzie alebo pozície vo
vyhľadávaní bez samostatného merania.

## Čo má obsahovať rozhodnutie pred realizáciou

Pred výberom dodávateľa alebo technológie si nechajte zodpovedať tieto otázky:

- Je hlavným cieľom získať dopyt, alebo obslúžiť katalóg a samostatné
  používateľské toky?
- Ktoré stránky musia byť verejné a indexovateľné a ktoré vyžadujú prihlásenie?
- Čo sa stane pri prázdnom výsledku, chybe API alebo nedostupnom externom
  systéme?
- Kde sa ukladajú dáta, kto vlastní zdrojový kód a ako prebehne odovzdanie?
- Ako sa bude testovať mobil, tablet, desktop, formuláre, navigácia a návrat
  do funkčného stavu po chybe?

Pri CottonCloud je dohodnutý custom plugin a zdrojový kód vytvorený pre projekt
po zaplatení vlastníkom zákazník; tretie strany a ich licencie ostávajú
oddelené. Konkrétny rozsah musí byť vždy písomne uvedený v ponuke a odovzdaní.

## Kde začať

Ak potrebujete [firemný web](https://cottoncloud.sk/firemny-web/?utm_source=github&utm_medium=referral&utm_campaign=firemny_web_marketplace_decision_map_2026_09&utm_content=service),
začnite zrozumiteľnou obchodnou cestou a dôkazmi. Pri rozsiahlejšom produkte
pomôže [tvorba web stránok](https://cottoncloud.sk/tvorba-webstranok/?utm_source=github&utm_medium=referral&utm_campaign=firemny_web_marketplace_decision_map_2026_09&utm_content=service)
a [WordPress alebo aplikačný vývoj](https://cottoncloud.sk/wordpress-vyvoj/?utm_source=github&utm_medium=referral&utm_campaign=firemny_web_marketplace_decision_map_2026_09&utm_content=service)
navrhnúť podľa reálneho toku používateľa, nie podľa názvu technológie.

Tento dokument je informačný. Nezaručuje výsledky vo vyhľadávaní, AI citácie,
návštevnosť ani počet dopytov; tie sa dajú posudzovať až z konkrétneho
nasadenia a porovnateľných dát.
