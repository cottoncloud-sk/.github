# Prečo čiastkový export nepreukazuje chýbajúci materiál

CottonCloud Engineering · 28. september 2026

Čiastkový skladový export vie potvrdiť, že sa položka v danom okamihu objavila.
Nevie však sám spoľahlivo dokázať jej absenciu. Pri inventúre môže zachytiť iba
časť rozsahu, stav pred návratom z inventúry alebo pohľad po presune, v ktorom
už chýba pôvodná pozícia. Bez ranného úplného stavu a finálneho úplného
výpisu by systém ľahko zamenil rozpracovanú zmenu za manko.

Preto má byť ranný úplný LX02 referenčným bodom, priebežné LX02 majú popísať
vývoj a finálny úplný LX02 má potvrdiť, ktoré rozdiely ostali otvorené. Toto
nie je náhrada skladového účtovania ani pokyn vykonať SAP pohyb. Je to pravidlo
pre systém, ktorý organizuje kontrolu a nestráca súvislosť medzi pôvodnou
pozíciou, priebehom inventúry a výsledným rozhodnutím.

## Modelové testovacie situácie

Nasledujúce situácie sú návrhy testov pre vlastný projekt. Opisujú očakávané
správanie, nie výsledok konkrétneho runtime testu.

1. **Riadok chýba v čiastkovom výpise.** Systém nesmie označiť materiál ako
   chýbajúci len preto, že sa neobjavil v priebežnom exporte. Zachová ho ako
   predbežný stav a čaká na relevantný úplný výpis alebo na ďalší podklad.

2. **HU sa vráti do iného bežného regála.** Ak sa tá istá manipulačná jednotka
   objaví mimo inventúrnej pozície v inom bežnom regáli, návrat sám osebe nie
   je chyba. Systém má zachovať pôvodnú pozíciu z ranného stavu, rozpoznať
   návrat jednotky a zobraziť novú aktuálnu pozíciu s kontextom zmeny.

3. **Cena je neznáma.** Chýbajúca alebo nejednoznačná cena
   sa nesmie nahradiť nulou. Neznáma jednotka alebo mena musí zostať označená.
   Report ukáže potrebu doplnenia, aby finančný súčet nevyzeral úplne iba
   preto, že chýbal vstup.

4. **Regál je otvorený alebo uzavretý.** Otvorený regál patrí do priebehu
   práce, preto ho systém nemá vyhodnocovať rovnako ako uzavretú časť. Po
   uzavretí sa dá jeho stav posúdiť voči pravidlám rozdielov; dovtedy zostáva
   viditeľný ako rozpracovaný krok.

5. **Monitorovací klient skúsi meniť spoločný stav.** Monitor má zobrazovať
   priebeh, ale nesmie vytvoriť ani prepísať spoločný záznam. Zápis patrí iba
   určenej pracovnej stanici, aby nevznikli dve konkurenčné interpretácie
   rovnakého rozdielu.

Takéto testy preverujú rozhodovaciu hranicu, ktorú samotný export nevidí:
prítomnosť je možný dôkaz, absencia bez úplného kontextu nie. Implementačný
kontext a anonymizovaný príklad sú verejne popísané v case study
[Inventúrny systém pre výrobný podnik](https://cottoncloud.sk/pripadova-studia-inventurny-system-sap-vyroba/).
