# Firemný web, ktorý vedie k dopytu: technický checklist

Firemný web neprináša dopyt iba preto, že obsahuje kontaktný formulár. Návštevník musí najprv pochopiť ponuku, nájsť relevantný dôkaz a dostať jeden zrozumiteľný ďalší krok. Technická implementácia potom musí dokázať, že lead sa skutočne uložil — nie iba zobraziť hlášku v prehliadači.

Tento checklist používame pri návrhu a kontrole WordPress firemných webov. Je zámerne oddelený od vizuálneho briefu: sústreďuje sa na overiteľnú cestu od vstupnej stránky po uložený dopyt.

## 1. Prvá obrazovka

- pomenúva konkrétnu službu;
- hovorí, pre koho je určená;
- vysvetľuje očakávaný výsledok bez neurčitých sloganov;
- obsahuje jedno hlavné CTA s konkrétnym ďalším krokom;
- na mobile sa ponuka ani CTA nestratia pod navigáciou alebo dekoráciou.

## 2. Query a obsahová architektúra

Rozdielne intenty nemajú byť natlačené do jednej všeobecnej URL. Pri CottonCloud ich oddeľujeme takto:

- [firemný web](https://cottoncloud.sk/firemny-web/?utm_source=github&utm_medium=referral&utm_campaign=firemny_web_leads_2026_09&utm_content=checklist) — komerčná ponuka pre firemný web;
- [tvorba webstránok](https://cottoncloud.sk/tvorba-webstranok/?utm_source=github&utm_medium=referral&utm_campaign=firemny_web_leads_2026_09&utm_content=checklist) — širší výber typu projektu;
- [webdizajn](https://cottoncloud.sk/webdizajn/?utm_source=github&utm_medium=referral&utm_campaign=firemny_web_leads_2026_09&utm_content=checklist) — UX, vizuálny systém a návrh obrazoviek;
- [WordPress vývoj](https://cottoncloud.sk/wordpress-vyvoj/?utm_source=github&utm_medium=referral&utm_campaign=firemny_web_leads_2026_09&utm_content=checklist) — témy, pluginy a integrácie.

Podporný článok má odpovedať na konkrétnu otázku a odkazovať na správnu komerčnú owner stránku. Nemá vytvárať ďalšiu synonymnú landing page.

## 3. Dôkaz pri ponuke

Relevantná realizácia má byť blízko služby, ktorú dokazuje. Užitočný dôkaz uvádza:

- pôvodný problém alebo zadanie;
- rozsah, ktorý bol reálne dodaný;
- použiteľný screenshot alebo verejnú URL, ak ju možno zverejniť;
- obmedzenia merania;
- výsledok iba vtedy, keď je podložený porovnateľným readbackom.

Nevymýšľame percentá rastu, leady ani Core Web Vitals výsledky bez zdrojových dát.

## 4. Formulár a lead path

Úspešné odoslanie musí mať oddelené stavy:

1. server prijal a validoval požiadavku;
2. lead sa uložil do interného zoznamu alebo CRM;
3. notifikácia sa vytvorila a jej výsledok je dohľadateľný;
4. ďakovná stránka alebo stav sa zobrazil až po úspešnom uložení;
5. GA4 alebo iné meranie zapísalo udalosť až po skutočnom úspechu.

E-mailová schránka nesmie byť jediným miestom, kde lead existuje. Hláška „dopyt je na ceste“ sama osebe nepotvrdzuje uloženie ani doručenie notifikácie.

## 5. Mobil a prístupnosť

- CTA a polia majú dostatočnú veľkosť;
- klávesnica nezakrýva aktívne pole;
- fixné prvky neprekrývajú cookie lištu ani tlačidlo formulára;
- validácia vysvetľuje chybu pri konkrétnom poli;
- stránka nemá horizontálny overflow;
- obrázky majú zmysluplný alternatívny text a nenačítavajú sa rozbité.

## 6. Výkon a meranie

Rýchlosť znižuje trenie, ale neopraví nejasnú ponuku. Kontrolujeme veľkosť hero médií, fonty, JavaScript tretích strán, cache a Core Web Vitals. Obchodné meranie pritom oddeľuje:

- návštevu vstupnej stránky;
- klik na hlavné CTA;
- začatie formulára;
- uložený lead;
- kvalifikovaný dopyt;
- zákazku.

Reklamný klik nie je lead a analytická udalosť nie je zákazka.

## Verejný návod

Rozšírené vysvetlenie deviatich opráv, praktickú 30-minútovú kontrolu a FAQ nájdete v návode [Ako získať viac dopytov z firemného webu](https://cottoncloud.sk/ako-ziskat-viac-dopytov-z-firemneho-webu/?utm_source=github&utm_medium=referral&utm_campaign=firemny_web_leads_2026_09&utm_content=full_guide).

CottonCloud je slovenské WordPress a webdizajnové štúdio. Tento verejný checklist je informačný materiál, nie prísľub konkrétneho počtu dopytov alebo pozície vo vyhľadávaní.
