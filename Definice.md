# Definice – přesná znění

> Sbírka **přesných definic** ke všem otázkám. Obdržálek (a Trtík, Strejček, Safránek…) vyžadují definici **doslova a ze státnicových materiálů**, ne opisem. Znění je převzaté z `teoreticke/` a `programove/`. Učit nazpaměť hlavně tučně označené „Definice".

---

# Teoretické základy

## 1. Lineární algebra

- **Gaussova eliminace** je metoda řešení soustavy lineárních rovnic převodem matice na schodovitý tvar pomocí elementárních řádkových úprav.
- **Determinant** čtvercové matice řádu $n$ je součet všech součinů $n$ prvků matice takových, že se v žádném součinu nevyskytují dva prvky z téhož řádku ani téhož sloupce; každý součin se označí znaménkem permutace. (Pro 2×2: $ad-bc$.)
- **Inverzní matice** je matice $A^{-1}$, pro kterou $A \cdot A^{-1} = E$ (jednotková matice). Existuje jen pro regulární matice ($\det \neq 0$).
- **Vektorový podprostor** je podmnožina $\emptyset \neq U \subseteq V$, která se zúženými operacemi sama tvoří vektorový prostor.
- **Báze** je lineárně nezávislá množina vektorů z podprostoru, která ho generuje; počet vektorů báze = dimenze.
- **Vlastní vektor** je nenulový vektor $\vec{v}$, pro který $A\vec{v} = \lambda\vec{v}$; **vlastní číslo** $\lambda$ udává, jak se vektor škáluje. Geometricky: směr, který transformace nemění, jen natáhne/smrští.

## 2. Základy matematické analýzy

- **Relace** mezi množinami $A_1, \dots, A_k$ je libovolná podmnožina kartézského součinu $R \subseteq A_1 \times \cdots \times A_k$. Dělení dle arity: unární ($k{=}1$), binární ($k{=}2$), ternární ($k{=}3$), obecně $n$-ární.
- **Zobrazení** $f: X \to Y$ je binární relace, která ke každému prvku $x \in X$ přiřazuje **nejvýše jeden** prvek $y \in Y$ tak, že $[x,y] \in f$.
  - **Injektivní** (prosté) – každý prvek oboru hodnot je mapován nejvýše jedním prvkem; jen pro prosté existuje inverzní.
  - **Surjektivní** (na) – každý prvek oboru hodnot je mapován alespoň jedním prvkem.
  - **Bijektivní** – právě jedním prvkem.
- **Polynom** je funkce $P(x) = a_n x^n + a_{n-1}x^{n-1} + \cdots + a_0$, kde $a_n \neq 0$ a $a_i \in \mathbb{R}$.
- **Limita (přesná definice).** Buď $x_0, L \in \mathbb{R}^*$. Funkce $f$ má v bodě $x_0$ limitu $L$ ($\lim_{x \to x_0} f(x) = L$), pokud pro každé okolí $\mathcal{O}(L)$ existuje okolí $\mathcal{O}(x_0)$ tak, že pro všechna $x \in \mathcal{O}(x_0) \setminus \{x_0\}$ je $f(x) \in \mathcal{O}(L)$. Rozlišujeme **vlastní** (konečné číslo) a **nevlastní** (nekonečno).
- **Spojitá funkce.** $f$ je spojitá v bodě $x_0$, jestliže v něm existuje vlastní limita, existuje $f(x_0)$ a platí $\lim_{x \to x_0} f(x) = f(x_0)$.
- **Závora / supremum / infimum.** Závora je prvek větší (horní) nebo menší (dolní) než všechny prvky množiny; nemusí do ní patřit. **Supremum** = nejmenší horní závora, **infimum** = největší dolní závora.
- **Derivace (přesná definice).** Nechť $x_0 \in \mathcal{D}(f)$. Pokud existuje limita $\lim_{x \to x_0} \frac{f(x)-f(x_0)}{x-x_0}$, nazýváme ji derivací $f$ v bodě $x_0$ a značíme $f'(x_0)$. Geometricky = směrnice tečny ke grafu.
- **Diferenciál funkce** je $\mathrm{d}f(x_0) = f'(x_0)\cdot h$, tj. $\mathrm{d}y = f'(x)\,\mathrm{d}x$.
- **Určitý integrál** určuje plochu ohraničenou grafem funkce $f$ a osou $x$ na intervalu $[a,b]$.
- **Neurčitý integrál** je **množina primitivních funkcí**, lišících se v hodnotě přičítané konstanty. ⚠️ (Trtík chce přesně „množina funkcí lišících se o konstantu".)

## 3. Popisná statistika

- **Statistika** je disciplína zabývající se sběrem, prezentací, analýzou a interpretací dat.
- **Popisná statistika** kvantitativně popisuje hlavní vlastnosti statistického souboru (není to matematická disciplína).
- **Pravděpodobnostní míra (definice).** Množinová funkce $P: \mathcal{A} \to [0,1]$ je pravděpodobnostní míra na $(\Omega, \mathcal{A})$, jestliže $P(\Omega)=1$ a pro disjunktní $A_1, A_2, \dots$ platí $P(\bigcup_i A_i) = \sum_i P(A_i)$.
- **Pravděpodobnostní prostor** je trojice $(\Omega, \mathcal{A}, P)$ modelující náhodný jev.
- **Podmíněná pravděpodobnost / Bayesova věta.** Pro $P(A),P(B)>0$ platí $P(A\mid B) = \frac{P(B\mid A)\cdot P(A)}{P(B)}$. Nezávislost: $P(A\cap B)=P(A)P(B)$.
- **Náhodná veličina** je měřitelná funkce $X$ přiřazující každému elementárnímu jevu hodnotu.
- **Distribuční funkce** $F(x)=P(X \leq x)$, definovaná na celém $\mathbb{R}$, neklesající, od 0 do 1. Dvě veličiny jsou stejně rozdělené, mají-li stejné distribuční funkce.
- **Zákon velkých čísel:** průměr velkého počtu nezávislých pokusů konverguje ke střední hodnotě, $\frac{1}{n}\sum X_i \to \mu$.
- **Centrální limitní věta:** dostatečně velký výběr nezávislých vlivů stejného typu má přibližně normální rozdělení, $\frac{\sum X_i - n\mu}{\sqrt{n\sigma^2}} \to N(0,1)$.

## 4. Grafy a jejich prohledávání

- **Graf** je uspořádaná dvojice $G=(V,E)$, kde $V$ je konečná množina vrcholů a $E \subseteq \binom{V}{2}$ je množina hran (dvouprvkových podmnožin vrcholů).
- **Orientovaný graf** je uspořádaná dvojice $D=(V,E)$, kde $E \subseteq V \times V$ je množina hran (uspořádaných dvojic).
- **Věta (princip sudosti):** součet stupňů v neorientovaném grafu je sudý, roven dvojnásobku počtu hran.
- **Úplný graf:** $G$ je úplný, pokud $|E| = \binom{|V|}{2}$, tj. má $\frac{n(n-1)}{2}$ hran.
- **Podgraf** $H \subseteq G$ je graf na $V(H) \subseteq V(G)$ s libovolnou podmnožinou hran $G$ majících oba vrcholy ve $V(H)$. **Indukovaný podgraf** obsahuje **všechny** hrany $G$ mezi vrcholy z $V(H)$.
- **Izomorfismus** grafů $G$ a $H$ je bijekce $f: V(G) \to V(H)$ taková, že $u,v$ jsou spojené hranou v $G$ právě tehdy, když $f(u),f(v)$ jsou spojené v $H$.
- **Strom** je minimální souvislý acyklický graf (mezi dvěma vrcholy vede právě jedna cesta). **Les** je graf bez kružnic, jehož komponenty jsou stromy.
- **Komponenty souvislosti** jsou třídy ekvivalence relace dosažitelnosti $\sim$ na $V(G)$.
- **Silné komponenty** orientovaného grafu jsou třídy ekvivalence relace $\approx$ (vzájemná dosažitelnost); graf je **silně souvislý**, má-li nejvýše jednu silnou komponentu.
- **DFS** – průzkum do hloubky: pro každou větev se zanoří úplně do hloubky, $O(V+E)$. Využití: backtracking, silné komponenty, detekce cyklu, topologické uspořádání.
- **BFS** – průzkum do šířky: prochází po vrstvách pomocí fronty (FIFO), $O(V+E)$. Využití: nejkratší cesta v neohodnoceném grafu, Dijkstra, Prim, bipartitnost.

## 5. Grafové algoritmy

- **Vážený (ohodnocený) graf** je graf $G$ s ohodnocením hran $w: E(G) \to \mathbb{R}$.
- **Cesta** v grafu $G=(V,E)$ je posloupnost vrcholů $p=\langle v_0,\dots,v_k\rangle$ taková, že $(v_{i-1},v_i)\in E$. Existence cesty = dosažitelnost. **Jednoduchá cesta** neopakuje vrcholy.
- **Nejkratší cesta** z $v_0$ do $v_k$ je cesta $p$ taková, že pro každou cestu $\bar{p}$ z $v_0$ do $v_k$ platí $w(\bar{p}) \geq w(p)$.
- **Kostra** je podgraf $T \subseteq G$ souvislého grafu, který je stromem a $V(T)=V(G)$ (propojuje všechny vrcholy, $n-1$ hran). **Minimální kostra** má nejmenší součet vah.
- **Dijkstrův algoritmus** řeší SSSP na **nezáporně** ohodnoceném grafu pomocí prioritní fronty; vždy odebere nejbližší vrchol a relaxuje jeho hrany. Invariant: odebraný vrchol má finální vzdálenost. Složitost: $\Theta(V^2)$ pole, $\Theta((V+E)\log V)$ bin. halda, $\Theta(V\log V+E)$ Fib. halda.
- **Bellman-Fordův algoritmus** řeší SSSP i pro **záporné hrany**; $(V-1)$-krát relaxuje všechny hrany a umí detekovat záporný cyklus. Složitost $O(V\cdot E)$.
- **Kruskal:** seřadí hrany dle vah a hladově přidává ty bez cyklu (disjunktní množiny), $O(E\log E)$.
- **Prim (Jarník):** od jednoho vrcholu přidává nejlevnější hranu ven z propojené komponenty, $O(E+V\log V)$.

## 6. Stromové datové struktury

- **Binární vyhledávací strom (BVS)** je kořenový strom, kde má každý uzel nejvýše 2 potomky a platí: klíč levého potomka $<$ klíč rodiče $<$ klíč pravého potomka.
- **Vyvážený BVS** udržuje logaritmickou hloubku (listy se liší max. o 1) pomocí rotací $O(1)$ → operace $O(\log n)$ (AVL, RB).
- **Červeno-černý strom** je BVS, kde je každý uzel červený/černý, splňující: (1) kořen černý, (2) listy (NIL) černé, (3) červený uzel má černého rodiče, (4) všechny cesty z uzlu do listů mají stejný počet černých uzlů (**černá výška**). Garantuje výšku $O(\log n)$.
- **Černá výška** = počet černých uzlů na cestě z $x$ do listu (výchozí uzel se nepočítá).
- **B-strom** je $n$-ární vyvážený vyhledávací strom; uzel s $k$ klíči má $k+1$ potomků, klíče vymezují intervaly. Podle min. stupně $t$: $t-1$ až $2t-1$ klíčů. Použití: databáze (méně čtení z disku).
- **B+ strom** je modifikace B-stromu, kde jsou **všechna data v listech** (vnitřní klíče jen intervaly). Použití: souborové systémy.
- **Binární halda** je binární strom plněný zleva splňující **vlastnost haldy** (rodič $\geq$ syn u max-haldy, $\leq$ u min-haldy). Typicky v poli (potomci $2i+1, 2i+2$). Insert/delete-root $O(\log n)$, search $O(n)$.

## 7. Návrh algoritmů

- **Rekurze** je definice funkce nebo datové struktury s využitím sebe sama. Fakt: každý rekurzivní algoritmus lze převést na iterativní.
- **Matematická indukce** je technika důkazu tvrzení o nekonečných posloupnostech: báze $T(k_0)$ + indukční krok $T(k) \Rightarrow T(k+1)$.
- **Rozděl a panuj** je rekurzivní metoda řešení problému jeho rozdělením na dílčí části (divide–conquer–combine); využívá ji merge sort a quicksort.
- **Algoritmus** je teoretický princip řešení problému – konečná posloupnost elementárních výpočetních kroků.
- **Asymptotická notace:** $\mathcal{O}$ horní odhad, $\Omega$ dolní odhad, $\Theta = \mathcal{O}\cap\Omega$ těsný odhad.
- **Master theorem:** pro $T(n)=aT(n/b)+\Theta(n^c)$: $a<b^c \Rightarrow \Theta(n^c)$; $a=b^c \Rightarrow \Theta(n^c\log n)$; $a>b^c \Rightarrow \Theta(n^{\log_b a})$.
- **Merge sort** – $\Theta(n\log n)$, stabilní, není in situ. **Quicksort** – pivot dělí pole, průměr $\Theta(n\log n)$, nejhůř $\Theta(n^2)$. **Heapsort** – $\Theta(n\log n)$, in situ, nestabilní.

## 8. Funkcionální programování

- **Redukční krok** je krok, ve kterém je výraz nebo jeho část nahrazena jednodušším podvýrazem.
- **Redukční strategie** je předpis určující, který podvýraz se v následujícím kroku redukuje.
- **Striktní** (zevnitř, nejdřív argumenty), **normální** (zvenčí, nejdřív funkce), **líná** (normální + pamatuje vyhodnocené výrazy). Haskell používá normální/líné vyhodnocování.
- **Church-Rosser:** výsledek ukončeného výpočtu nezávisí na redukční strategii.
- **Perpetualita:** zacyklí-li se kterákoli strategie, zacyklí se i **striktní**. **Normalizace:** skončí-li kterákoli, skončí i **normální**.
- **Funkce vyšších řádů** jsou funkce, které berou jako argumenty jiné funkce nebo vracejí funkce jako výsledek.
- **Lambda (anonymní) funkce** nemají jméno a jsou definovány přímo v místě použití; jinak fungují jako normální funkce.
- **Typ** je množina hodnot vykazujících jisté společné vlastnosti.
- **Typová třída** zahrnuje typy s podobnými vlastnostmi; umožňuje sdílet kód ve striktně typovaných jazycích.
- **Katamorfismus** je výraz vzniklý nahrazením hodnotových konstruktorů v hodnotě algebraického typu jinými funkcemi vhodné arity.

## 9. Regulární jazyky

- **Formální jazyk** je libovolná množina slov nad určitou **abecedou** (konečnou množinou symbolů).
- **Gramatika** je množina pravidel umožňující konečně popsat potenciálně nekonečný formální jazyk; čtveřice $(NTerm, \Sigma, P, S)$.
- **Chomského hierarchie:** typ 0 (frázové – TS), typ 1 (kontextové – lineárně ohraničené TM), typ 2 (bezkontextové – zásobníkový automat), typ 3 (regulární – konečný automat).
- **Regulární jazyk** je jazyk, který akceptuje nějaké DFA, NFA, nebo je generován regulární gramatikou.
- **Regulární výraz** je matematický koncept určený pro popis regulárních jazyků (Kleeneho věta: stejná síla jako automat).
- **DFA (deterministický konečný automat)** – pětice $(Q,\Sigma,\delta,s,F)$ s totální (jednoznačnou) přechodovou funkcí $\delta: Q\times\Sigma \to Q$.
- **NFA (nedeterministický)** – stejná pětice, ale $\delta: Q\times\Sigma \to 2^Q$; slovo přijato, dovede-li alespoň jedna větev do koncového stavu.
- **Determinizace** znamená zbavení se nedeterminismu a epsilon-kroků (podmnožinová konstrukce, stav DFA = množina stavů NFA, až $2^n$ stavů – vznikají všechny podmnožiny).
- **Produktový automat** je synchronní paralelní spojení dvou automatů (stavy = $Q_1\times Q_2$).
- **Rozlišitelnost:** dva stavy $q,r$ jsou rozlišitelné slovem $w$, pokud po přečtení $w$ je právě jeden z výsledných stavů koncový. Stavy jsou **ekvivalentní**, nejsou-li rozlišitelné (slouží k minimalizaci).
- **Uzávěrové vlastnosti:** třída regulárních jazyků je uzavřená na sjednocení, průnik, rozdíl, komplement, zřetězení (a iteraci, reverzi).

## 10. Rozhodnutelnost

- **Výpočetní problém** je jakýkoliv problém, který předkládáme výpočetnímu zařízení, aby jej vyřešilo.
- **Algoritmus** je sekvence kroků/instrukcí nutná k vyřešení problému.
- **Rozhodovací problém** vrací pouze True/False – rozhoduje o nějaké vlastnosti matematického objektu. Lze ho převést na **problém příslušnosti** (patří slovo do jazyka?).
- **Turingův stroj (TS)** je obecný model výpočetního zařízení; sedmice $(Q,\Sigma,\Gamma,\delta,s,Q_{acc},Q_{rej})$. **Konfigurace** = (kontrolní stav, stav pásky, pozice).
- **Úplný TS** vždy akceptuje/zamítá – nikdy necyklí.
- **Churchova-Turingova teze / Univerzalita:** TS dokáže simulovat libovolný jiný TS; všechna zobecnění TS lze simulovat pomocí DTS.
- **Rozhodnutelnost** znamená, že existuje **úplný** TS, který akceptuje každý řetězec s vlastností $P$ a zamítá každý, který ji nemá. Formálně: existuje DTS $\mathcal{T}$ takový, že $w\in L \Rightarrow$ akceptuje, $w\notin L \Rightarrow$ zamítne, a **nikdy necyklí**.
- **Nerozhodnutelnost** znamená, že takový TS neexistuje.
- **Částečná rozhodnutelnost:** existuje TS, který požadovaná slova akceptuje, ostatní zamítá **nebo cyklí**. (Jazyk je částečně rozhodnutelný ⟺ je generován gramatikou typu 0.)
- **Halting problem** = rozhodnout, jestli TS nad daným slovem zastaví. **Věta (Turing 1936):** Halt je nerozhodnutelný.
- **Rekurzivně spočetný jazyk (RE):** $L=L(M)$ pro nějaký TM (TM ho akceptuje, typ 0).
- **Rekurzivní jazyk (Rec):** $L=L(M)$ pro nějaký **úplný** TM (TM ho rozhoduje).
- **Redukce (definice).** Funkce $f: \mathcal{D}_1 \to \mathcal{D}_2$ je redukcí $P_1$ na $P_2$, jestliže: $f$ je počítaná algoritmem, který **vždy zastaví**; pozitivní instance se převedou na pozitivní ($out_1(x)=True \Rightarrow out_2(f(x))=True$) a negativní na negativní. Píšeme $P_1 \leq P_2$.
- **Diagonalizace** je metoda pro určení (ne)rozhodnutelnosti vycházející z Cantorovy diagonální metody.

## 11. Složitost

- **Teorie výpočetní složitosti** se zabývá tím, kolik zdrojů (čas, paměť) je nutné spotřebovat na vyřešení **rozhodnutelných** problémů.
- **Složitost algoritmu** vyjadřuje náročnost algoritmu na zdroje (časová = počet kroků, prostorová = max. zabraná paměť).
- **Složitost problému** je složitost **optimálního** algoritmu řešícího tento problém.
- **Polynomiální algoritmus:** $Time_{\mathcal{A}}(n) \in \mathcal{O}(n^k)$ pro nějakou konstantu $k$. **Exponenciální:** $\mathcal{O}(2^{n^k})$.
- **Třída P** – problémy řešitelné deterministickým polynomiálním algoritmem.
- **Třída NP** – rozhodovací problém je v NP, jestliže existuje nedeterministický polynomiální algoritmus, který ho rozhoduje (ekvivalentně: pozitivní instance mají polynomiálně ověřitelný certifikát).
- **Pozitivní instance** je konkrétní případ s odpovědí „ano" (existuje řešení splňující podmínky problému).
- **Věta:** $P \subseteq NP \subseteq EXPTIME$.
- **Savitchova věta:** pro časově konstruovatelnou $f(n)$ platí $SPACE(f^2(n)) \supseteq NSPACE(f(n))$.
- **Polynomiální redukce (definice).** ⚠️ KLÍČOVÉ PRO OBDRŽÁLKA. Funkce $f: \Sigma_1^* \to \Sigma_2^*$ je polynomiální redukcí $L_1$ na $L_2$, jestliže:
  1. $f$ je počítaná deterministickým TS s **polynomiální** časovou složitostí,
  2. $w \in L_1 \Rightarrow f(w) \in L_2$,
  3. $w \notin L_1 \Rightarrow f(w) \notin L_2$.

  Píšeme $L_1 \leq_p L_2$. **Důsledek:** je-li $L_2 \in$ PTIME a $L_1 \leq_p L_2$, pak i $L_1 \in$ PTIME.
- **NP-těžký (NP-Hard):** problém, na který se **polynomiálně redukuje každý** problém třídy NP (sám nemusí být v NP).
- **NP-úplný (NP-Complete):** problém, který patří do **NP-Hard a zároveň do NP**.
- **Věta:** byl-li by nějaký NP-úplný problém řešitelný v deterministickém polynomiálním čase, platilo by $P = NP$.
- **Věta (důkaz NP-úplnosti redukcí):** je-li $L \in NP$ a existuje-li NP-úplný $L'$ s $L' \leq_p L$, pak i $L$ je NP-úplný.

---

# Programové, výpočetní a informační systémy

## 1. Podprogramy a OOP
- **Podprogram** – pojmenovaný blok kódu; **funkce** vrací hodnotu, **procedura** ne. **Čistá funkce** nemá vedlejší efekty.
- **Rozsah jmen (scope)** – prostor viditelnosti entit; **statický** (dle struktury kódu) vs. **dynamický** (dle pořadí volání).
- **Výjimka** – objekt nesoucí info o chybě, propaguje se po call-stacku k handleru (`try-catch-finally`).
- **Zapouzdření** – jazyková konstrukce spojující související data a operace pod jediným jménem + řízení přístupu.
- **Dědičnost** – nová třída přebírá členy rodičovské třídy a rozšiřuje ji.
- **Polymorfismus** – ad-hoc (přetěžování, výběr za překladu), parametrický (generika), podtypový (override, výběr za běhu).
- **LSP (Liskov):** objekt typu `T` lze bez negativních důsledků kdekoliv nahradit objektem podtypu `S`.

## 2. Nízkoúrovňové programování
- **Paměťový model programu** – segmenty: textový (instrukce), zásobník (lokální proměnné, návratové adresy), halda (dynamická paměť), inicializovaný a neinicializovaný (BSS) datový segment.
- **Ukazatel** – adresa do paměti, má typ; `&` vrací adresu, `*` dereferencuje.
- **Ukazatelová aritmetika** – posun ukazatele po prvcích podle typu (`pArray + 3` = 4. prvek).
- **Dynamická paměť (halda):** `malloc` (neinicializuje), `calloc` (n × velikost + inicializace), `realloc` (změna velikosti), `free` (uvolní). Bez `free` → memory leak.
- **struct / union / enum** – záznam pojmenovaných položek (zarovnaný) / sdílená paměť (velikost největší položky) / výčet (vnitřně int).

## 3. Nízkoúrovňové architektury
- **Polyadická (poziční) soustava** – $A = \sum a_i z^i$. Převody: 1 OCT = 3 bity, 1 HEX = 4 bity.
- **Doplňkový kód** (nejrozšířenější) – kladná čísla v přirozeném kódu, záporná negací bitů +1; jedna nula, nesymetrický rozsah, aritmetika bez korekcí.
- **Detekční kódy** – paritní bit, kontrolní součet (checksum), CRC (polynomiální dělení).
- **Opravné kódy** – zdvojení (detekce), ztrojení (oprava), Hammingův kód (paritní bity na mocninách dvojky).
- **RISC** – málo jednoduchých instrukcí pevné délky, LOAD/STORE, 1 instrukce/takt, více registrů (ARM).
- **CISC** – velký instrukční set, kompaktní kód, více adresovacích režimů (x86).
- **Mikroprogramování** – instrukce realizovány sekvencí mikroinstrukcí v mikroprogramové paměti.

## 4. Databáze
- **Relační model** – data jako $n$-ární relace, založen na predikátové logice.
- **Atribut / doména / relace** – atribut = atomická hodnota; doména = množina povolených hodnot; relace = podmnožina kartézského součinu domén (množina n-tic bez duplicit).
- **Klíče** – **superklíč** (unikátní množina atributů), **kandidátní** (minimální superklíč), **primární** (vybraný kandidátní), **cizí** (kandidátní klíč z jiné relace, tvoří vazbu).
- **Funkční závislost $X \to Y$** – dva řádky se stejným $X$ nemají různé $Y$.
- **1NF** – všechny atributy atomické (nedělitelné).
- **2NF** – 1NF + žádná **parciální** závislost (neklíčový atribut závisí na celém kandidátním klíči).
- **3NF** – 2NF + žádná **tranzitivní** závislost (neklíčové atributy vzájemně nezávislé). Formálně: pro každou závislost je triviální, $\alpha$ je superklíč, nebo $\beta-\alpha$ je v kandidátním klíči.
- **BCNF** – každá závislost je triviální nebo $\alpha$ je superklíč. Platí $\text{BCNF} \subset \text{3NF} \subset \text{2NF} \subset \text{1NF}$.
- **Dekompozice** – rozklad schématu; musí být **bezztrátová** a ideálně **zachovat funkční závislosti**.

## 5. SQL, transakce, dotazy
- **SQL** – standardizovaný neprocedurální dotazovací jazyk pro relační databáze.
- **DML / DDL / DCL** – manipulace dat (`INSERT/SELECT/UPDATE/DELETE`) / definice (`CREATE/ALTER/DROP`) / práva a transakce (`COMMIT/ROLLBACK/GRANT`).
- **Trigger** – akce provedená automaticky při události (DML/DDL/logon).
- **Integritní omezení** – `NOT NULL`, `UNIQUE`, `PRIMARY KEY`, `FOREIGN KEY`, `CHECK`, `DEFAULT`.
- **Transakce** – posloupnost operací; mezi začátkem a koncem může být DB nekonzistentní, na konci musí být konzistentní.
- **ACID** – Atomicity (celá/nic), Consistency (zachová konzistenci), Isolation (neviditelnost mezivýsledků), Durability (změny přežijí výpadek).
- **Index** – pomocná struktura zrychlující čtení (často B+ strom); nevyplatí se na malých tabulkách.
- **Vyhodnocení dotazu** – parsing → optimalizace (nejlevnější plán dle statistik) → vyhodnocení; náklady dominují diskové přístupy.

## 6. Operační systémy
- **Operační systém** – abstrakce nad hardwarem zajišťující HW přenositelnost; spravuje prostředky, izoluje procesy.
- **Jádro (kernel)** – běží v privilegovaném režimu; **monolitické** (vše v jádře, Linux), **mikrojádro** (servery mimo jádro, IPC), **hybridní** (Windows).
- **Režimy procesoru** – privilegovaný (kernel) vs. uživatelský (omezená práva).
- **Proces** – spuštěný program s vlastním virtuálním adresním prostorem (drahý na vytvoření). **Vlákno** – základní výpočetní jednotka sdílející prostředky procesu kromě zásobníku (levné).
- **Virtuální paměť** – každý proces má virtuální adresní prostor a překladovou tabulku; překlad řeší **MMU**.
- **Stránkování** – stránka = blok virtuální paměti, rámec = blok fyzické; spodních $n$ bitů (offset) se opisuje.
- **Plánování (scheduler)** – rozhoduje o spouštění vláken; preemptivní vs. kooperativní.
- **Uváznutí (deadlock)** – vlákna vzájemně čekají na zdroje. **Coffmanovy podmínky:** vzájemné vyloučení, čekající vlastník, neodnímatelnost, kruhové čekání.
- **Fork / exec / copy-on-write** – `fork` duplikuje proces, `exec` přepíše paměť novým programem; po forku jsou stránky sdílené read-only a kopírují se až při zápisu.

## 7. Souborové systémy
- **Souborový systém** – hierarchické uspořádání souborů (virtualizace úložiště).
- **Blokové zařízení** – abstrakce úložiště jako adresovatelného pole bloků (512 B–4 KB).
- **I/O plánovač** – spravuje frontu požadavků na disk a přeskládá je do optimálního pořadí.
- **RAID** – více disků jako jedno zařízení: 0 (striping/rychlost), 1 (zrcadlení), 5 (parita distribuovaná), 10 (kombinace).
- **I-node** – anonymní objekt reprezentující soubor/složku; obsahuje metadata a seznam datových bloků, **neobsahuje jméno**.
- **Adresář** – seznam namapovaných i-nodů (mapuje jména na inody).
- **Vnitřní fragmentace** – nevyužitý zbytek bloku; **vnější fragmentace** – soubory roztroušené po FS.
- **Memory-mapped I/O** – soubor namapován do virtuálního adresního prostoru, stránky se načítají lazily přes page fault.

## 8. Sítě
- **Síťový protokol** definuje formát a pořadí zpráv vyměňovaných mezi komunikujícími entitami a akce při jejich odeslání/příjmu.
- **ISO/OSI model** – 7 vrstev (L1 fyzická → L7 aplikační); TCP/IP slučuje L5–L7 a L1–L2.
- **Adresace** – MAC (L2), IP (L3), port (L4).
- **Řízení přístupu k médiu** – CSMA/CD (drátový Ethernet, detekce kolize) vs. CSMA/CA (WiFi, čeká než nikdo nevysílá).
- **Přepínání / směrování** – switch přepíná dle MAC, router směruje mezi sítěmi dle směrovací tabulky (next-hop).
- **Multicast** – zasílání skupině zájemců (IPv4 třída D).
- **ARQ** – mechanismus spolehlivosti potvrzováním (ACK): Stop-and-Wait, Go-Back-N, Selective-Repeat.
- **TCP vs. UDP** – TCP spojovaný, spolehlivý, číslovaný (handshake SYN→SYN-ACK→ACK); UDP nespojovaný, best-effort, rychlý.

## 9. Síťové aplikace a bezpečnost
- **DNS** – jmenná služba překládající doménová jména na IP; hierarchický strom (root → TLD → autoritativní server → IP).
- **SMTP / POP3 / IMAP** – odesílání pošty (SMTP); POP3 stahuje lokálně a maže ze serveru, IMAP ponechá na serveru a pamatuje stav zprávy.
- **HTTP** – přístup k datům na WWW (hypertext, request-response, TCP port 80).
- **QoS** – zajištění kvality přenosu (delay, bandwidth); DiffServ (značkování, bezstavové) vs. IntServ (rezervace, stavové). Omezování toků: Leaky Bucket vs. Token Bucket.
- **Symetrická vs. asymetrická kryptografie** – symetrická = 1 sdílený klíč (rychlá); asymetrická = veřejný + privátní klíč (pomalá, podpisy, výměna klíče).
- **Certifikát** – váže veřejný klíč na identitu; vydává certifikační autorita (CA).
- **Digitální podpis** – podepsaný hash zprávy privátním klíčem (ověření veřejným); zajišťuje integritu, nepopiratelnost, autentizaci.

## 10. Základy informační bezpečnosti
- **Bezpečnostní funkce** – **důvěrnost** (jen oprávnění vidí data), **integrita** (data nelze nepozorovaně změnit), **dostupnost** (data k dispozici), **nepopiratelnost** (původce nemůže popřít).
- **Trustworthy ≠ trusted** – spoléhání na systém (trusted) neznamená, že je objektivně bezpečný (trustworthy).
- **Kerckhoffsův princip** – bezpečnost musí záviset na utajení klíče, ne implementace.
- **Kryptografická primitiva** – symetrická/asymetrická šifra, hashování, RNG, MAC.
- **Hashování** – jednosměrný převod libovolného vstupu na pevně velký otisk; lavinový efekt, kolize nelze vyloučit.
- **MAC** – otisk zprávy se sdíleným symetrickým klíčem; ověřuje integritu i autenticitu.
- **nonce** – hodnota (např. timestamp), jejíž použití předchází replay útokům.
- **Řízení rizik** – identifikace aktiv (Asset), hrozeb (Threat) a zranitelností (Vulnerability); $R = P\cdot V\cdot C$.

## 11. Vývoj bezpečných aplikací
- **Identita** – podmnožina atributů dostačující k identifikaci v množině osob.
- **Autentizace vs. autorizace** – autentizace ověřuje identitu (heslo, biometrie, klíč); autorizace povoluje operaci dle oprávnění.
- **Modely řízení přístupu** – **RBAC** (role = skupiny oprávnění), **MAC** (centrální politiky, tagy), **DAC** (práva uděluje vlastník).
- **Koncepty soukromí** – anonymita (bez odhalení identity), pseudonymita (anonymní, ale dohledatelný), nespojitelnost, nepozorovatelnost.
- **Statická vs. dynamická analýza** – statická = z kódu bez spuštění; dynamická = za běhu (fuzzing, sanitizéry).
- **Fuzzing** – posílání kvant náhodných dat a analýza výstupů.
- **Použitelná bezpečnost** – balanc využitelnosti a zabezpečení; opatření musí být user-friendly (learnability, memorability).

## 12. Paralelní systémy
- **Paralelní systém** – systém, jehož chování vzniká interakcí souběžných procesů.
- **Dekompozice** – rozložení problému na paralelizovatelné podproblémy (úlohová, datová, průzkumová, spekulativní).
- **Mapování** – přiřazení úloh vláknům; statické (za překladu) vs. dynamické (za běhu, vyrovnává zátěž).
- **Sdílená vs. distribuovaná paměť** – sdílená = globální adresní prostor (OpenMP, pthreads); distribuovaná = oddělené paměti + zprávy (MPI).
- **Výkonnostní metriky** – zrychlení $S = T_s/T_p$, efektivita $E = S/p$, cena $C = p\cdot T_p$.
- **Amdahlův zákon** – $S_{max} = \frac{1}{(1-p)+p/S_p}$; limit zrychlení daný sekvenční částí.
- **OpenMP** – API pro paralelní C/C++, paralelizaci řeší překladač dle direktiv (`#pragma omp`).
- **MPI (Message Passing Interface)** – standard pro komunikaci posíláním zpráv v distribuovaném prostředí.
- **Lock-free** – souběžnost bez zamykání pomocí atomických operací (CAS); bez deadlocku, ale složitá korektnost.
- **CAS (Compare-And-Swap)** – atomická instrukce, která mění hodnotu jen pokud odpovídá očekávané.
