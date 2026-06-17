# Zkušenosti ze státních zkoušek – FI MUNI PVA

> Shrnutí zkušeností ze státnic nasbíraných z Discord komunity studentů FI MUNI.
> Obsahuje info o průběhu, komisích, chytácích a FAQ.
> ⚠️ **Generováno pomocí AI (Claude) z exportů Discord kanálu** – informace vycházejí ze zkušeností studentů, nikoli z oficiálních zdrojů. Vždy si ověř aktuální stav u garanta nebo na webu FI MUNI.

---

## ⚠️ Aktuální změny otázek PVA (2026)

> Stav k červnu 2026 – ověř aktuální seznam na: https://www.fi.muni.cz/studies/fe-bc/bc-pva.html

- Ze seznamu praktických otázek PVA byly **odstraněny 2 otázky**: Značkovací jazyky (XML) a Informační systémy (AIS)
- Přidána nová otázka z **PB007** (místo PV028) – zatím pro budoucí šablony, v červnu 2026 pravděpodobně ještě ne
- **Digitální systémy** rovněž v seznamu chybí
- Thason (garant PVA): „To tam pridame namiesto PV028... A to XML tiez zrevidujeme" (únor 2026)
- ❗ Pokud jdeš na státnice v červnu 2026, ověř si aktuální seznam – mohl se oproti materiálům z roku 2024–2025 lišit

---

## Obecné informace

- Úspěšnost na první pokus na jaře se pohybuje kolem **94 %** (podzimní termíny jsou nižší)
- Hodnocení: **V** (Výborně, zpravidla = A) nebo **P** (Prospěl, = B–E); V je vzácnější
- Výsledky (známky) přicházejí zpravidla **druhý den** po zkoušce do ISu
- **Délka celé SZZ:** ~40 min – přibližně 15 min obhajoba (8 min prezentace + 7 min rozbor posudků), 20 min ústní zkoušení, 5 min administrativa
- Statistiky průchodnosti (historické): https://is.muni.cz/auth/predmety/statistika_znamek?fakulta=1433;obdobi=9783;kod=SZB
- Komise si někdy **sama vybírá „nejtěžší podotázku"** z vylosované otázky – počítej s tím, že tě zaměří na obtížnější části
- Zkoušející může **odmítnout zkoušet stejnou otázku znovu** (pokud ji daný den zkoušel víckrát) – pak se losuje nová otázka

---

## Průběh zkoušení

- Někteří zkoušející (např. **Černá**) nechají studenta **si vybrat, čím chce začít**
- Zkoušející zpravidla nechají studenta **mluvit volně**, pak přerušují doplňujícími dotazy
- Pseudokód k algoritmům může být vyžadován – je dobré mít **základní pseudokódy naučené** (BFS, DFS, ...)
- Pokud si opravíš sám chybu (uvědomíš si omyl a opravíš ho), komise to bere pozitivně
- **Pořadí otázek závisí na komisi**: někteří nechají studenta vybrat (Kozlíková, Sojka, Křetínský); jiní kliknou obě najednou a pak ti dají vybrat; jiní sami řeknou pořadí
- **Máčka (fyzické lístečky s poznámkami)** jsou povoleny u komisí s **Hliněným** nebo **Přenosilem** – u ostatních nepočítej
- **Přípravný čas před odpovídáním: žádný** – po COVIDu zrušen, jdeš rovnou odpovídat (papír a tabule k dispozici ale jen při zkoušení samotném)
- **Po vylosování otázky** vidíš seznam pojmů z dané otázky na obrazovce – to je opora; nemusíš rawdoggovat zpaměti bez kontextu
- **Zkoušení probíhá česky/slovensky** (v jazyce studijního programu)
- **Kalkulačku na státnice nebrat** – výpočty po tobě chtít nebudou; stačí umět příklad z hlavy (determinant 2×2, max. jednoduchý integrál)
- Zkoušení probíhá cca od 8:00 do ~15–16 hodin; **jít první ráno = výhoda** (komise je svěží, jsou na to i studie)
- Jít jako první po obědě není ideální
- **Mluv co nejvíc** – chovej se jako prodejce auta, prodáváš to co umíš; verbální výkon hodně ovlivňuje výsledek
- Co je přímo v názvu/tématu otázky = musíš umět dobře; co se probralo jen v navazující diskuzi = volnější požadavky

---

## Přehled zkoušejících a jejich styl

### Barnat
- Zkoušel **informační bezpečnost**: nepopiratelnost → podpisy, certifikáty, certifikační autorita; celé zkoušení se točilo okolo podpisů
- Trochu vtipkuje, příjemný; když se student zasekl, snažil se navést
- Jako **oponent** (2025): jeden student poznamenal, že „se zamračil pokaždé, když jsem něco řekl" – Obdržálek / Barnat jako oponent je náročný

### Batko
- Zkoušel **architektury**: jak funguje procesor, z čeho se skládá, přepínání procesu (context switch), RISC vs CISC
- Zkoušel **informační bezpečnost**: bezpečné programování, síťové útoky
- Milý, snaží se pomáhat

### Beneš
- Zkoušel **popisnou statistiku** – dvě varianty:
  - *Náročná* (u složitějšího tématu): náhodný jev, elementární jev, distribuční funkce, funkce hustoty, vztah F(x)=P(X≤x); nakreslit rozdělení + DF + hustotu, přesné hodnoty na osách, správně zabarvenat kolečka u diskrétní DF; **táhne definici velmi dlouho i když je zjevné, že ji student neuvede**
  - *Přístupná* (jindy): distribuční funkce a různá rozdělení – **nechtěl vzorce, jen vysvětlit co znamenají**; při zaseknutí přeformuloval otázku; celkově friendly encounter
  - Na jakém intervalu je def. distribuční funkce? **(ℝ)**
- Zkoušel **grafové algoritmy**: definice nejkratší cesty, algoritmy (Dijkstra, Bellman-Ford – omezení), minimální kostra (definice, algoritmy); ohodnocený graf
- Zkoušel **funkcionální programování**: postup výpočtu / redukce, redukční kroky, vyhodnocení v různých strategiích, trochu Haskellu; příjemný, ochotný čekat na odpověď

### Brandejs
- Předseda komise – chilloval, zajímavé dotazy k bakalářce; do zkoušení nezasahoval

### Brázdil
- Zkoušel **matematickou analýzu**: limita (⚠️ – jeden student se ji naučil „obráceně"; Brázdil mu to řekl a nakonec dospěli ke správné odpovědi), derivace (y=ax+k → a je derivace), určitý integrál, Newton-Leibniz
- Zkoušel **sítě**: kódování na fyzické vrstvě, adresace, topologie, kolize a řešení (CSMA/CD, CSMA/CA – grilloval i na detailech, které jsou v materiálech jen okrajově!)
- Zkoušel **neuronové sítě** (INF): model neuronu, vnitřní potenciál, aktivační funkce, zpětná propagace
- Styl: **potrpí na formalismy** a přesná vyjádření; napovídá, má dobré analogie (spolupráce s Ručkou)
- „Brázdil je mega týpek, ale nenechá se ubullshitovat vařením z vody" – solid základy mu stačí, ale musí to být skutečné znalosti, ne plácání

### Bühnová
- Předsedkyně komise – příjemná, nechá studenta vybrat pořadí otázek
- Spokojená se základy, nechce velké detaily

### Byška
- Zkoušel **síťové aplikace**: jmenná služba (DNS), QoS (Leaky Bucket, Token Bucket), řízení přístupu, autentizace, asymetrická kryptografie
- Zkoušel **sítě**: TCP/IP vs ISO/OSI model, fyzická vrstva, kódování signálu, synchronizace
- Zkoušel **značkovací jazyky**: DOM (úrovně, výhody/nevýhody, využití v praxi), XML, namespaces, DTD vs XSD, XPath, XQuery a proč vzniklo
- Zkoušel **databáze**: relace, klíče, normální formy s příklady (kdy splňují/nesplňují danou NF a jak upravit); nepotřeboval přesné vyjadřování
- Zkoušel **OS**: architektury jádra (monolitické vs. mikrojádro), virtualizace (přeshouplo k Dockeru/kontejnerizaci), virtuální paměť – stránky a frames, plánování procesů vs. vláken
- Zkoušel **nízkoúrovňové** (INF): pamäťový model, segmenty, dynamická alokácia (funkcie, free 2×?), void pointer (veľkosť), ukazateľová aritmetika (void pointer neumí)
- Styl: jde po podotázkách, nechtěl přesné definice – zajímal ho obecný přehled a intuitivní vysvětlení

### Čeleda
- Milý; zkoušel BC základy; nenáročný

### Černá
- Nechává si student vybrat, čím začít
- Ptá se na **složitostní třídy** (PSPACE, NP-úplnost, Savitchova věta)
- U grafů chce BFS pseudokód + složitost, silně souvislé komponenty, lineární čas
- Aktivně **napovídá**, ale ne vždy úspěšně – očekává samostatné domyšlení
- Komise se domlouvá, co bude zkoušet – vedoucí navrhoval u složitosti PSPACE problémy

### Dohnal
- Předseda nebo zkoušující – příjemný; základy (databáze, SOA); naváděl

### Foltýnek
- Zkoušel **regulární jazyky**: Chomského hierarchie + pravidla gramatik pro jednotlivé typy, determinismus vs. nedeterminismus, NFA→DFA (2^n stavů – **chce odůvodnění: vznikají všechny podmnožiny stavů**)
- Styl: spíš testuje, jestli student zaslouží PV, než chce vyhodit; navádí ke správné odpovědi

### Furmanová
- Zkoušela **síťové aplikace, nízkoúrovňové programování, OOP**
- U nízkoúrovňového programování: začíná strukturou paměti programu (segmenty), pak dynamická alokace
- U sítí: ptá se na QoS, scheduling, congestion avoidance, autentizaci
- U OOP: chce vazby, dědičnost, polymorfismus, abstraktní třída
- Zkoušela **souborové systémy**: blokové zařízení, bloková vrstva, I/O scheduler, adresářová struktura (superblok, inode, datové bloky, bitmapy), B+ stromy (jak se používají v FS)
- Zkoušela **databáze**: relace, relační schéma, klíče (kandidátní, primární), funkční závislosti, 1./2./3. NF
- Upozornění: může si stěžovat, že „dneska je to už potřetí" – nenechej se vyvést z míry
- Pokud zmateš abstraktní třídu s ADT a pak se opravíš, bere to v pohodě

### Hladká
- Zkoušela (zmíněna bez detailů o stylu)

### Holub
- Milý; zkoušel **sítě** – chce přehled, základy

### Horák
- Zkoušel **složitost**
- Ptal se na: definice asymptotické složitosti, složitostní třídy a vztahy mezi nimi, P=NP, příklady problémů, NP-těžký vs NP-úplný
- Milý, pomáhal naváděním

### Chmelík
- Zkoušel **strukturu a řídení běhu programu**: předávání hodnot (hodnotou vs. referencí – odpověď „záleží" se mu líbila), výjimky, dědičnost, konstruktory v C#
- Zkoušel **informační bezpečnost**: identita a přístup (autentizace, hesla, biometrika, ACL), síťové útoky + prevence, digitální podpis, asymetrická kryptografie, použitelná bezpečnost (learnability, memorability…)
- Zkoušel **databáze**: relační model, schéma, klíče, relační algebra (selekce, projekce), 1NF/2NF/3NF (Boyce-Coddovu NE)
- Zkoušel **SQL**: SELECT příklad, cena vyhodnocování, indexy (jak fungují, kdy se nevyplatí – **malé tabulky!**), hashování
- Zkoušel **síťové aplikace**: SMTP, POP3 vs IMAP (IMAP kopíruje, POP3 přesouvá), FTP/SFTP/HTTP, DNS, QoS
- Styl: kývá hlavou při správných odpovědích, nechá dlouho mluvit, co konkrétně chce – zeptá se; **přátelský, dávají A**

### Jakubíček
- Zkoušel **SQL**: transakce, integritní omezení, cizí klíč, triggery, indexování, B+ stromy, hashování
- Pohodový, zajímá ho pochopení

### Jonáš
- Zkoušel **statistiku** (PVA i INF): uniformní diskrétní rozdělení (hod kostkou), funkce pravděpodobnosti, kumulativní distribuční funkce, normální rozdělení (parametry, hustota, CDF, převod derivací/integrálem)
- Zkoušel **grafové algoritmy**: minimální kostra + ukázat algoritmus, Dijkstra – jak funguje; reprezentace grafu v PC (matice sousednosti vs. seznam – výhody, kdy použít), DFS/BFS – jak fungují, k čemu slouží, barvení vrcholů
- Zkoušel **bezkontextové jazyky**: BK jazyk, zásobníkový automat, způsoby akceptování, uzávěrové vlastnosti
- Zkoušel **funkcionální programování**: princip výpočtu, redukční strategie (striktní vs. normální – rozdíl, ukázka na příkladu), funkce vyššího řádu (map), **implementovat `map` na tabuli** včetně typového předpisu
- Zkoušel **regulární jazyky**: definice jazyka + abecedy, Chomského hierarchie, reg. výrazy, DFA/NFA, determinizace (2^n stavů + odůvodnění: vznikají všechny podmnožiny stavů), uzávěrové vlastnosti + důkaz (produktový automat)
- Zkoušel **matematickou logiku** (INF): splnitelnost, tautologie, kontradikce; výroková + predikátová logika
- Styl: jde postupně od podotázky k podotázce, chce toho **hodně** – buď na to připraven; milý, trpělivý, nevychází ze své role

### Kopeček
- Matematik – někdy zákeřné otázky a nepříjemný; jindy studenty zachránil
- Nechce analytické odpovědi bez formálních definic

### Křenek
- Příjemný; základy

### Křetínský
- Zkoušel **lineární algebru**: vektorový prostor, skalární součin (geometrický význam, k čemu je), vlastní čísla a vektory, jejich geometrický význam (i ve 3D)
- Jako předseda: bývá ticho; po obhajobě se ptá výhradně na věci z ní

### Kuba
- Zkoušel **síťové aplikace**: SMTP, FTP/SFTP, HTTP, DNS; kryptografie – podpisování, certifikáty, symetrické + asymetrické šifrování
- Pohodář; předseda Sojka se ho doptával na věci z obhajoby

### Kučera
- Předseda komise – velmi milý; **záchrana ve stresu** – pokud vidí, že student panikuje, může převzít zkoušení a navodit ho
- Obecně do zkoušení nezasahuje, ale je záchranná síť

### Lexa
- Příjemný; v pohodě; základy

### Liška
- Zkoušel **nízkoúrovňové programování** (INF): co je pointer (chce přesné vyjádření), pamäťový model procesu, halda vs. stack (doplňovací otázka: přibližná velikost stacku), proč je stack menší než heap (stack se ukládá při context switchi)
- Nadšený z tématu bakalářky – rád by se ptal víc, ale nebyl čas

### Loutocký
- Zkoušel **kyberválku**: nechá studenta mluvit, pak se soustředí na atribuci a mezinárodní dohody (Budapestská úmluva); zmínka Stuxnetu mu stačí
- Milý, neklade zákeřné otázky

### Matěj
- Zkoušel **nízkoúrovňové programování**: nakreslit paměť programu, co je stack a co se tam ukládá, proč dynamická alokace, ukazatele, pointer aritmetika, co se stane při sčítání dvou pointerů, \0 na konci stringu
- Zkoušel **SQL**: nakreslit relaci, SELECT + JOIN, co je trigger, index, hashování; stačí hlavní myšlenka
- Zkoušel **informační bezpečnost**: základní pojmy (důvěrnost, integrita, dostupnost, nepopiratelnost), kryptografická primitiva, podpisy, certifikáty
- Zkoušel **architektury**: zdůrazňuje doplňkový kód jako „nejpoužívanější", parita, RISC/CISC

### Matula
- Předseda komise – zpravidla do zkoušení nezasahuje

### Mráková
- Příjemná; zkoušela **lineární algebru a grafy** (INF); trochu detailnější než průměr

### Musil
- Zkoušel **regulární jazyky**: definice jazyka, operace nad jazyky, definice gramatiky, Chomského hierarchie, příklady pravidel pro typ 3, automaty (DFA vs NFA – rozdíly, pětice)
- Zkoušel **matematickou analýzu**: derivace (co to je, nakreslit, popsat limitou, rovnice tečny), spojitost – funkce spojitá ale bez derivace (odpověď: |x|), neurčitý integrál = množina primitivních funkcí, otázky ohledně intervalů definice
- Začíná s pohoda otázkami, ale **když vidí, že student ví, jde nad rámec PVA** – buď na to připrav
- Hodně napovídá a táhne odpovědi ze studenta; příjemný

### Novotný
- Zkoušel **návrh algoritmů**: rozděl a panuj (definice + příklady), mergesort (ukázat rozdělení na tabuli + O(nlogn) přes rekurzivní strom; pseudokód pro mergesort **není nutný**), **pseudokód faktoriálu rekurzivně i iterativně** na tabuli
- Zkoušel **grafové algoritmy**: definice nejkratší cesty, kdy existuje, Dijkstra nebo Bellman-Ford na výběr + vysvětlit
- Zkoušel **stromové datové struktury**: BVS (hledání, worst case), samovyvažující BST (hlavní operace = rotace, ukázat a vysvětlit složitost), hloubka stromu → složitost
- Zkoušel **strojové učení** (INF): lineární regrese (příklad 2D, model, učicí algoritmus, chybová funkce, gradient descent)
- Styl: milý, přímočarý, poradí když si nepamatuješ → **kafedoruky mu děkuje za radu na grafech, bez níž by ho vyhodili**
- Pohodový

### Obdržálek

Komise, ve které byl: **Brim, Obdržálek, Rusnak** (2024) / **Černá, Obdržálek, Plhák** (2025)

**Statistika:** V jaru 2025 měl **0 % úspěšnost na první pokus** (potvrzeno z tabulky hodnocení komisí v Discord pinu). ⚠️ **Pozor:** tabulka komisí (CSV s 300+ recenzemi) ho ale popisuje jako příjemného a usměvavého – v mnoha případech hodnotil mírně a pomáhal. Pověst "nejhoršího examinátora" může být přehnaná; záleží na dni, komisi a tématu.

**Styl a přístup:**
- Zkoušel **složitost** (nejčastěji) i **lineární algebru** – není fixován jen na složitost!
- Začíná **od konce** – rovnou u NP-úplných úloh, přeskakuje základy (v případě složitosti)
- Vyžaduje **přesné vyjadřování a přesné definice** – to je klíčové!
  - Chce definice z **jeho** výukových materiálů, ne z IB110 nebo jiných předmětů. Pokud říkáš správně, ale jinými slovy než on zná, zamračí se.
  - Černá ho u jednoho studenta opakovaně umírňovala, že student říká vše správně
- Skončili u **polynomiální redukce**; chtěl důkaz, že SAT je NP-úplný (naštěstí netrval)
- Celkový dojem: Není hnusný, ale bez zkušeného předsedy komise (Černá) může být náročnější; „bez Černé bych ho mít nechtěl"
- Když pochopí, že student alespoň chápáním reaguje, je spokojený

**Co zkoušel – složitost:**
- NP-úplný problém – definice, příklady (Subset-sum, 3-SAT)
- Pojem problému (rozhodovací problém)
- NP-těžké vs. NP-úplné
- Redukce, polynomiální redukce – **přesná definice!**
- Důkaz NP-úplnosti SAT (Cook-Levin) – zmíní se, ale nemusí trvat

**Statistika s Obdržálkem:**
- Studenti, kteří ho měli v komisi, se **učili PMF/PDF/CDF nazpaměť pro každé rozdělení** – je known za to, že to chce. Přímá zkušenost: *"Ja som sa ucil tie funkcie naspamat, ale tak ja som mal Obdrzalka."*
- Brázdil (jiný zkoušující) má podobný přístup – taky zkouší vzorce distribucí do hloubky.

**Co zkoušel – lineární algebra (Pali11, únor 2026):**
- Determinant – co to je (definice), výpočet 2×2, Laplaceův rozvoj pro 4×4
- Co když je determinant nula? → inverzní matice, lineárně závislé vektory
- Praktické využití determinantu (chyták – student neznal)

**Tip:** Nauč se přesnou definici polynomiální redukce a NP-úplnosti ze státnicových materiálů (ne jen z IB110). Obdržálek chce slyšet konkrétní formulaci.

**Jako oponent (2025):** jeden student (adam4) popsal, že „oponent Obdržálek se pokaždé zamračil, když jsem něco řekl" – přestože komise byla hodná a pomáhala. Pokud je Obdržálek oponentem tvé BP, počítej s napjatou atmosférou při obhajobě.

### Ošlejšek
- Zkoušel **bezpečnost** (bezpečnostní funkce, řízení rizik, audit)
- Zkoušel **souborový systém**: RAID (0, 1, 5, 10), i-node, přístupová práva, co znamená executable bit na složce
- Zkoušel **síťovou bezpečnost**: Kerberos session, metody řízení přístupů, anonymita, digitální podpisy
- Zkoušel **AIS** (Aplikované informační systémy) – byl vidět, že neví co se ptát, šel od základů: architektura OS, procesy, vlákna, uváznutí; každou chvíli kontroloval čas
- Tip: u Ošlejška pomáhá kecání nonstop – jeden student přiznal, že „varil" u AIS 12 minut a zachránil ho objem slov

### Oujezský
- Zkoušel **souborové systémy**: blokové zařízení, RAID typy, souborové systémy, alokace; příjemný pohodář
- Zkoušel **sítě**: ISO/OSI + TCP/IP, MAC adresa (z čeho se konkrétně skládá), IP adresace; někdy pokládá nejasné otázky
- Styl: nechá mluvit, klid

### Pala
- ⚠️ Hnidopich na **gramatické chyby a překlepy v prezentaci** – zkontroluj texty BP před obhajobou!
- Při ústním zkoušení bývá tichý; u přesné definice může být vybíravý

### Pelánek
- Příjemný; ⭐ výhra v komisi
- Zkoušel **logiku, formální jazyky, statistiku** (INF); chce **příklady a intuitivní vysvětlení**
- U formálních jazyků zmínil diagonalizaci; u lingebry základy + příklady

### Pelikan
- ⚠️ **Detajlista** – chce podrobnosti; na segmentaci a stránkování jde do hloubky; OOP: eventy, konstruktory, C++ více než Java
- Zkoušel **SQL**: kategorie DDL/DML/DQL, CREATE TABLE na tabuli, INSERT, SELECT s WHERE, ACID; úplné základy
- Zkoušel **databáze**: relační model, typy klíčů, nakreslit relace s cizím klíčem, normální formy – pohodář
- Zkoušel **XML**: ⚠️ **chce XML + XSLT snippety na tabuli!** Pak DOM, příklady ke každé úrovni stromové struktury
- Zkoušel **OS**: typy architektur OS, virtuální paměť, stránkování, stránkovací tabulky – popsat + nakreslit překlad na příkladu, vypočítat velikost stránky
- Zkoušel **nízkoúrovňové programování**: ukazatele, dynamická alokace

### Pitner
- Zkoušel **funkcionální programování**
- Ptá se na: typy programovacích paradigmat → FP → způsob vyhodnocování → redukční strategie → příklad vyhodnocení různými strategiemi

### Plhák
- Zkoušel **databáze**: typy klíčů, normální formy (definice 3NF, BCNF už nechtěl), relační algebra na tabuli + normalizace do 3NF; relační schéma, operace (selekce, projekce, přejmenování), spojení – efektivní vyhodnocování
- Zkoušel **SQL**: integritní omezení, transakce, ACID, indexování
- Pohodář, jen úplné základy

### Polčák
- Předseda komise – příjemný; matematika; pomáhá

### Popelínský
- Příjemný; zkoušel **logiku a statistiku**; trochu nepředvídatelný; základy mu stačí

### Přenosil
- Předseda – bývá tichý, ale ⚠️ **pokud jsi nejistý nebo se zasekneš, může převzít zkoušení a jít do detailů!**
- Máčka povolena u komisí s Přenosilem

### Ráček
- Zkoušel **základy bezpečnosti**: základní bezpečnostní funkce (důvěrnost, integrita, dostupnost, nepopiratelnost), kryptografická primitiva – hash + příklad, symetrická a asymetrická kryptografie – jak fungují, kterou zvolit na dlouhý soubor
- Chce jen **velké základy**, neprohrabává se detaily

### Ručka
- Zkoušel **XML**: DOM, XML schema, atributy – základní pojmy, psaní na tabuli (základní věci)
- Zkoušel **nízkoúrovňové programování**: paměť programu, stack, halda, malloc/free/realloc, pointery, stránkování, jak malloc využívá stránkování
- Styl: nechá si student vybrat, čím začne; ptá se formou diskuse – příjemná forma
- Pokud student zamotá, chápe to a přeformuluje otázku

### Rudová
- Předsedkyně komise – milá, nezasahuje do zkoušení

### Rusňák
- Zkoušel **sítě**: ISO/OSI model + TCP/IP – vrstvy zdola nahoru, základní úlohy, adresace, zařízení; povrchní přehled stačí
- Zkoušel **souborové systémy**: co je souborový systém, blokové zařízení, I/O plánovač, šifrování disku, co je obyčajný soubor
- Zkoušel **strukturování a řízení běhu programu** (OOP): třída vs. objekt, kde se ukládá třída → klíčový pojem „**paměť programu**" (data/BSS segment); static atribut → datový segment; **nepřejde dál, dokud student neřekne správný pojem** – kroužil 10 minut (FialKate 🟥)

### Rychlý
- ⚠️ Pokud řekneš něco špatně, **viditelně se naštve** nebo se usměje slovy „no to není o tom si to zapamatovat" – nenervuj se, jen oprav
- Zkoušel **statistiku**: střední hodnota + výpočet, medián (chyták: **nutno nejdřív seřadit!**), rozptyl; chce vzorce i výpočet
- Zkoušel **grafy**: matematická definice grafu, stupeň vrcholu, strom (vztah vrcholů a hran), BFS (fronta) + ukázka na příkladu; může grillovat 15–20 minut
- Zkoušel **rozhodnutelnost**: co je algoritmus, sedmice Turingova stroje + přechodová funkce, Halting problem (vstup/výstup); navádí, přeruší tě uprostřed odpovědi (někdy to znamená, že jsi odpověděl dost)

### Řehák
- Zkoušel **statistiku**: definice distribuční funkce, nakreslit spojitou/diskrétní DF, hustota pravdepodobnosti (co je to?); komunikativní, přeformuluje otázku, nepotřebuje přesné pojmy, navádí
- Zkoušel **složitost**: složitost problému vs. algoritmu, C-těžký a C-úplný problém

### Safránek
- Zkoušel **grafové algoritmy**: definice nejkratší cesty, reprezentace grafů v PC + složitosti, Dijkstra, Bellman-Ford
- Zkoušel **stromové datové struktury**: BVS, složitosti, operace, RB stromy (pravidla + rotace – insert, rotace); stopne rychle když vidí, že to víš
- Zkoušel **matematickou analýzu**: **formální definice limity** (tvrdí, chce přesnou ε-δ formulaci), derivace (definice pomocí limity)
- Zkoušel **kombinatoriku** (INF): kombinace bez/s opakováním (definice + výpočet), proč vzorec takový je, permutace, variace, pravidlo součtu + součinu, princip inkluze/exkluze
- Tip: Pokud ukážeš, že to chápeš, i když chybí přesné slovo, řekne „je vidět, že to chápete" a přejde dál
- Poznámka: stále chtěl zkoušet praktickou otázku i u teoretické – sranda

### Sedmidubský
- Předseda komise (2025) – zpravidla nezasahuje do zkoušení
- Zkoušel **strukturování a řízení běhu programu** (OOP): mluvil jako kněz, příjemný; velmi trpělivý, dobře opravoval a naváděl dál

### Sochor
- Předseda – supermilý; organizační typ; vše připravil, upozorňoval na čas, snažil se student uvolnit

### Staudek
- Předseda komise – příjemný; dává rady a usměrňuje

### Strejček
- Zkoušel **matematickou analýzu** (spojitost funkce, limita, relace a zobrazení)
- Zkoušel **grafy**: BFS – byl naštvaný, protože to byl již 4. student s touto otázkou v jeden den; napsat pseudokód ocenil
- Zkoušel **statistiku**: střední hodnota, medián, rozptyl, korelace
- Zkoušel **složitost**: polynomiální redukce – chce **přesnou definici** (chyták!)
- Může odmítnout zkoušet stejnou otázku znovu → reroll

### Stupka
- Zkoušel **kyberválku**: nechá studenta mluvit, pak Stuxnet, atribuce, mezinárodní dohody
- Zkoušel **ochranu osobních údajů**: zákon o ochraně os. údajů v ČR, účel zpracování, co je osobní údaj; pseudonymizaci zná a ocení

### Sýs
- Zkoušel **výpočetní systémy**: číselné soustavy, záporná čísla – pozor: u pojmu „přímý kód" tě zastaví a chce pokračovat k doplňkovému; převody (16 ↔ 2), sčítání čísel
- Zkoušel **sítě**: zahájení/ukončení spojení, TCP vs UDP, ztráta paketu, ARQ
- Zkoušel **databáze**: relační model, relační schéma, integritní omezení, **nakreslit všechny joiny na tabuli!**
- Může se mračit, ale je v pohodě

### Trtík
- Zkoušel **matematickou analýzu** – byl **přísný**
  - Neurčitý integrál: chce odpověď, že je to **množina funkcí lišící se konstantou** (ne jen „primitivní funkce")
  - Relace a zobrazení: chce formální zápis
  - Derivace: jako tangenta v bodě – zmateného studenta peskoval, že se to učí na střední
  - Výpočet určitého integrálu: dal spočítat příklad
  - Navrhoval E/F i při znalosti základů – za analytiku jde tvrdo
- Zkoušel **návrh algoritmů**: rozděl a panuj, mergesort, pseudokód faktoriálu, tail rekurze (jak upravit rekurzi na tail-recursive?)
- Zkoušel **neuronové sítě** (INF): model neuronu, aktivační funkce (ReLU, sigmoida, step), ukázat síť na AND, vrstvy v MLP

### Vykopal
- Předseda komise (BCS) – po obhajobě se ptá na reálné využití projektu; nezákeřný

### Walletzký
- Příjemný; základy; bez zákerností

### Zezula
- Předseda nebo zkoušující – příjemný; nechává studenta dokončovat věty; pokud zkoušel, šel na DB/sítě základy

---

## Průběh zkoušení – doplňky

- **Psát a kreslit na tabuli je povoleno a doporučeno** – vždy jsou k dispozici tabule a fixky; prezentaci posílej den předem na technici@fi.muni.cz (do předmětu „SZZ Bc") + USB záloha!
- ⚠️ **Video v prezentaci → dej zálohu na USB!** Na zkušebním PC (.ppsx) videa nefungují – kafedoruky musel live přepnout na flešku, 17 s před limitem (místnost A217 potvrzeno)
- Výsledek se dozvíš **hned po zkoušení** – jdeš ven, komise se domluví (~3 min) a zavolá tě zpět
- **Tři známky**: 1) za bakalářku, 2) za zkoušení, 3) celková (průměr nebo přikloní se k jedné) → ovlivňuje červený diplom
- Opravný termín pro podzimní státnice: **až na jaře** společně s jarními; studium se pozastavuje
- Při opravném termínu komise nemusí být stejná (je to random); na opravném losujete **obě otázky znovu** (ne jen tu, co jste neudělali)
- Komise se při zkoušení dívá na hodiny – na jednu otázku je cca **10 minut**; ne vše z otázky bývá stihnuto
- Zkoušejícísi mohou **vyhazovat otázky**, které sami dobře neovládají → u konkrétního zkoušejícího se pak opakují otázky z jeho oblasti
- Pokud se student zasekne: zkoušející buď přejde na jiné téma, nebo „vytáhne" odpověď ze studenta
- Zkoušejicí jsou obecně friendly a **chtějí aby studenti prošli** – snaží se naváděním pomoci (Thason, insider)
- **⚠️ Generátor otázek**: v ISu klikej nejdřív jen na **první otázku**, na druhou až po vyzvání komisí! (tip od Hladké)
- Na státnice můžeš přijít přihlížet jako divák (veřejná zkouška) – přijď před začátkem

---

## Co vedlo k neúspěchu (oficální důvody z ISu)

Toto jsou reálné důvody zaznamenaných propadů (oficiální znění z ISu + zkušenosti z Discordu):

1. Neznalost principů operačního systému, synchronizace procesů a aplikačního rozhraní OS.
2. Neznalost základních pojmů a notace v teorii složitosti.
3. **Neznalost datové struktury HALDA** – nezná definici, neví k čemu ji lze použít, neovládá operace s haldou.
4. Neschopnost základních definic rekurzivních a rekurzivně spočetných jazyků.
5. Základní neznalosti v oblasti zabezpečení síťových aplikací.
6. **Neznalost Bellman-Fordova algoritmu.**
7. **Neznalost Dijkstrova algoritmu** pro hledání cest.
8. Neznalost pojmů variace, permutace.
9. Neznalost principů práce s pamětí – segment, stránkování, virtualizace.
10. Neschopnost demonstrovat surjektivní a injektivní zobrazení na dvou tříprvkových množinách.
11. Neznalost souvislosti binárních relací ekvivalence a rozkladů.
12. **Neznalost algoritmu DFS**, neznalost pojmu silně souvislá komponenta.
13. Neznalost pojmu relace, integritní omezení, neznalost B+ stromů.
14. Neznalost operace **modulární inverze** (modulární operace) v elementární teorii čísel.
15. **Neznalost pojmu O-notace**, neschopnost uvést korektní definici.
16. Neznalost pojmu podmíněná pravděpodobnost, neznalost **Bayesovy věty**.
17. Neschopnost vymezení základních pojmů **proces, vlákno** v kontextu operačních systémů.
18. Neznalost základních technik vyčíslitelnosti (**diagonalizace**, pojem částečné rozhodnutelnosti).
19. **Neznalost pojmu „paměť programu"** (text/data/BSS segment) – student věděl o stack a heap, ale neznal přesný název; Rusňák čekal 10 minut a nepřešel dál.
20. **Neznalost definice regulárního jazyka** – Devids10 (únor 2026): „Dostál som regulárne jazyky. Absolútny block. Ptal se jen co je regularny jazyk a co je jazyk." DFA/NFA/determinizaci by věděl, ale ani k tomu se nedostali.
21. Neznalost definice statistických rozdělení (statistika obecně – opakující se problém únor 2026).

---

## FAQ a chytáky

### Složitost – prostorová složitost a PVA

- **PSPACE na PVA**: V PVA otázkách je jen *"Složitostní třídy (P, NP)"*, zatímco INF má *"(P, NP, PSPACE)"* → PVA by PSPACE neměli muset znát do hloubky. Znalost neublíží, ale není primárně požadovaná.

### Grafové algoritmy – Dijkstra: složitost

- Složitost Dijkstry **záleží na implementaci prioritní fronty**:
  - Binární halda: **O((V + E) log V)**
  - Pole: **O(V²)**
  - Fibonacci halda: **O(E + V log V)**
  - Na státnicích stačí zmínit, že záleží na implementaci PQ, a uvést aspoň jednu variantu

### Regulární jazyky – minimalizace a kanonizace

- Determinizaci (NFA → DFA) zkoušeli; minimalizaci/kanonizaci **také mohou chtít** – není důvod proč ne. Doporučeno mít alespoň základní algoritmus v hlavě.

### Stromové struktury – Red-black tree delete

- Delete z RB stromu: mohou se zeptat, ale spíš jen na intuitivní popis (jak funguje); přesný pseudokód není typicky očekáván

### Matematická analýza – diferenciální rovnice

- Diferenciální počet je součástí otázky **na PVA**, ale hloubka záleží na komisi
- Konsenzus: stačí říct **co to je** (rovnice obsahující derivaci) a k čemu se používá; na PVA s největší pravděpodobností nebudou chtít řešit konkrétní diferenciální rovnici (na rozdíl od INF)
- Bezpečná odpověď: „diferenciální rovnice je rovnice, ve které se vyskytuje derivace funkce; používají se k modelování dynamických systémů"

### Lineární algebra – Gram-Schmidt, Cramerovo pravidlo, afinní transformace

- **Gram-Schmidt (ortogonalizace):** Pro INF povinné; pro PVA stačí vědět co to je, výpočet pravděpodobně nechtějí
- **Cramerovo pravidlo:** Doporučeno naučit se i jako PVA (řešení systému lin. rovnic přes determinanty) – není explicitně v otázce, ale Beneš nebo Ručka to mohou zmínit
- **Afinní transformace:** Pro PVA stačí říct: „je to jako vektorový prostor, ale rozšíření umožňuje i posun (translaci)" – nepotřebuješ detailní formalizmus
- **Výpočet vzdálenosti přímek a podobné:** Komise to typicky nechtějí; stačí základy

### Architektury / OS – cache a paměť

- **Cache coherence** – bylo skutečně zkoušeno na státnicích: *"Jak procesor zjistí, jestli je hodnota v cache správná?"* Jeden přístup: vedle hodnoty v cache se zapíše adresa v hlavní paměti a podle toho se ověří. Lze zmínit **MESI protokol** (zmíněn v materiálech k Výpočetním systémům; probraný podrobněji v IB109 Paralelní systémy).
- **TLB (Translation Lookaside Buffer)** – Rockai je šokovaný, když to student nezná; považuje za **common knowledge** (učí se na UNIX 1). Mít připraveno.

### Programovací jazyky – volba jazyka

- U otázek na principy programovacích jazyků / strukturování programu **si lze zvolit preferovaný jazyk** (C++, Python, …) – Java není povinná, pokud jsi v ní neprogramoval. Potvrď si to začátkem u zkoušejícího.

### Složitost

- **Je problém zastavení NP-hard?**
  NE. NP jsou podmnožina rozhodnutelných problémů. Halting problem je nerozhodnutelný → nemůže být NP-hard (může ale být NP-hard jen pokud je NP-hard definováno přes redukci, bez požadavku na příslušnost do NP). Přesněji: halting problem **není NP-complete**, ale technicky NP-hard by mohl být (NP-hard nevyžaduje příslušnost do NP). Dávej pozor na přesnou formulaci.

- **Je problém zastavení PSPACE-úplný?**
  CHYTÁK. PSPACE-úplnost se vztahuje jen na **rozhodnutelné problémy**. Halting problem je nerozhodnutelný → nemůže být PSPACE-úplný. Odpověď je NE.

- **Ekvivalent P=NP v prostorové složitosti?**
  Ze **Savitchovy věty** plyne, že NPSPACE ⊆ PSPACE (a tedy NPSPACE = PSPACE). Na rozdíl od časové složitosti zde víme, že nedeterminismus nepomáhá víc než kvadraticky.

- **Proč kvadraticky (Savitchova věta)?**
  Savitchova věta říká NSPACE(f(n)) ⊆ DSPACE(f(n)²). Myšlenka důkazu: rekurzivní „reach" algoritmus šetří paměť tím, že neukládá celou cestu, ale půlí problém – odpovídá myšlence, že rekurze s logaritmickou hloubkou šetří paměť.

- **Jsou regulární jazyky v PSPACE?**
  ANO. Regulární jazyky jsou rozhodnutelné v lineárním čase → tedy i v polynomiálním prostoru → patří do PSPACE.

- **SAT a PSPACE**
  SAT je NP-úplný, ale také leží v PSPACE (NP ⊆ PSPACE).

### Matematická analýza

- Neurčitý integrál = **množina funkcí lišící se konstantou** (ne jen „primitivní funkce") – Trtík toto vyžaduje
- Relace vs. zobrazení: umět **formálně zapsat** – funkce je relace F ⊆ A×B taková, že pro každé a existuje nejvýše jedno b s (a,b) ∈ F
- Derivace: umět popsat jako tangenta v bodě (na pravouhlém trojúhelníku)
- Mít připravený výpočet jednoduchého určitého integrálu

### Grafy

- U BFS je dobré znát **pseudokód** a složitost O(V+E)
- K DFS se ne vždy dostane, ale je dobré být připraven
- Silně souvislé komponenty v lineárním čase: **Kosarajův nebo Tarjanův algoritmus** – znát alespoň existenci a princip
- Minimální kostra: znát Kruskalův nebo Primův algoritmus; kostra grafu s n vrcholy má **n−1 hran** (ne 2^n!)
- Dijkstra + Bellman-Ford: obojí povinné – padají jako důvody propadnutí

### OOP

- Nezaměňovat **abstraktní třídu** s **ADT (abstraktním datovým typem)** – jsou to různé věci
- Vazby: statické vs. dynamické – umět obsáhle vysvětlit

### Nízkoúrovňové programování

- Struktura paměti programu: segmenty (text, data, BSS, heap, stack)
- Dynamická alokace: heap, příklady použití
- Datová struktura pro neznámou velikost bez časté realokace → **linked list**

### Síťové aplikace

- QoS: scheduling (fronta, prioritizace) a congestion avoidance; znát **Leaky Bucket a Token Bucket**
- Autentizace: symetrické a asymetrické **challenge-response protokoly**
- Jmenná služba (DNS): jak se resolvují adresy

### Databáze

- Typy klíčů (primární, cizí, unikátní, …)
- Normální formy: 1NF, 2NF, **3NF** (definice), BCNF – mít alespoň intuici
- Relační algebra na tabuli: příklady jako SELECT jmen studentů s věkem > 30
- **ACID**: atomičnost, konzistence, izolace, trvalost – umět vysvětlit

### Popisná statistika – chytáky

- **Kombinatorika, pravděpodobnost, Bayesova věta jsou pro PVA nevyžadovány** – jsou jen u INF. PVA má jen popisnou statistiku, rozdělení pravděpodobnosti, apod.
- Distribuční funkce: definovaná na celém **ℝ**, ne jen na (0,1)
- U diskrétní distribuční funkce: správně zabarvenat kolečka (filled = ≤, open = <)
- Beneš u statistiky táhne definici dlouho i při očividném neúspěchu studenta

### Quicksort / Merge sort

- Pseudokód není třeba znát zpaměti – lze „uvařit" na místě (QS, MS ano; RB-delete ne)
- Matematické příklady: max jednoduchý integrál – není třeba se učit rozklad na parciální zlomky

### Klíčový tip od Thasona (garanta PVA)

> „Prvá vec, co sa treba učiť je odpoveď na 'Co to je?' ... aspoň *nejakú* odpověď."

- U každého klíčového slova v otázce mej připravenou **alespoň jednu větu definici** – i když neformální
- Devids10 (🟥, únor 2026) selhal výhradně proto, že neodpověděl na „co je regulárny jazyk?" a komisař ho nepustil dál
- Platí pro všechny okruhy: komise začíná od začátku otázky a chce definici prvního pojmu

### Regulární jazyky – NFA → DFA

- Kolik stavů může mít DFA po determinizaci NFA s n stavy? **2^n** (horní mez)
- Proč 2^n? **Odůvodnění**: při determinizaci vznikají stavy odpovídající podmnožinám stavů NFA → nejvýše 2^n podmnožin
- Foltýnek a Jonáš chce toto odůvodnění, nestačí jen říct 2^n

### Databáze – indexy

- Index se nevyplatí na **malých tabulkách** (overhead na procházení indexu > sekvenční sken)
- Chmelík se na to specificky ptá

### Síťové aplikace – DNS a TLS

- **DNS**: znát celý strom (kořen, TLD, doménové servery), iterativní vs. rekurzivní překlad; Bártek vyžaduje přesný popis jak se mapuje jméno na IP (chyták – nestačí říct „hierarchický strom")
- **TLS/HTTPS handshake**: přibližně jak funguje navázání spojení (asymetrické šifrování k dohodnutí symetrického klíče); Bártek se na to ptal do hloubky

### Stromové datové struktury – BVS

- U BVS nestačí říct „≤ vlevo, > vpravo" – chcí slyšet, že **levý podstrom obsahuje menší prvky, pravý větší**
- Světylko: komise nebyla spokojená jen s nerovností
- Halda: umět přidat prvek (probublání nahoru)

---

## Studijní zdroje a nástroje

### Materiály k PVA státnicím

- **Google Drive – PVA materiály (2024, cross-checked):**
  https://drive.google.com/drive/folders/1jUZXBaV9Y5RdWVB2jKdWe64yTE27nfO_
  *(vypracovány skupinou studentů, cross-checkované s materiály předmětů; někde mohou být starší verze otázek)*

- **Marvavovy ZIP soubory (jaro 2024):** sdíleny na Discordu – praktické i teoretické otázky, s příklady z MGR přijímaček. Odkaz v pinech Discord kanálu.

- **Quizlet kartičky (PVA):** https://quizlet.com/user/rendaur/sets
- **Quizlet kartičky (INF/obecné):** https://quizlet.com/user/Informatici/sets

- **Seznam otázek PVA 2018:** https://www.fi.muni.cz/studies/fe-bc/bc-pva2018.html

### Generátor losování otázek

- **Ostrý generátor (IS MUNI):**
  https://is.muni.cz/auth/do/fi/SO/
  https://is.muni.cz/auth/do/fi/SO/losovani_otazek_bc_SZZ.html
  *(Tip: klikej nejdřív jen na první otázku, na druhou až po vyzvání komisí!)*

### Procvičování

- **Mikroprogramování – KSI úloha:** https://ksi.fi.muni.cz/ulohy/755
- **SQL + OpenMP/MPI dojo cvičení** (Skoupý, 2026) – praktická cvičení na státnicové otázky:
  https://gitlab.fi.muni.cz/xskoupy1/dojo-collection
  *(Vhodné jako příprava na SQL a paralelní systémy; v tabulce komisí se prý na OpenMP ptali)*
- **Kyber materiály (2024)** – vypracované otázky 12. Bezpečnostní architektura + další:
  https://drive.google.com/drive/folders/1WWfWzAZkNJ0Fwbjpg2CbO3O2oEdZRqQT?usp=sharing

### Sítě – YouTube série

- **Výborná série na sítě** (Segmentation fault, 05/2026 – doporučeno, sám si vytáhl sítě a prošel v klidu):
  https://www.youtube.com/watch?v=a5SMTyhn0U8
  *(Pokud jdeš na sítě od nuly nebo slajdy nefeelují – tohle je záchrana)*

### Výuková videa a skripta

- **Thasonovo video k obhajobě:** (odkaz v pinech Discord kanálu `#szb-statni-zaverecna-zkouska`)
- **Slides z MA007 (logika):** https://www.fi.muni.cz/usr/kucera/teaching.html
- **Skripta/sbírka z PB016 (logika):** https://is.muni.cz/www/pyty/57307760/sbirka.pdf
- **IB015 přednáška (FP, redukční strategie):** https://is.muni.cz/auth/el/fi/podzim2022/IB015/um/prednasky/IB015_05.pdf

### Soubory PDF ke stažení

- **12 – AIS (aplikované informační systémy)**, sepsáno valgrinderror podle Račkovy přednášky:
  https://cdn.discordapp.com/attachments/673515003017691181/1450130197520318636/12-ais.pdf
  *(19 záložek, pokrývá co přesně Ráček chce slyšet; prosinec 2025)*

- **13 – Digitální systémy**, sepsáno valgrinderror:
  https://cdn.discordapp.com/attachments/673515003017691181/1452830158686912552/13-digitalni_systemy.pdf
  *(hlavně postupy, které v jiných materiálech chybí; prosinec 2025)*

### Foto z promocí

- **PVA A-Ko OneDrive (říjen 2025):** https://1drv.ms/f/c/c7b60faaece64bec/IgBw77Ek-WAKTL0tPCvegAg_AX26p6t4RlwGO9T559RBFMI?e=aVf6oG
  *(sdílí jijik_hal, přístup přes pozvánku)*
