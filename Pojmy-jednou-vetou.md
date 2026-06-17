# Pojmy jednou větou

> Kontrolní seznam **ke každému pojmu z [[Otazky]]** – jedna věta / intuice. Slouží k poslednímu ujištění před zkouškou, že ke každému slovu z otázky umíš aspoň „co to je" (Thasonův tip). Detaily v souborech `teoreticke/` a `programove/`.

---

# Teoretické základy

## 1. Lineární algebra
- **Vektor** – uspořádaná n-tice čísel; má směr a velikost.
- **Matice** – obdélníkové schéma čísel; reprezentuje lineární zobrazení nebo soustavu rovnic.
- **Operace s vektory** – sčítání po složkách, skalární součin (→ číslo), vektorový součin (ve 3D → kolmý vektor).
- **Operace s maticemi** – sčítání (stejné rozměry), násobení (řádek × sloupec), transpozice (překlopení přes diagonálu).
- **Gaussova eliminace** – převod matice na schodovitý tvar řádkovými úpravami, slouží k řešení soustav rovnic.
- **Inverzní matice $A^{-1}$** – matice, pro kterou $A A^{-1} = E$; existuje jen pro regulární matice ($\det \neq 0$).
- **Determinant** – číslo čtvercové matice udávající orientovaný objem; $=0$ znamená singulární matici (lin. závislé vektory, žádná inverze).
- **Lineární operace** – zachovává sčítání a násobení skalárem ($L(x+y)=L(x)+L(y)$, $L(\alpha x)=\alpha L(x)$).
- **Skalární součin** – součin vektorů dávající číslo; $=0$ znamená kolmost, umožňuje počítat délky a úhly.
- **Vektorový podprostor** – podmnožina prostoru uzavřená na lineární kombinace (sama je vektorovým prostorem).
- **Vektorová báze** – množina lin. nezávislých vektorů generujících celý prostor; jejich počet = dimenze.
- **Lineární transformace** – zobrazení zachovávající operace s vektory (otočení, škálování, projekce…).
- **Matice zobrazení** – matice transformace; vznikne aplikací zobrazení na vektory standardní báze (výsledky = sloupce).
- **Vlastní vektor** – vektor, jehož směr se transformací nemění, jen se škáluje.
- **Vlastní číslo $\lambda$** – kolikrát se vlastní vektor natáhl/smrštil/otočil ($Av=\lambda v$).
- **Geometrický význam vl. čísel/vektorů** – osy, podél nichž transformace jen škáluje.

## 2. Základy matematické analýzy
- **Relace** – libovolná podmnožina kartézského součinu množin.
- **Zobrazení** – relace přiřazující každému prvku nejvýše jeden; **injektivní** (prosté), **surjektivní** (na), **bijektivní** (oboje).
- **Reálná funkce** – zobrazení mezi číselnými množinami; má definiční obor, obor hodnot, sudost/lichost, periodicitu, omezenost.
- **Polynom** – výraz $a_n x^n + \dots + a_0$; kořen je $x$, pro který $P(x)=0$.
- **Limita** – hodnota, k níž se funkce blíží v daném bodě; existuje, když si jsou rovny obě jednostranné limity.
- **Spojitá funkce** – v každém bodě se funkční hodnota rovná limitě ($\lim_{x\to x_0}f(x)=f(x_0)$); nakreslíš ji bez zvednutí tužky.
- **Derivace** – směrnice tečny ke grafu; okamžitá rychlost změny funkce (limita podílu přírůstků).
- **Neurčitý integrál** – množina primitivních funkcí (opak derivace), lišících se o konstantu, bez mezí.
- **Určitý integrál** – orientovaná plocha pod grafem na intervalu $[a,b]$.
- **Geometrický význam** – derivace = sklon tečny; integrál = obsah plochy.

## 3. Popisná statistika
- **Popisná statistika** – kvantitativně popisuje data (statistický soubor), nezobecňuje na populaci.
- **Aritmetický průměr** – součet hodnot / jejich počet; citlivý na extrémy.
- **Medián** – prostřední hodnota seřazených dat (50. percentil); odolný vůči extrémům.
- **Rozptyl** – průměrná kvadratická odchylka od průměru ($\sigma^2$); jeho odmocnina = směrodatná odchylka.
- **Korelace** – síla a směr lineárního vztahu dvou veličin (koeficient $\in \langle -1,1\rangle$).
- **Odhad statistiky** – **bodový** (jedno číslo) nebo **intervalový** (konfidenční interval s danou spolehlivostí).
- **Spolehlivost odhadu** – konfidenční interval $100(1-\alpha)\%$: v něm parametr leží s pravděpodobností $1-\alpha$.
- **Náhodná veličina** – funkce přiřazující výsledkům pokusu čísla.
- **Distribuční funkce $F(x)=P(X\leq x)$** – pravděpodobnost, že veličina nepřekročí $x$; definovaná na celém $\mathbb{R}$, neklesající, od 0 do 1.
- **Rozdělení náhodné veličiny** – předpis pravděpodobností; diskrétní (skoky, např. binomické, Poissonovo) vs. spojité (hustota, např. normální).
- **Příklady rozdělení** – rovnoměrné (kostka), binomické (n pokusů), normální (zvonovka $N(\mu,\sigma^2)$).

## 4. Grafy a jejich prohledávání
- **Graf** – dvojice $(V,E)$: vrcholy a hrany (spojnice mezi nimi).
- **Typy grafů** – cesta, kružnice, **úplný** (vše propojeno), **bipartitní** (dvě skupiny, hrany jen mezi nimi), strom.
- **Strom** – souvislý acyklický graf; mezi dvěma vrcholy vede právě jedna cesta, má $n-1$ hran.
- **Stupeň vrcholu** – počet hran z vrcholu; součet stupňů = dvojnásobek počtu hran.
- **Orientovaný graf** – hrany mají směr (šipky).
- **Reprezentace grafu** – **matice sousednosti** ($V^2$, husté grafy, test hrany $O(1)$) nebo **seznam následníků** ($V+E$, řídké grafy).
- **DFS (do hloubky)** – zanoří se co nejdál do větve, pak se vrací; zásobník/rekurze, $O(V+E)$.
- **BFS (do šířky)** – prochází po vrstvách pomocí fronty; najde nejkratší cestu v neohodnoceném grafu, $O(V+E)$.
- **Využití prohledávání** – DFS: cykly, topologické uspořádání, silné komponenty; BFS: nejkratší cesta, bipartitnost.
- **Komponenta souvislosti** – maximální skupina vzájemně dosažitelných vrcholů; **silná** (s orientací) vs. **slabá**.

## 5. Grafové algoritmy
- **Ohodnocený graf** – každá hrana má váhu (číslo).
- **Nejkratší cesta** – cesta s minimálním součtem vah mezi dvěma vrcholy; každá její podcesta je též nejkratší.
- **Minimální kostra (MST)** – strom propojující všechny vrcholy ($n-1$ hran) s nejmenším součtem vah.
- **Relaxace hrany** – zlepšení odhadu vzdálenosti vrcholu, pokud přes hranu vede kratší cesta.
- **Dijkstrův algoritmus** – nejkratší cesty z jednoho vrcholu, přes prioritní frontu; jen **nezáporné** hrany.
- **Bellman-Fordův algoritmus** – nejkratší cesty i se **zápornými** hranami; umí detekovat záporný cyklus, $O(V\cdot E)$.
- **Kruskalův algoritmus** – MST: hladově přidává nejlevnější hrany bez vzniku cyklu (union-find).
- **Jarníkův (Primův) algoritmus** – MST: od jednoho vrcholu přidává nejlevnější hranu ven z komponenty.

## 6. Stromové datové struktury
- **Binární vyhledávací strom (BVS)** – uzly se 2 potomky, kde levý podstrom má menší a pravý větší klíče.
- **Vyvážený BVS** – listy ve zhruba stejné hloubce → operace $O(\log n)$; vyvažuje se rotacemi.
- **B-strom** – n-ární vyvážený strom (uzel s $k$ klíči má $k+1$ potomků); méně čtení z disku → databáze.
- **B+ strom** – B-strom s daty jen v listech, listy propojené pro rychlé sekvenční čtení → souborové systémy.
- **Červeno-černý strom** – samovyvažující BVS s barvami uzlů, garantuje výšku $\leq 2\log_2(n+1)$.
- **Rotace** – lokální přestavba stromu v $O(1)$, zachová uspořádání, použije se při vyvažování.
- **Halda (heap)** – binární strom, kde rodič je vždy větší (max-halda) / menší (min-halda) než synové; implementuje prioritní frontu.
- **Operace haldy** – insert a odebrání kořene $O(\log n)$ probubláváním; stavba $O(n)$.
- **Hashovací tabulka** – klíče mapuje hashovací funkce; kolize řeší zřetězení nebo otevřená adresace.
- **Složitost operací** – vyvážené stromy $O(\log n)$, nevyvážený BVS až $O(n)$, hash průměrně $O(1)$.

## 7. Návrh algoritmů
- **Rozděl a panuj** – rekurzivně rozděl problém, vyřeš části, spoj výsledky (divide–conquer–combine).
- **Rekurze** – funkce volá sama sebe až k zarážce (triviálnímu případu).
- **Výhody rekurze** – čitelný, krátký zápis odpovídající definici problému.
- **Nevýhody rekurze** – paměťová náročnost (zásobník, stack overflow), často pomalejší.
- **Odstranění rekurze** – nahrazení cyklem + explicitním zásobníkem; tail-rekurzi optimalizuje kompilátor.
- **Merge sort** – rozděl a panuj, $O(n\log n)$, stabilní, není in situ.
- **Quicksort** – pivot rozdělí pole, rekurze na obě části; průměrně $O(n\log n)$, nejhůř $O(n^2)$.
- **Heapsort** – opakované odebírání kořene haldy, $O(n\log n)$, in situ, nestabilní.
- **Matematická indukce** – důkaz přes bázi + indukční krok ($T(k)\Rightarrow T(k+1)$).
- **Vztah rekurze a indukce** – jdou opačně: indukce začíná u báze a postupuje výš, rekurze směřuje dolů k bázi.

## 8. Funkcionální programování
- **Funkcionální paradigma** – program je výraz, výpočet = jeho postupné zjednodušování; čisté funkce a imutabilita.
- **Redukční krok** – jedno nahrazení podvýrazu jednodušším.
- **Redukční strategie** – pravidlo, který podvýraz redukovat dál: **striktní** (zevnitř, nejdřív argumenty), **normální** (zvenčí), **líná** (normální + pamatování výsledků).
- **Vlastnosti strategií** – striktní je nejméně bezpečná (nejdřív se zacyklí), normální nejbezpečnější; výsledek je vždy stejný (Church-Rosser).
- **Funkce vyšších řádů** – berou funkci jako argument nebo ji vrací (`map`, `filter`, `fold`).
- **Nepojmenovaná (lambda) funkce** – funkce bez jména definovaná na místě: `\x -> x*x`.
- **Haskell** – čistě funkcionální, staticky typovaný, líné vyhodnocování.
- **Elementární programování v Haskellu** – pattern matching, rekurze nad seznamy, typové předpisy.

## 9. Regulární jazyky
- **Formální jazyk** – množina slov nad abecedou $\Sigma$.
- **Chomského hierarchie** – vnořené třídy gramatik: typ 0 (frázové, Turingův stroj), typ 1 (kontextové), typ 2 (bezkontextové, zásobníkový automat), typ 3 (regulární, konečný automat).
- **Regulární jazyk** – jazyk rozpoznatelný konečným automatem / popsaný regulárním výrazem.
- **Reprezentace a převody** – gramatika ↔ konečný automat ↔ regulární výraz (mají stejnou sílu, Kleeneho věta).
- **DFA** – deterministický konečný automat; každá dvojice (stav, symbol) → právě jeden stav.
- **NFA** – nedeterministický automat; přechod do množiny stavů, slovo přijato, dovede-li aspoň jedna větev do koncového stavu.
- **Determinizace** – převod NFA na DFA podmnožinovou konstrukcí (až $2^n$ stavů, protože vznikají všechny podmnožiny stavů).
- **Uzávěrové vlastnosti** – regulární jazyky jsou uzavřené na sjednocení, průnik, doplněk, zřetězení, iteraci, reverzi.

## 10. Rozhodnutelnost
- **Algoritmický problém** – problém zadaný výpočetnímu zařízení (doména instancí + požadovaný výstup).
- **Algoritmus** – konečná posloupnost elementárních kroků s jasným vstupem a výstupem.
- **Turingův stroj** – konečný automat s nekonečnou páskou; formální model „čehokoli vyčíslitelného".
- **Problém zastavení (Halting)** – rozhodnout, zda daný TS nad daným vstupem zastaví; **nerozhodnutelný**.
- **Rozhodnutelnost** – existuje **úplný** TS, který slova s vlastností přijme a ostatní zamítne (nikdy necyklí).
- **Částečná rozhodnutelnost** – TS požadovaná slova přijme, ostatní zamítne **nebo cyklí**.
- **Nerozhodnutelnost** – žádný úplný TS pro daný problém neexistuje.
- **Metoda redukce** – převod problému $P_1$ na $P_2$; je-li $P_1$ nerozhodnutelný a $P_1 \leq P_2$, je i $P_2$ nerozhodnutelný.

## 11. Složitost
- **Časová složitost algoritmu** – počet kroků nejdelšího výpočtu pro vstup dané velikosti.
- **Časová složitost problému** – složitost nejlepšího (optimálního) algoritmu, který problém řeší.
- **Asymptotická notace** – $\mathcal{O}$ horní odhad, $\Omega$ dolní, $\Theta$ těsný (oba).
- **Třída P** – problémy řešitelné deterministicky v polynomiálním čase.
- **Třída NP** – řešitelné nedeterministicky v polynomiálním čase; ekvivalentně mají polynomiálně ověřitelný certifikát.
- **Vztah P a NP** – $P \subseteq NP$; otevřená otázka, zda $P = NP$.
- **NP-těžký** – na problém se polynomiálně redukuje každý problém z NP (sám nemusí být v NP).
- **NP-úplný** – NP-těžký a zároveň v NP (nejtěžší problémy NP).
- **Polynomiální redukce $L_1 \leq_p L_2$** – funkce v polynomiálním čase s $w\in L_1 \iff f(w)\in L_2$.
- **NP-úplné úlohy** – příklady: SAT/3-SAT, problém batohu, obchodní cestující, vertex cover, subset-sum.

---

# Programové, výpočetní a informační systémy

## 1. Podprogramy a OOP
- **Podprogram** – pojmenovaný blok kódu; **funkce** vrací hodnotu, **procedura** ne.
- **Rozsah jmen (scope)** – oblast viditelnosti proměnné; **statický** (dle struktury kódu) vs. **dynamický** (dle volání).
- **Předávání hodnot** – **hodnotou** (kopie) nebo **odkazem/referencí** (sdílení, efektivní, riziko aliasů).
- **Výjimka** – objekt s informací o chybě, propaguje se po zásobníku k handleru (`try-catch`).
- **OOP** – paradigma s objekty (data + metody); principy abstrakce, zapouzdření, dědičnost, polymorfismus.
- **Zapouzdření** – spojení dat a operací + řízení přístupu (`private`/`public`); skrytí vnitřku.
- **Dědičnost** – nová třída přebírá členy rodičovské, rozšiřuje ji.
- **Polymorfismus** – jeden interface, různé chování; přetěžování (ad-hoc), generika (parametrický), override (podtypový, vybrán za běhu).
- **Implementace polymorfismu** – tabulka virtuálních metod (vtable): objekt nese ukazatel na metody své třídy → pozdní vazba.

## 2. Principy nízkoúrovňového programování
- **Paměťový model programu** – segmenty: text (kód), data/BSS (globální proměnné), halda (dynamická), zásobník (lokální + návratové adresy).
- **Správa paměti** – statická (za překladu) vs. dynamická (za běhu na haldě).
- **Nízkoúrovňová práce s pamětí** – přímý přístup přes adresy, `malloc`/`free`, bez kontroly mezí.
- **Ukazatel** – proměnná obsahující adresu do paměti; `&` vezme adresu, `*` dereferencuje.
- **Pole** – souvislý blok prvků; meze se nehlídají (přístup mimo = segfault).
- **Ukazatelová aritmetika** – posun ukazatele po prvcích podle typu (`p+3` = 4. prvek).
- **Uživatelské datové struktury** – `struct` (záznam položek), `union` (sdílená paměť), `enum` (výčet).

## 3. Nízkoúrovňové výpočetní architektury
- **Číselné soustavy** – poziční zápis čísla v dané bázi; 1 hex číslice = 4 bity, 1 oct = 3 bity.
- **Zobrazení celého čísla** – **doplňkový kód** (nejrozšířenější): záporná = negace bitů +1, jedna nula.
- **Aritmetika** – sčítání/odčítání v doplňkovém kódu bez korekcí.
- **Detekční kódy** – odhalí chybu: paritní bit, checksum, CRC.
- **Opravné kódy** – opraví chybu: ztrojení, Hammingův kód.
- **Obvody** – hradla (AND, OR, NOT, XOR…) složená z tranzistorů, bez paměti.
- **Paměti** – registry (nejrychlejší, na čipu), RAM (volatilní), ROM (permanentní), cache.
- **Procesor** – synchronní stroj řízený řadičem; vykonává instrukce dle čítače instrukcí (PC).
- **Programování / mikroprogramování** – instrukce realizovány sekvencí mikroinstrukcí v mikroprogramové paměti.
- **RISC** – málo jednoduchých instrukcí pevné délky, rychlý běh, více kódu (ARM).
- **CISC** – velký instrukční set, kompaktní kód, složitější instrukce (x86).
- **Vyrovnávací paměť (cache)** – rychlá paměť mezi CPU a RAM; L1/L2/L3, algoritmy LRU/LFU.

## 4. Databáze
- **Relační model** – data jako $n$-ární relace (tabulky), založen na predikátové logice.
- **Relační schéma** – soubor relací (struktura databáze).
- **Klíče** – **superklíč** (unikátní množina atributů), **kandidátní** (minimální superklíč), **primární** (vybraný kandidátní), **cizí** (klíč z jiné relace, tvoří vazbu).
- **Relační algebra** – procedurální jazyk nad relacemi: **selekce** (řádky), **projekce** (sloupce), **agregace**, **přejmenování**, **spojení (join)**.
- **Funkční závislost** – hodnota jedněch atributů jednoznačně určuje hodnotu jiných.
- **1NF** – atributy atomické (žádné vícehodnotové sloupce).
- **2NF** – 1NF + žádný neklíčový atribut nezávisí jen na části složeného klíče.
- **3NF** – 2NF + žádný neklíčový atribut nezávisí na jiném neklíčovém (žádné tranzitivní závislosti).
- **Boyce-Coddova NF (BCNF)** – přísnější 3NF: levá strana každé závislosti je superklíč.
- **Normalizace / dekompozice** – rozklad schématu do vyšších NF kvůli odstranění redundance a anomálií.

## 5. SQL, transakce a dotazy
- **Syntaxe a sémantika SQL** – deklarativní jazyk; říkáš *co* chceš, ne *jak* to získat.
- **Dotazování** – `SELECT ... FROM ... WHERE`; aktualizace `INSERT`/`UPDATE`/`DELETE`.
- **Agregační funkce** – `COUNT`, `SUM`, `AVG`, `MIN`, `MAX` (často s `GROUP BY`).
- **Trigger** – akce automaticky spuštěná při události (insert/update/delete).
- **Uložená procedura** – pojmenovaný kód uložený a vykonávaný na serveru.
- **Integritní omezení** – pravidla na data (primární/cizí klíč, NOT NULL, UNIQUE, CHECK).
- **Transakce** – nedělitelná posloupnost operací; vlastnosti **ACID** (atomičnost, konzistence, izolace, trvanlivost).
- **Vyhodnocování dotazu** – optimalizátor hledá nejlevnější plán (náklady = počet čtení z disku).
- **Index** – pomocná struktura (často B+ strom) pro rychlé vyhledávání; nevyplatí se na malých tabulkách.
- **Hašování** – mapování klíče na pozici hash funkcí, rychlý přístup k záznamu.

## 6. Operační systémy
- **Architektura OS / jádra** – **monolitické** jádro (vše pohromadě) vs. **mikrojádro** (minimum v jádře, služby v user space).
- **Režimy procesoru** – privilegovaný (kernel) vs. uživatelský (omezený přístup).
- **Programovací rozhraní / knihovny** – systémová volání + knihovny zpřístupňující služby OS aplikacím.
- **Přístupová práva** – kontrola, kdo smí číst/zapisovat/spouštět (uživatelé, skupiny).
- **Virtualizace** – běh izolovaných prostředí (VM, kontejnery) na jednom HW.
- **Virtuální paměť** – každý proces vidí souvislý adresní prostor, mapovaný na fyzickou paměť.
- **Proces** – běžící program s vlastní pamětí; **vlákno** – odlehčený běh sdílející paměť procesu.
- **Stránkové tabulky** – překlad virtuálních adres na fyzické (po stránkách).
- **Plánování** – plánovač rozhoduje, které vlákno/proces poběží na CPU.
- **Souběžnost a uváznutí (deadlock)** – více procesů soupeří o zdroje; deadlock = vzájemné čekání bez postupu.
- **Vznik procesu (POSIX)** – `fork()` (kopie procesu) + `exec()` (nahrazení programem); **copy-on-write** kopíruje paměť až při zápisu.

## 7. Souborové systémy
- **Blokové zařízení** – disk přistupovaný po blocích pevné velikosti.
- **Bloková vrstva / I/O plánovač** – řadí a optimalizuje požadavky na disk.
- **RAID** – spojení více disků: 0 (rychlost), 1 (zrcadlení), 5 (parita), 10 (kombinace).
- **Šifrování disku** – data na disku jsou uložena zašifrovaně.
- **Obyčejný soubor** – pojmenovaná posloupnost bajtů; popsán metadaty v **inode**.
- **Alokace volného místa** – jak se souboru přidělují bloky; sledováno bitmapou.
- **Fragmentace** – soubor rozházený po nesouvislých blocích → pomalejší čtení.
- **Adresářová struktura** – hierarchie složek; adresář mapuje jména na inody.
- **I/O mapované do paměti (mmap)** – soubor/zařízení přístupné jako oblast paměti.

## 8. Sítě
- **ISO/OSI a TCP/IP model** – vrstvené modely sítí; každá vrstva poskytuje službu vyšší a využívá nižší.
- **Adresace** – MAC (linková vrstva), IP (síťová), port (transportní).
- **Fyzická vrstva** – přenos signálu po médiu; kódování bitů do signálu.
- **Řízení přístupu k médiu** – kdo smí vysílat (CSMA/CD u Ethernetu, CSMA/CA u Wi-Fi).
- **Propojování sítí** – opakovač, switch (dle MAC), router (dle IP).
- **Přepínání a směrování** – switch přepíná v rámci sítě, router směruje mezi sítěmi dle směrovací tabulky.
- **Multicast** – doručení jednoho toku skupině příjemců najednou.
- **Zajištěný přenos** – potvrzování a opakované odeslání ztracených dat (ARQ).
- **Sestavení/ukončení spojení** – TCP three-way handshake (SYN, SYN-ACK, ACK).
- **Transportní protokoly** – **TCP** (spolehlivý, spojovaný) vs. **UDP** (rychlý, nespolehlivý, bez spojení).

## 9. Síťové aplikace a bezpečnost
- **Doručování pošty** – SMTP (odesílání), POP3/IMAP (vyzvedávání; IMAP nechává na serveru, POP3 stahuje).
- **Přenos souborů** – FTP/SFTP.
- **Web** – HTTP/HTTPS (klient–server, request–response).
- **Jmenná služba (DNS)** – překládá doménová jména na IP adresy hierarchickým stromem serverů.
- **Kvalita služby (QoS)** – řízení provozu: scheduling, prioritizace, congestion avoidance (Leaky/Token Bucket).
- **Zabezpečení komunikace** – šifrování + autentizace na různých vrstvách (TLS, IPsec).
- **Autentizace** – ověření identity (hesla, certifikáty, challenge-response).
- **Šifrování** – **symetrické** (jeden klíč, rychlé) vs. **asymetrické** (veřejný/soukromý klíč, podpisy, výměna klíče).

## 10. Základy informační bezpečnosti
- **Důvěrnost** – data vidí jen oprávnění.
- **Integrita** – data nelze nepozorovaně změnit.
- **Dostupnost** – data/služby jsou k dispozici, když je třeba.
- **Nepopiratelnost původu** – odesílatel nemůže popřít, že data poslal (digitální podpis).
- **Kryptografická primitiva** – základní stavební bloky: hash, symetrická/asymetrická šifra, podpis.
- **Kryptografický protokol** – posloupnost kroků dosahující bezpečnostního cíle (TLS, Kerberos).
- **Řízení rizik** – identifikace, hodnocení a snižování bezpečnostních rizik.
- **Audit** – kontrola a záznam událostí kvůli odhalení a doložení incidentů.
- **Hodnocení bezpečnosti / standardy** – posuzování dle norem (Common Criteria, ISO 27001).

## 11. Vývoj bezpečných aplikací
- **Řízení identity a přístupu (IAM)** – kdo je uživatel (autentizace) a co smí (autorizace, ACL/RBAC).
- **Ochrana soukromí** – minimalizace dat, pseudonymizace, anonymizace, souhlas se zpracováním.
- **Bezpečné programování** – psaní kódu odolného vůči zranitelnostem (validace vstupů, ošetření přetečení).
- **Statická analýza** – kontrola kódu **bez spuštění** (hledá vzory zranitelností).
- **Dynamická analýza** – testování za **běhu** programu (fuzzing, sanitizéry).
- **Použitelná bezpečnost** – bezpečnostní mechanismy navržené tak, aby je lidé správně používali (learnability, memorability).

## 12. Paralelní systémy
- **Dekompozice** – rozdělení problému na úlohy, které lze počítat souběžně.
- **Mapování** – přiřazení úloh procesorům/vláknům s ohledem na zátěž a komunikaci.
- **Komunikační primitiva** – způsoby výměny dat mezi procesy (send/receive, broadcast, reduce).
- **Výkonnostní analýza** – zrychlení (speedup), efektivita, Amdahlův zákon (limit dán sériovou částí).
- **Sdílená paměť** – vlákna sdílejí adresní prostor; nutná synchronizace (zámky).
- **OpenMP** – standard pro paralelizaci na sdílené paměti pomocí direktiv (`#pragma omp`).
- **POSIX Threads (pthreads)** – nízkoúrovňové API pro vlákna.
- **Lock-free** – souběžný přístup bez zámků (atomické operace) → bez deadlocku, lepší škálování.
- **Distribuovaná paměť** – procesy mají vlastní paměť, komunikují zprávami.
- **MPI (Message Passing Interface)** – standard pro komunikaci posíláním zpráv v distribuovaném prostředí.
