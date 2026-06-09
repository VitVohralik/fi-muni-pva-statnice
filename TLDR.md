## 1. Lineární algebra
* **Operace s vektory a maticemi:**
  * **Vektory:** Sčítání (po složkách), skalární součin (výsledkem číslo, 0 = kolmost), vektorový součin (ve 3D, výsledkem kolmý vektor).
  * **Matice:** Sčítání (stejné rozměry), násobení (řádky první $\times$ sloupce druhé, počet sloupců první = počet řádků druhé), transpozice (překlopení přes diagonálu).
* **Gaussova eliminace:** Metoda řešení soustav lineárních rovnic. Převádí matici na schodovitý tvar pomocí elementárních řádkových úprav (záměna, násobení číslem, sčítání řádků).
* **Inverzní matice:** Značí se $A^{-1}$, platí $A \cdot A^{-1} = E$ (jednotková matice). Existuje jen pro regulární čtvercové matice ($\det \neq 0$). Získá se eliminací: $(A|E) \to (E|A^{-1})$.
* **Determinant:** Skalární hodnota čtvercové matice. Geometricky udává orientovaný objem rovnoběžnostěnu. Je-li roven nule, matice je singulární (nemá jednoznačné řešení ani inverzi).
* **Vlastnosti lineárních operací a skalárního součinu:**
  * **Lineární operace** zachovávají aditivitu $L(\vec{x}+\vec{y}) = L(\vec{x})+L(\vec{y})$ a homogenitu $L(\alpha\vec{x}) = \alpha L(\vec{x})$.
  * **Skalární součin** je symetrický ($\vec{u}\cdot\vec{v} = \vec{v}\cdot\vec{u}$) a umožňuje počítat délky a odchylky.
* **Vektorové podprostory:** Podmnožina vektorového prostoru, která je sama o sobě vektorovým prostorem (je uzavřená na lineární kombinace vektorů – sčítání a násobení skalárem).
* **Vektorové báze:** Množina lineárně nezávislých vektorů, které generují celý prostor (každý vektor prostoru lze složit z jejich kombinace). Počet vektorů báze tvoří **dimenzi** prostoru.
* **Lineární transformace:** Zobrazení zachovávající základní operace s vektory. Reprezentují např. otočení, zvětšení/zmenšení, zkosení nebo projekci.
* **Matice zobrazení:** Matice reprezentující lineární transformaci. Získáme ji tak, že zobrazovanou operaci aplikujeme na vektory standardní báze a výsledky zapíšeme jako sloupce této matice.
* **Vlastní čísla a vektory a jejich geometrický význam:**
  * **Vlastní vektor ($\vec{v}$):** Vektor, u kterého se transformací nemění jeho směr, pouze velikost nebo orientace.
  * **Vlastní číslo ($\lambda$):** Skalár (koeficient) udávající, jak moc se vlastní vektor natáhl, smrštil nebo otočil do protisměru ($A\cdot\vec{v} = \lambda\cdot\vec{v}$).
  * **Geometrický význam:** Jsou to směry (osy transformace), ve kterých transformace funguje pouze jako škálování.

## 2. Základy matematické analýzy
* **Relace:** Libovolná podmnožina kartézského součinu množin. Podle počtu množin je unární, binární, ternární, obecně $n$-ární.
* **Zobrazení:** Binární relace přiřazující každému prvku nejvýše jeden prvek. **Injektivní** (prosté – nejvýše jeden vzor), **surjektivní** (na – alespoň jeden vzor), **bijektivní** (právě jeden vzor).
* **Funkce:** Zobrazení mezi číselnými množinami. **Totální** (definovaná všude), **parciální** (ne nutně všude), **inverzní** (existuje jen pro injektivní), **konstantní**.
* **Vlastnosti reálných funkcí:** Definiční obor a obor hodnot, sudost ($f(x)=f(-x)$) / lichost ($-f(x)=f(-x)$), periodicita ($f(x+p)=f(x)$), omezenost shora/zdola.
* **1. derivace:** Určuje monotonii – $f'>0$ rostoucí, $f'<0$ klesající. Stacionární body ($f'=0$) a lokální extrémy.
* **2. derivace:** Určuje prohnutí – $f''>0$ konvexní, $f''<0$ konkávní. Inflexní body, kde se mění prohnutí ($f''=0$, $f'''\neq 0$).
* **Asymptota:** Přímka, k níž se křivka funkce s rostoucí hodnotou blíží.
* **Polynom:** Výraz $P(x)=a_n x^n + \dots + a_0$ (sčítání, odčítání, násobení). Kořen je $x$, pro které $P(x)=0$. **Hornerovo schéma** hledá celočíselné kořeny a rozklad na kořenové činitele.
* **Limita:** Hodnota, k níž se funkce blíží v daném bodě. **Vlastní** (konečné číslo), **nevlastní** (nekonečno). Existuje, právě když si jsou rovny obě jednostranné limity.
* **Spojitá funkce:** Funkce, jejíž funkční hodnota se v bodě rovná vlastní limitě: $\lim_{x\to x_0} f(x) = f(x_0)$.
* **Body nespojitosti:** **Odstranitelná** (limity zleva i zprava stejné, ale $\neq f(a)$), **skok** (1. druhu – různé vlastní limity), **2. druhu** (alespoň jedna limita nevlastní).
* **Závora, supremum, infimum:** Závora je prvek větší (horní) / menší (dolní) než všechny prvky množiny, nemusí do ní patřit. Supremum = nejmenší horní závora, infimum = největší dolní závora.
* **Derivace:** Směrnice tečny ke grafu funkce; limita podílu změny funkce ku změně argumentu. Udává okamžitou změnu (růst/pokles) funkce.
* **Pravidla derivací:** Linearita, součin ($(fg)'=f'g+fg'$), podíl, složená funkce (řetízkové pravidlo $f'(x)=h'(g(x))\cdot g'(x)$).
* **l'Hospitalovo pravidlo:** Úprava neurčitých výrazů ($\frac{0}{0}$, $\frac{\infty}{\infty}$) pomocí limity podílu derivací.
* **Taylorův polynom:** Polynomiální aproximace funkce v okolí bodu pomocí jejích derivací; od $x_0=0$ se nazývá Maclaurinova řada.
* **Diferenciál funkce:** Přírůstek funkční hodnoty na tečně: $\mathrm{d}y = f'(x)\,\mathrm{d}x$.
* **Určitý integrál:** Orientovaná plocha pod grafem funkce na intervalu $[a,b]$: $\int_a^b f(x)\,\mathrm{d}x$.
* **Neurčitý integrál:** Množina primitivních funkcí (opak derivace), liší se o konstantu, bez mezí.
* **Integrační metody:** **Per partes** (integrace součinu) a **substituční metoda** (zavedení nové proměnné).

## 3. Popisná statistika
* **Kombinatorika:** **Variace** (uspořádaná $k$-tice), **kombinace** (neuspořádaná $k$-tice), **permutace** (uspořádaná $n$-tice) – s opakováním i bez.
* **Statistika:** Disciplína sběru, analýzy a interpretace dat. **Popisná statistika** kvantitativně popisuje statistický soubor (množina statistických jednotek se statistickými znaky).
* **Statistické znaky:** **Kvantitativní** (diskrétní/spojité), **kvalitativní** (ordinální/nominální), **alternativní**. Podle měřítka: nominální, ordinální, intervalové, poměrové.
* **Aritmetický průměr:** Podíl součtu hodnot a jejich počtu; ovlivnitelný rozptylem. **Vážený průměr** přiřazuje každé hodnotě váhu.
* **Medián:** Prostřední hodnota (50. percentil), neovlivněný extrémy. **Modus** je nejčastější hodnota.
* **Střední hodnota (E):** Vážený průměr rozdělení (vahou je pravděpodobnost). Průměr z dat, střední hodnota z pravděpodobností.
* **Rozptyl (D):** Střední hodnota kvadrátů odchylek od střední hodnoty: $\sigma^2(X)=E(X^2)-[E(X)]^2$. **Směrodatná odchylka** je jeho odmocnina.
* **Kvantily:** Dělí uspořádaná data na části – kvartily (Q1 25 %, Q2 medián, Q3 75 %), percentily.
* **Kovariance a korelace:** Kovariance udává směr lineární závislosti, korelace její sílu (koeficient $\in\langle-1,1\rangle$). **Kovarianční matice** má na diagonále rozptyly.
* **Pravděpodobnost:** Míra očekávání jevu, $P:\mathcal{A}\to[0,1]$, $P(\Omega)=1$. Liší se od šance (příznivé ku všem vs. příznivé ku nepříznivým).
* **Pravděpodobnostní prostor:** Trojice $(\Omega,\mathcal{A},P)$ – elementární jevy, jevové pole, pravděpodobnostní míra.
* **Operace s jevy a nezávislost:** Sjednocení, průnik, opačný jev. Nezávislost: $P(A\cap B)=P(A)P(B)$. **Podmíněná pravděpodobnost** $P(A\mid B)=\frac{P(A\cap B)}{P(B)}$.
* **Věty:** **Bayesova** (vztah opačných podmíněných pravděpodobností), **ZVČ** (průměr konverguje ke střední hodnotě), **CLV** (velký výběr má přibližně normální rozdělení).
* **Náhodná veličina:** Měřitelná funkce $X:\Omega\to\mathbb{R}$. **Distribuční funkce** $F(x)=P(X\leq x)$. Diskrétní (skoky) vs. spojitá (hustota).
* **Diskrétní rozdělení:** Geometrické, negativně binomické, hypergeometrické, Poissonovo, alternativní (Bernoulli), binomické, rovnoměrné.
* **Spojitá rozdělení:** Normální ($\mu, \sigma^2$), exponenciální ($\lambda$), gamma ($\alpha, \beta$).
* **Statistický odhad:** **Bodový** (1 číslo, např. průměr) a **intervalový** (konfidenční interval). **MLE** = metoda maximální věrohodnosti.
* **Konfidenční interval:** $100(1-\alpha)\%$; neznámý parametr v něm leží s pravděpodobností $1-\alpha$; $\alpha$ je hladina významnosti.
* **Regresní analýza:** Vztah mezi proměnnými. **Lineární model** $y=\beta_0+\beta_1 x+\epsilon$; hodnocení přes $R^2$, P-hodnotu, deviance.
* **Testování hypotéz:** $H_0$ (vztah neexistuje) vs. $H_1$. **Chyba 1. druhu** (falešné zamítnutí $H_0$), **2. druhu** (nezamítnutí nepravdivé $H_0$). Testy: t.test, wilcox.test.

## 4. Grafy a jejich prohledávání
* **Graf:** Uspořádaná dvojice $G=(V,E)$ – množina vrcholů $V$ a hran $E$ (dvouprvkové podmnožiny vrcholů).
* **Stupeň vrcholu:** Počet vycházejících hran $d_G(v)$. **Věta:** součet stupňů = dvojnásobek počtu hran. **$d$-regulární** graf = všechny vrcholy stejný stupeň.
* **Orientovaný vs. neorientovaný graf:** Orientovaný má jednosměrné hrany (šipky, $E\subseteq V\times V$), neorientovaný obousměrné. **Transpozice** obrací směr hran, **symetrizace** zapomíná směr.
* **Typy grafů:** Kružnice, cesta, **úplný** ($\frac{n(n-1)}{2}$ hran), **bipartitní** (vrcholy do 2 disjunktních množin, bez liché kružnice), úplný bipartitní.
* **Podgraf:** Graf na podmnožině vrcholů s podmnožinou hran. **Indukovaný podgraf** obsahuje všechny hrany původního grafu mezi vybranými vrcholy.
* **Izomorfismus:** Bijektivní zobrazení vrcholů zachovávající hrany. Izomorfní grafy mají stejné počty vrcholů, hran i stupně.
* **Eulerovský graf:** Souvislý graf se všemi vrcholy sudého stupně – jde nakreslit jedním tahem.
* **Strom:** Minimální souvislý acyklický graf; mezi dvěma vrcholy vede právě jedna cesta. **Les** = graf bez kružnic (komponenty jsou stromy), hran = vrcholy − stromy.
* **Kořenový strom:** Má kořen (hloubka 0), hierarchii potomků, listy. **Výška** = počet hran ke nejvzdálenějšímu listu. **Úplný** $n$-ární strom = všechny listy ve stejné hloubce.
* **Komponenta souvislosti:** Maximální podmnožina vrcholů, mezi nimiž vede cesta. **Silná** (s orientací) vs. **slabá** (bez orientace) souvislost.
* **Kosaraju–Sharir:** Hledá silně souvislé komponenty v $O(V+E)$ – DFS, reverse postorder, transpozice grafu, opakované DFS.
* **Reprezentace grafu:** **Matice sousednosti** ($\Theta(V^2)$, husté grafy, test hrany $O(1)$) vs. **seznam následníků** ($\Theta(V+E)$, řídké grafy).
* **Typy hran při průchodu:** Stromová, zpětná (cyklus/smyčka), dopředná, příčná. Vrcholy se obarvují bílý/šedý/černý (discovery a finish time).
* **Topologické uspořádání:** Sekvence vrcholů, kde $u$ je před $v$ pro každou hranu $(u,v)$. Opačné pořadí dokončení DFS.
* **DFS (do hloubky):** Zanoří se úplně do každé větve, $O(V+E)$, rekurze/zásobník. Využití: backtracking, silné komponenty, detekce cyklu, topologické uspořádání.
* **BFS (do šířky):** Prochází po vrstvách pomocí fronty (FIFO), $O(V+E)$. Využití: nejkratší cesta v neohodnoceném grafu, Dijkstra, Prim, ověření bipartitity.

## 5. Grafové algoritmy
* **Ohodnocený (vážený) graf:** Každá hrana má přiřazenou váhu $w:E(G)\to\mathbb{R}$. Lze reprezentovat **maticí vah** $W$.
* **Cesta:** Posloupnost vrcholů spojených hranami; existence = dosažitelnost. **Jednoduchá cesta** neopakuje vrcholy, **Hamiltonovská** projde všechny vrcholy.
* **Délka cesty:** Počet hran (u ohodnocených součet vah). Neexistuje → $\infty$, obsahuje záporný cyklus → $-\infty$.
* **Nejkratší cesta:** Cesta s minimální vahou. Existuje vždy i jednoduchá; **každá podcesta nejkratší cesty je nejkratší**.
* **SSSP (Single Source Shortest Path):** Nejkratší cesty z jednoho vrcholu do všech. Neohodnocený → BFS, acyklický → relaxace v topologickém uspořádání.
* **Relaxace hrany:** Aktualizace odhadu vzdálenosti vrcholu, pokud se přes hranu našla kratší cesta. Základ Dijkstry i Bellman-Forda.
* **Dijkstrův algoritmus:** Nejrychlejší SSSP přes **prioritní frontu**, jen **nezáporné** hrany. Složitost dle fronty: pole $\Theta(V^2)$, binární halda $\Theta((V+E)\log V)$, Fibonacciho $\Theta(V\log V+E)$.
* **Bellman-Fordův algoritmus:** SSSP i pro **záporné hrany**, umí **detekovat záporný cyklus**. $(V-1)\times$ relaxuje všechny hrany, složitost $O(V\cdot E)$.
* **Minimální kostra (MST):** Podgraf-strom propojující všechny vrcholy ($n-1$ hran) s nejmenším součtem vah. Využití: stavba sítí.
* **Kruskalův algoritmus:** Hladově řadí hrany dle vah a přidává ty bez cyklu (disjunktní množiny, union-find), $O(E\log E)$.
* **Jarníkův (Primův) algoritmus:** Od jednoho vrcholu přidává nejlevnější hranu ven z komponenty, $O(E+V\log V)$.

## 6. Stromové datové struktury
* **Binární vyhledávací strom (BVS):** Kořenový strom s max. 2 potomky, kde levý potomek $<$ rodič $<$ pravý potomek. Operace v nevyváženém stromu $O(n)$.
* **Následník / předchůdce:** Uzel s nejmenším větším / největším menším klíčem než $x$. Používají se při mazání uzlu se 2 potomky.
* **Průchody:** **preorder** (kořen, L, P), **inorder** (L, kořen, P — vypíše seřazeně), **postorder** (L, P, kořen).
* **Mazání v BVS:** Bez potomka → smazat; 1 potomek → nahradí ho potomek; 2 potomci → nahradí následník/předchůdce.
* **Vyvážený BVS:** Listy mají přibližně stejnou hloubku $\Rightarrow$ hloubka $\log_2(n+1)$ a operace $O(\log n)$. Vyvažuje se **rotacemi** $O(1)$. Příklady: AVL, RB stromy.
* **AVL strom:** Samovyvažující se implementace BVS.
* **Červeno-černý strom (RB):** Samovyvažující BVS s uzly červený/černý. Garantuje výšku $2\log_2(n+1)$. Pravidla: kořen černý, listy (NIL) černé, červený má černého rodiče, stejná **černá výška** všech cest do listů.
* **Černá výška:** Počet černých uzlů na cestě z $x$ do listu (bez výchozího uzlu).
* **Rotace:** `LeftRotate` / `RightRotate` — vzájemně inverzní, zachovávají uspořádání BVS, mění strukturu v $O(1)$.
* **RB korekce po vložení:** Nový uzel je červený; podle barvy strýce buď **přebarvení** (strýc červený) nebo **rotace** (strýc černý) ve třech případech.
* **B-strom:** $n$-ární vyvážený vyhledávací strom; uzel s $k$ klíči má $k+1$ potomků, klíče vymezují intervaly. Min. stupeň $t$: uzel má $t-1$ až $2t-1$ klíčů, hloubka $\log_t\!\frac{n+1}{2}$. Použití: databáze (méně čtení z disku).
* **Štěpení / merge uzlu:** Plný uzel se rozdělí, prostřední klíč vystoupá do rodiče (dělení kořene zvyšuje výšku). Při podtečení se uzly slučují. Preemptivní štěpení rozděluje skoro plné uzly už při průchodu.
* **B+ strom:** Modifikace B-stromu — **všechna data v listech**, vnitřní klíče jen pro intervaly. Listy propojené odkazem na následující list (rychlé čtení sekvenčních dat). Použití: souborové systémy.
* **Binární halda (heap):** Binární strom plněný zleva splňující **vlastnost haldy** (max-halda: rodič $\geq$ syn; min-halda: rodič $\leq$ syn). Typicky v poli (potomci $2i+1$, $2i+2$, rodič $\lfloor(i-1)/2\rfloor$).
* **Operace haldy:** Insert i Delete-Root $O(\log n)$ (probublávání), Search $O(n)$, stavba haldy $O(n)$. **Heapify** opravuje vlastnost haldy probubláváním dolů.
* **Heapsort:** Opakované odebírání kořene max-haldy. $O(n\log n)$, **in situ**, **není stabilní**. Halda implementuje **prioritní frontu**.
* **Hashovací tabulka:** Klíče přiděluje deterministická **hashovací funkce**. Kolize: **zřetězení** (uzavřená adresace, linked list pod klíčem) nebo **otevřená adresace** (sondování — lineární, kvadratické). Smazání značí hodnotou **Deleted**.

## 7. Návrh algoritmů
* **Rekurze:** Definice funkce/struktury s využitím sebe sama; iteruje až k **zarážce** (triviální případ). Drží volání na zásobníku.
* **Druhy rekurze:** **Přímá** (A volá A), **nepřímá** (A→B→A), **tail-rekurze** (volání na konci, nahraditelné cyklem — kompilátor optimalizuje).
* **Výhody/nevýhody rekurze:** Čitelný zápis vs. paměťová náročnost (**stack overflow**), těžší odhad složitosti, často pomalejší. Každou rekurzi lze převést na iterativní (explicitní zásobník/cyklus).
* **Matematická indukce:** Důkaz tvrzení o nekonečných posloupnostech — **báze** $T(k_0)$ + **indukční krok** $T(k)\Rightarrow T(k+1)$. Jde opačným směrem než rekurze (indukce začíná bází, rekurze k ní směřuje).
* **Rozděl a panuj:** Rekurzivní dělení na triviální podproblémy: **Divide → Conquer → Combine**. Výhody: lepší asymptotika, paralelismus, práce v cache. Používá merge sort a quicksort.
* **Algoritmus:** Konečná posloupnost elementárních kroků; má vstupní podmínku, **invariant cyklu** (platí před i po iteraci) a výstupní podmínku.
* **Korektnost:** **Konvergence/úplnost** (výpočet skončí), **parciální korektnost** (skončí-li, je výsledek správný), **totální korektnost** = obojí.
* **In situ:** Algoritmus s konstantní extra pamětí (modifikuje vstup). **Extrasekvenční** složitost neuvažuje vstupní data.
* **Asymptotická notace:** $\mathcal{O}$ (horní odhad, „nejvýše tak rychle"), $\Omega$ (dolní odhad), $\Theta = \mathcal{O}\cap\Omega$ (stejně rychle).
* **Substituční metoda:** Odhad řešení + důkaz indukcí ($T(n)\le cn\log n$).
* **Rekurzivní strom:** Rozbalení rekurze — sčítání práce po úrovních (geometrická řada).
* **Master theorem:** Pro $T(n)=aT(n/b)+\Theta(n^c)$: $a<b^c\Rightarrow\Theta(n^c)$; $a=b^c\Rightarrow\Theta(n^c\log n)$; $a>b^c\Rightarrow\Theta(n^{\log_b a})$.
* **Řadicí algoritmy:** **Stabilní** nemění pořadí stejných prvků; **přirozený** rychleji zpracuje částečně seřazená data.
* **Insertion / Selection sort:** Oba $\Theta(n^2)$, in situ. Insertion **vkládá** do seřazené části (stabilní), selection **vybírá** min/max (nestabilní).
* **Merge sort:** Rozděl a panuj, $\Theta(n\log n)$, **stabilní**, **není in situ**, asymptoticky optimální.
* **Heapsort:** $\Theta(n\log n)$, **in situ**, **není stabilní**, asymptoticky optimální (řazení haldou).
* **Quicksort:** Pivot dělí pole na menší/větší, rekurze na obě části. Průměrně $\Theta(n\log n)$, nejhůř $\Theta(n^2)$; vhodný v praxi.
* **Nekomparativní řazení ($O(n)$):** **Counting sort** (počítá výskyty), **radix sort** (po číslicích od nejméně signifikantní), **bucket sort** (přihrádky dle rozsahu, lze paralelizovat).

## 8. Funkcionální programování
* **Funkcionální paradigma:** Deklarativní paradigma; program je výraz, výpočet = jeho zjednodušování. Důraz na čisté funkce, imutabilitu a funkce vyšších řádů.
* **Redukce:** Postupné nahrazování výrazu jednodušším podvýrazem; jeden takový krok je **redukční krok**.
* **Redukční strategie:** Předpis, který podvýraz redukovat dál. **Striktní** (zevnitř, nejdřív argumenty — Java, Python), **normální** (zvenčí, nejdřív funkce — Haskell), **líná** (normální + pamatuje si vyhodnocené výrazy, zvládá nekonečná data).
* **Churchova–Rosserova věta:** Skončí-li výpočet, je výsledek vždy stejný nezávisle na strategii (délka výpočtu i zacyklení se lišit mohou).
* **Perpetualita / Normalizace:** Zacyklí-li se kterákoli strategie, zacyklí se i **striktní** (nejméně bezpečná). Skončí-li kterákoli, skončí i **normální** (nejbezpečnější).
* **Arita:** Počet parametrů funkce — nulární (konstanta), unární, binární, ternární.
* **Čistá funkce:** Bez vedlejších efektů; v Haskellu jsou ale i nečisté (I/O). Vše je **immutable**.
* **Funkce vyšších řádů:** Berou funkci jako argument nebo ji vracejí (`map`, `filter`, `fold`). Umožňují abstrakci a znovupoužití kódu.
* **Lambda (anonymní) funkce:** Funkce bez jména definovaná v místě použití: `\x -> x*x`.
* **Currying a částečná aplikace:** Funkce je řetězec unárních funkcí; aplikací na část argumentů vznikne nová funkce. `curry`/`uncurry` převádí mezi více parametry a n-ticí; `flip` prohodí pořadí parametrů.
* **Haskell:** Čistě funkcionální, silně a staticky typovaný, líné vyhodnocování. Kompilátor GHC/GHCi, start funkcí `main`.
* **Typy:** **Monomorfní** (`Int`, `Integer`, `Float`, `Char`, `String`=`[Char]`, `Bool`), **polymorfní** (typová proměnná `a`), **kvalifikovaný** (polymorfní s omezením typovou třídou).
* **Typové třídy:** Sdružují typy s podobnými vlastnostmi (`Eq`, `Ord`, `Num`, `Integral`, `Show`). Umožňují sdílení kódu.
* **Uživatelské typy:** Definice přes `data` (hodnotové konstruktory), např. `data Maybe a = Nothing | Just a`. **Pattern matching** rozkládá hodnoty podle vzoru.
* **Seznamy:** Immutable, líné, konstrukce přes `(:)`, spojování `(++)`, `zip`, `concat`. Lze definovat nekonečné (`[1..]`, `cycle`, `iterate`).
* **Intenzionální seznamy:** Definice pravidlem s generátorem: `[2*n | n <- [0..9]]`.
* **Fold / katamorfismus:** Akumulace seznamu do jedné hodnoty (`foldl` zleva, `foldr` zprava). Katamorfismus = nahrazení hodnotových konstruktorů jinými funkcemi vhodné arity.

## 9. Regulární jazyky
* **Formální jazyk:** Libovolná množina slov nad **abecedou $\Sigma$** (konečná množina symbolů). **Slovo** je konečná posloupnost symbolů, **$\varepsilon$** je prázdné slovo.
* **Operace nad jazyky:** Sjednocení, průnik, rozdíl, zřetězení ($L_1.L_2$), iterace ($L^*$, $L^+$), doplněk ($\Sigma^* \setminus L$), reverze (palindrom $ww^R$).
* **Pumping lemma (lemma o vkládání):** Každé dostatečně dlouhé slovo z dané třídy lze rozdělit a „napumpovat" zopakováním části → opět slovo z jazyka. Slouží k důkazu, že jazyk **není** regulární.
* **DFA (deterministický konečný automat):** Pětice $(Q, \Sigma, \delta, s, F)$ s **totální injektivní** přechodovou funkcí $Q \times \Sigma \to Q$. Pamatuje si jen současný stav.
* **NFA (nedeterministický):** Stejná pětice, ale $\delta: Q \times \Sigma \to 2^Q$ (potenční množina). Slovo je platné, dovede-li alespoň jednu větev do koncového stavu. **$\varepsilon$-NFA** povoluje epsilon-kroky (přechod bez čtení znaku).
* **Síla NFA = síla DFA:** Oba akceptují pouze regulární jazyky; NFA převedeme na DFA **determinizací**.
* **Determinizace:** Odstranění $\varepsilon$-kroků (Next1/2/3 – epsilon okolí) + **podmnožinová konstrukce** (stav DFA = množina stavů NFA).
* **Produktový automat:** Synchronní paralelní spojení 2 DFA (sdílí abecedu), stavy = kartézský součin $Q_1 \times Q_2$. Průnik: $F = F_1 \times F_2$; sjednocení: $F = (F_1 \times Q_2) \cup (Q_1 \times F_2)$.
* **Uzávěrové vlastnosti:** Regulární jazyky jsou uzavřené na sjednocení, průnik, rozdíl, zřetězení, iteraci, reverzi a doplněk.
* **Doplněk automatu:** Prohození koncových a nekoncových stavů – nutná **totální** přechodová funkce.
* **Minimalizace:** Slučování **ekvivalentních** (nerozlišitelných) stavů. Hledáme stavy **rozlišitelné** slovem délky $\leq$ počet stavů; odstraníme nedosažitelné, iterujeme třídy rozkladu. Pro každý regulární jazyk existuje jedinečný minimální DFA.
* **Kanonizace:** Přečíslování stavů v pořadí průchodu (do šířky) → jedinečný kanonický DFA. Umožňuje test ekvivalence dvou automatů.
* **Gramatika:** Čtveřice $(NTerm, \Sigma, P, S)$ – neterminály, terminály, přepisovací pravidla, počáteční neterminál. Větší vyjadřovací síla než automaty (popis syntaxe jazyků).
* **Chomského hierarchie:** Vnořené třídy: **typ 0** frázové (Turingův stroj), **typ 1** kontextové ($\alpha A\beta \to \alpha\gamma\beta$, lineárně ohraničené TM), **typ 2** bezkontextové ($A \to \gamma$, zásobníkové automaty), **typ 3** regulární ($A \to a$ / $A \to aB$, konečné automaty).
* **Regulární výraz:** Popis regulárního jazyka pomocí závorek, sjednocení, zřetězení a iterace. **Kleeneho věta:** stejná vyjadřovací síla jako automat.
* **Převody:** Gramatika ↔ NFA ↔ DFA ↔ regulární výraz (odstranění stavů a nahrazení šipek regulárními výrazy).

## 10. Rozhodnutelnost
* **Výpočetní problém:** Problém předkládaný výpočetnímu zařízení; reprezentace dvojicí $(\mathcal{D}, out)$ – doména instancí a funkce přiřazující výstup. **Algoritmický problém** vyžaduje specifický algoritmus (konečný, s jasnými vstupy/výstupy).
* **Rozhodovací problém:** Vrací True/False o vlastnosti objektu. Každý lze přeložit na **problém příslušnosti** (patří slovo do jazyka?).
* **Turingův stroj (TS):** Konečný automat s nekonečnou páskou. Sedmice $(Q, \Sigma, \Gamma, \delta, s, Q_{acc}, Q_{rej})$; $\Gamma = \Sigma$ + zarážka $\triangleright$ + prázdné políčko $\sqcup$. **Konfigurace** = (stav, páska, pozice).
* **Úplný TS:** Vždy akceptuje/zamítá, nikdy necyklí. Pokud TS cyklí nebo se zasekne, slovo je zamítnuto.
* **Churchova–Turingova teze:** Každé reálné výpočetní zařízení simuluje nějaký TS (nelze dokázat). **Univerzalita:** TS umí simulovat libovolný jiný TS (lze ho zapsat jako řetězec a poslat na vstup).
* **Rozhodnutelnost:** Existuje **úplný** TS akceptující slova s vlastností $P$ a zamítající ostatní. **Nerozhodnutelnost:** takový TS neexistuje. **Částečná rozhodnutelnost:** TS požadovaná slova akceptuje, ostatní zamítá nebo cyklí.
* **Halting problem:** Rozhodnout, zda TS nad slovem zastaví. **Nerozhodnutelný** (Turing 1936), ale částečně rozhodnutelný (instance, které zastaví).
* **Třídy jazyků:** **Rekurzivně spočetný (RE)** = akceptován nějakým TM (typ 0); **rekurzivní (Rec)** = rozhodován **úplným** TM. Každý rekurzivní je i rekurzivně spočetný; regulární jazyky jsou rozhodnutelné.
* **Nedeterministický TS (NTS):** $\delta: Q \times \Gamma \to 2^{Q \times \Gamma \times \{+1,-1,0\}}$; v pseudokódu `Oracle()`. Akceptuje, pokud alespoň jeden výpočet vrátí True. Lze simulovat DTS.
* **Metoda redukce:** Transformační algoritmus převádějící problém $P_1$ na $P_2$ ($P_1 \leq P_2$). Nerozhodnutelnost $P_1$ ⟹ nerozhodnutelnost $P_2$; rozhodnutelnost $P_2$ ⟹ rozhodnutelnost $P_1$.
* **Nerozhodnutelné problémy:** Postův problém přiřazení (PCP), CFG-EQUIVALENCE, CFG-REGULARITY (pro bezkontextové gramatiky).
* **Diagonalizace:** Cantorova metoda – anti-diagonální stroj dělá opak diagonály matice (TS × vstupy). Dokazuje nerozhodnutelnost halting problému i problému příslušnosti pro TM.

## 11. Složitost
* **Teorie výpočetní složitosti:** Zkoumá, kolik výpočetních zdrojů (čas, paměť) stojí řešení **rozhodnutelných** problémů; výpočetní model = Turingův stroj, délka výpočtu = počet kroků.
* **Složitost algoritmu:** Náročnost konkrétního algoritmu na zdroje. **Časová** = délka nejdelšího výpočtu pro daný vstup; **prostorová** = největší zabraná paměť. Měří se v nejhorším/průměrném/nejlepším případě.
* **Složitost problému:** Složitost **optimálního** (nejrychlejšího/nejúspornějšího) algoritmu řešícího problém, bere se nejhorší vstup.
* **Asymptotická notace:** $\mathcal{O}(g)$ roste nejvýše tak rychle, $\Omega(g)$ alespoň tak rychle, $\Theta(g) = \mathcal{O} \cap \Omega$ stejně rychle jako $g$. Polynomiální $\mathcal{O}(n^k)$, exponenciální $\mathcal{O}(k^n)$.
* **Polynomiální = efektivní:** Polynomiální algoritmy ($Time \in \mathcal{O}(n^k)$) jsou považovány za prakticky řešitelné.
* **P (PTIME):** Problémy řešitelné **deterministickým** polynomiálním algoritmem (DTS). Např. NSD, prvočíselnost, řazení, minimální kostry, SSSP.
* **NP:** Problémy řešitelné **nedeterministickým** polynomiálním algoritmem; ekvivalentně mají **polynomiálně verifikovatelný certifikát** pozitivní instance. P ⊆ NP ⊆ EXPTIME.
* **P vs. NP:** Otevřený problém – lze-li výsledek rychle ověřit, lze ho také rychle nalézt? Neví se ani $NP = EXPTIME$.
* **Pozitivní instance + certifikát:** Instance s odpovědí „ano"; certifikát je důkaz pozitivnosti ověřitelný v polynomiálním čase (např. ověření součtu u SUBSET-SUM).
* **EXP / PSPACE / EXPSPACE:** Exponenciální čas, resp. polynomiální / exponenciální prostor (paměť).
* **Savitchova věta:** $SPACE(f^2) \supseteq NSPACE(f)$ – nedeterministický prostor $N$ lze simulovat deterministicky v $N^2$.
* **Polynomiální redukce ($\leq_p$):** Převod problému $L_1$ na $L_2$ funkcí počítanou v PTIME, zachovávající (ne)pozitivnost. Pokud $L_2 \in$ PTIME a $L_1 \leq_p L_2$, pak i $L_1 \in$ PTIME.
* **NP-Hard (těžké):** Na problém se polynomiálně redukuje **každý** problém z NP; sám nemusí být v NP.
* **NP-Complete (úplné):** NP-Hard ∩ NP. Každý úplný je těžký, ne naopak. P řešení jednoho úplného ⟹ $P = NP$ (kolaps celé NP do P).
* **Důkaz NP-úplnosti:** Je-li $L \in$ NP a $L' \leq_p L$ pro nějaký NP-úplný $L'$, pak je i $L$ NP-úplný (redukce z kanonického problému).
* **Kanonické NP-úplné problémy:** 3SAT, problém obchodního cestujícího (rozhodovací varianta), problém batohu, VERTEX-COVER, CLIQUE.
* **TQBF (True Quantified Boolean Formula):** Rozhodnout pravdivost plně kvantifikované výrokové formule ($\forall$/$\exists$ u každé proměnné). Kanonický **PSPACE-úplný** problém (obdoba SATu pro NP), zobecnění SATu.
* **Příklady tříd:** P – NSD, prvočíselnost; NP – faktorizace, izomorfismus grafů, SUBSET-SUM; PSPACE – TQBF; EXP – šachy; nerozhodnutelné – Halt, CFG-Equality.

---

# Programové, výpočetní a informační systémy

## 1. Podprogramy a OOP
* **Programovací paradigmata:** **Procedurální/imperativní** (strukturované, nestrukturované, OOP – záleží na pořadí instrukcí) vs. **deklarativní** (funkcionální, logické – co se má udělat, ne jak).
* **Dělení jazyků:** Dle abstrakce (nízko-/vysokoúrovňové), dle kompilace (**kompilované** – binárka se statickými dependencies, vs. **interpretované** – interpretace/JIT/mezikód za běhu).
* **Datové typy:** **Jednoduché** (ordinální – int, bool, char, enum; neordinální – float/double dle IEEE 754, void) a **složené** (pole, string, list, struct, union, tagged union, tuple).
* **Ukazatel:** Adresa do paměti / null. **Dangling pointer** míří na dealokovanou paměť; **odkaz** je ukazatel, který se sám dereferencuje a nepoužívá aritmetiku.
* **ADT:** Implementačně nezávislá specifikace struktury dat s povolenými operacemi (zásobník, fronta, množina). Schovává detaily okolnímu světu.
* **Typování:** **Silně/slabě** (zda zamezuje nesprávné operace) × **staticky/dynamicky** (kontrola při překladu/za běhu). Java, Haskell, C# = silně staticky; Python = silně dynamicky; C/C++ = slabě staticky; JS/PHP = slabě dynamicky.
* **Ekvivalence typů:** **Jmenná** (porovnává jména, striktní vs. volná vůči aliasům) vs. **strukturální** (nahrazuje jména definicemi). **Type cast** (implicitní/explicitní konverze), **koerce** (stačí kompatibilita).
* **Proměnná:** Pojmenovaná oblast v paměti s hodnotou. **Vazba** statická/dynamická, **aliasing** (více jmen na týž objekt), **mutable** (mění hodnotu, drží identitu) vs. **immutable**.
* **Řízení toku:** **Příkazy** provádějí akci (přiřazení, podmínky, cykly, blok); **výrazy** se vyhodnotí na hodnotu. **Operátor** = funkce se speciální notací (pre-/in-/postfix, unární/binární/ternární).
* **Priorita a asociativita:** Priorita určuje pořadí operátorů (neviditelné závorky), asociativita řeší stejnou prioritu (zleva/zprava). **Líné vyhodnocování** rozhodne bez vyhodnocení celého výrazu.
* **Rozsah (scope):** Prostor viditelnosti entit. **Statický** (dle struktury kódu, určen při překladu) vs. **dynamický** (dle pořadí volání, za běhu). Globální rozsah = globální proměnné.
* **Podprogram:** Základní mechanismus řízení běhu. **Funkce** vrací hodnotu (volá se ve výrazu), **procedura** ji nevrací (volá se jako příkaz). **Čistá funkce** nemá vedlejší efekty.
* **Předávání parametrů:** **Hodnotou** (kopie), **odkazem/sdílením** (efektivní, riziko aliasů), **jménem** (líné vyhodnocení výrazu), **výsledkem** (`out`), **hodnotou-výsledkem** (`in-out`).
* **OOP:** Paradigma s objekty (data + metody), které komunikují. 4 principy: **abstrakce, zapouzdření, dědičnost, polymorfismus**. Stavební kameny – třída (typ i implementace) a rozhraní (bez implementace).
* **Abstrakce:** Skrývání nedůležitých detailů, high-level pohled (rozhraní, abstraktní třídy s deklarovanými metodami – nelze instanciovat).
* **Zapouzdření:** Spojení dat a operací pod jediným jménem, řízení přístupu (`public`/`protected`/`private`/package). **Boxing** = obalení hodnotového typu objektem. **Namespace** = prostor jmen.
* **Dědičnost:** Nová třída využívá rodičovskou (tranzitivně, stromová hierarchie). Dědí se min. `protected` členy; konstruktor potomka volá konstruktor rodiče. **Diamond problem** u vícenásobné dědičnosti tříd.
* **LSP:** Objekt typu T lze nahradit objektem podtřídy S bez negativních důsledků. Alternativa k dědičnosti = **kompozice**.
* **Polymorfismus:** **Ad-hoc** (přetěžování, výběr za překladu), **parametrický** (generika, dynamická vazba v runtime), **podtypový** (T drží objekt podtřídy). **Override** přepisuje metodu rodiče (výběr za běhu).
* **Časná vs. pozdní vazba:** **Časná (statická)** – metoda vybrána za překladu dle deklarovaného typu, v C# klíčové slovo `new` (skrytí). **Pozdní (dynamická)** – vybrána za běhu dle skutečného typu objektu, v C# `virtual` + `override` (přepsání). Časná je rychlejší.
* **Tabulka virtuálních metod (vtable):** Každý objekt nese ukazatel na tabulku své třídy s odkazy na implementace virtuálních metod (code pointers). Umožňuje pozdní vazbu; u `override` se odkaz přesměruje, jinak zděděn z rodiče.
* **Výjimky:** Objekt nesoucí info o chybě, propaguje se nahoru po call-stacku k handleru (`try-catch-finally`). **Kontrolované** (musí se chytit / `throws`) vs. **nekontrolované** (`RuntimeException`).
* **Event-driven programming:** Asynchronní paradigma, tok řízen událostmi ve frontě dispatcheru, obsluhují je posluchače (EventListener) mimo hlavní vlákno (aplikace nezamrzá).
* **SOLID:** Single-responsibility, Open–closed, Liskov substitution, Interface segregation, Dependency inversion – principy návrhu udržovatelných OOP systémů.

## 2. Principy nízkoúrovňového programování
* **Paměť:** Adresovatelné množství slotů fixní délky (slot typicky 1 bajt). Entity zabírají více slotů, přístup přes adresu začátku (hexadecimálně, např. `0x0a`).
* **Paměťové segmenty programu:** **Textový** (instrukce), **zásobník** (stack-frame s lokálními proměnnými), **halda** (dynamická paměť), **inicializovaný** a **neinicializovaný (bss)** datový segment (globální proměnné).
* **C jako slabě typovaný jazyk:** Objekty mohou měnit typy. **Implicitní** konverze (interpretuje bity jiným typem) vs. **explicitní** (převede hodnotu vnitřní funkcí). `sizeof()` vrací počet bajtů typu.
* **Zarovnání (alignment):** Typy zarovnané na násobky slova procesoru kvůli optimalizaci čtení (`int` 4 B bez paddingu, `char` 1 B + 3 B padding).
* **Bitové operátory:** `&` (AND), `|` (OR), `^` (XOR), `~` (INVERT), `<<`/`>>` (shift = násobení/dělení 2). Reprezentace dat jako flagů, čtení maskou.
* **`const`:** Označuje konstantu, překladač hlídá neměnnost. Lze ošálit přiřazením do nekonstantního ukazatele.
* **Plytká vs. hluboká kopie:** Plytká = přiřazení (povrch struktury), hluboká = `malloc()` + `memcpy()`. Předání struktury hodnotou tvoří plytkou kopii.
* **Uživatelské typy:** **`enum`** (výčet, vnitřně `int`), **`struct`** (záznam pojmenovaných položek, zarovnaný), **`union`** (sdílená paměť, velikost největší položky, bitová reinterpretace), **`typedef`** (nový název typu).
* **Ukazatel:** Adresa do paměti, má typ. `&` vrací adresu, `*` dereferencuje. **Ukazatelová aritmetika** posouvá po prvcích (`pArray + 3` = 4. prvek). `Pole` ≡ `&Pole[0]`, ale `int*` ≠ `int[10]`.
* **NULL / void\* / funkční ukazatel:** NULL = adresa 0 (`(void*)0`). `void*` bez znalosti typu. Funkční ukazatel míří na kód funkce (předávání funkce parametrem).
* **Aliasing:** Více ukazatelů různého typu na stejné místo. **Strict aliasing** to zakazuje kvůli optimalizacím (lze vypnout).
* **Pole:** Souvislý blok, alokace za překladu, **meze se nehlídají** (segfault při přístupu mimo). Vícerozměrné pole překladač ukládá jednorozměrně. Řetězec = pole charů s koncovou `\0`.
* **Dynamická paměť (halda):** `malloc` (neinicializuje), `calloc` (n × velikost + inicializuje), `realloc` (změna velikosti, zachová obsah), `free` (uvolní, nemaže obsah), `memset` (rychlá inicializace). Bez `free` → memory leak; double free = undefined behaviour (CWE-415).
* **Ladění:** **Debugger** krokuje program, zkoumá proměnné/zásobník/haldu. **Breakpoint** (i conditional), **memory breakpoint** (změna paměti, nutná podpora CPU), **Valgrind** (memory leaky, analýza paměti). HW podpora: trap flag, instrukce pro virtualizaci.

## 3. Nízkoúrovňové výpočetní architektury
* **Číselné soustavy:** **Polyadické** (poziční, $A=\sum a_i z^i$) vs. **nepolyadické** (římské). Převody: 1 OCT = 3 bity, 1 HEX = 4 bity BIN.
* **Přirozený kód:** Přímý binární obraz čísla, nejlevější bit je znaménko. Rozsah $(-127,127)$, dvě nuly, složitější aritmetika.
* **Inverzní kód:** Záporná čísla mají invertované bity. Při přetečení / kladném výsledku nutno přičíst +1. Dvě nuly.
* **Doplňkový kód:** Nejrozšířenější. Kladná v přirozeném, záporná negací bitů +1. Jedna nula, nesymetrický rozsah $(-128,127)$, bez korekce.
* **Aditivní kód:** Posunutá nula (obraz nuly `0111…1`). Nesymetrický rozsah, výhoda = přímé porovnávání kladných i záporných.
* **Váhový / BCD kód:** Řádům přiřazeny váhy (BCD = 8-4-2-1, 4 bity = 1 desítková číslice). **Packed** (4 bity/číslice) vs. **unpacked** (1 bajt/číslice). Bez zaokrouhlovacích chyb, ale plýtvá místem.
* **IEEE 754:** Plovoucí desetinná čárka $F=m\cdot Z^{exp}$. Znaménko (1 b) + exponent (aditivní, 8 b) + mantisa (přímý, 23 b).
* **Vnitřní / vnější kódy:** Vnitřní = uvnitř systému (BCD, doplňkový, ASCII). Vnější = ordinální hodnota znaku (Unicode, UTF-8).
* **Detekční kódy:** Redundance pro odhalení chyb – **paritní bit**, **kontrolní součet (checksum)**, **CRC** (polynomiální dělení).
* **Opravné kódy:** Redundance pro opravu – **zdvojení** (detekce), **ztrojení** (oprava), **Hammingův kód** (paritní bity na mocninách dvojky).
* **Booleova algebra:** Šestice $(A,\wedge,\vee,\neg,1,0)$ nad $\{0,1\}$. Pravidla: komutativita, distributivita, De Morgan, absorpce, idempotence…
* **Hradla:** Skládají se z tranzistorů (NOT, AND, OR, NAND, NOR, XOR), nemají paměť.
* **Paměti:** Druhy vnější/vnitřní/permanentní/registry. **RWM/RAM** (volatilní), **registry** (na čipu, nejrychlejší), **ROM/EPROM/EEPROM** (permanentní), **CAM** (asociativní, adresace tagem).
* **Endianita:** **Little-Endian** (nejnižší bajt na nejmenší adrese), **Big-Endian** (nejvyšší bajt na nejmenší adrese), Middle-Endian.
* **Cache:** SRAM, asociativní, oddělená pro instrukce/data. **L1** (per jádro), **L2** (per jádro/skupina), **L3** (sdílená). Algoritmy **LRU**, **LFU**. Vyrovnávací paměť (zápis) vs. mezipaměť (čtení, prefetch).
* **Procesor:** Synchronní stroj řízený řadičem, dvojkový doplňkový kód. Dělí se dle velikosti slova, struktury (RISC/CISC/DSP), počtu jader. Takt = operace/s.
* **Registry:** Úložiště velikosti 1 slovo, monolitické, neindexovatelné. **A** (střádač/akumulátor), **PC** (čítač instrukcí, adresa vykonávané instrukce).
* **Instrukční set:** LDA, STA, JMP, MOV, aritmetické/logické, podmíněné skoky dle flagů (JC/JZ/JP…), zásobník (PUSH/POP).
* **Zásobník volání (callstack):** Stack-frame = lokály + návratová adresa + parametry. Stack Pointer (vrchol) a Frame Pointer (rámec).
* **Přerušení:** Pozastavení práce mezi instrukcemi, v privilegovaném režimu, flag IF. Lze nořit. Obsluha podprogramem + RET. 256 typů v tabulce. Souběh řešen spinlockem + zákazem přerušení.
* **Typy přerušení:** **Vnější** (HW, ze zařízení přes řadič přerušení), **vnitřní** (procesor – dělení nulou, výpadek stránky), **softwarové** (synchronní instrukce – systémové volání). **Offload** (zařízení s vlastní jednotkou, např. síťovka).
* **Mikroprogramování:** Instrukce realizovány sekvencí **mikroinstrukcí** uložených v mikroprogramové paměti. Chyby v mikrokódu → zranitelnosti (Meltdown).
* **Von Neumannova architektura:** 5 modulů – vstupní zařízení, ALU, řadič, operační paměť, výstupní zařízení. Dnešní odlišnosti: multitasking, více procesorů, DMA, částečné zavádění programu.
* **RISC:** Málo jednoduchých instrukcí pevné délky, LOAD/STORE, 1 instrukce/takt, více registrů, složitost v kompilátoru. Více kódu, rychlejší běh (ARM).
* **CISC:** Velký instrukční set, kompaktní kód, více adresovacích režimů, méně RAM, nižší výkon (Intel x86).

## 4. Databáze
* **Data:** Údaje s vypovídací schopností. **Redundance** = opakovaný výskyt informace, **inkonzistence** = porušení pravidel (např. duplicitní „unikátní" ID).
* **Databázový model:** Logická struktura ukládání dat – **relační**, **síťový**, **hierarchický**.
* **Relační model:** Model založený na predikátové logice; data = $n$-ární relace. Využívají ho relační databáze.
* **Atribut / doména / relace:** Atribut = atomická hodnota (plní sloupec), doména = množina povolených hodnot (`null` je vždy v ní), relace = podmnožina kartézského součinu domén (množina $n$-tic bez duplicit). Soubor relací = **relační schéma**.
* **Klíče:** **Superklíč** (dostatečně unikátní množina atributů), **kandidátní klíč** (minimální superklíč), **primární klíč** (vybraný kandidátní), **cizí klíč** (kandidátní klíč z jiné relace – tvoří vazbu).
* **Relační algebra:** Procedurální dotazovací jazyk, operace uzavřené nad relacemi (vstup i výstup je relace). 6 základních operací.
* **Selekce $\sigma$:** Vybírá **řádky** splňující podmínku $P(t)$.
* **Projekce $\Pi$:** Vybírá **sloupce**, umí i aritmetiku nad sloupci.
* **Sjednocení $\cup$ / rozdíl $-$:** Vyžadují stejnou **aritu** (počet sloupců) a domény. Sjednocení spojí, rozdíl odebere $n$-tice z druhé relace.
* **Kartézský součin $\times$:** Všechny kombinace řádků; při společných atributech nutné **přejmenování**.
* **Přejmenování $\rho$:** Přejmenuje atributy (výsledky agregací, konflikty u součinu).
* **Agregační funkce $G$:** `avg`, `min`, `max`, `sum`, `count`. `count` vrací 0 pro `null`, ostatní `null`.
* **Join:** **Natural join $\bowtie$** spojí přes společné atributy (selekce + projekce nad $\times$). **Outer join** doplní `null` – left/right/full dle připojené strany.
* **Funkční závislost ($X \rightarrow Y$):** Dva řádky se stejným $X$ nemají různé $Y$. **Triviální** ($Y \subseteq X$, platí vždy), **úplná** (potřeba celé $X$), **částečná** (opak úplné – stačí část $X$), **tranzitivní** (přes prostředníka $\gamma$). Slouží k dekompozici a prevenci redundance.
* **Armstrongovy axiomy:** Pravidla pro odvození uzávěru závislostí – reflexivita, tranzitivita, pseudotranzitivita, sjednocení, dekompozice, rozšíření, zúžení.
* **1NF:** Všechny domény (atributy) jsou **atomické** (nedělitelné).
* **2NF:** 1NF + každý neklíčový atribut závisí na **celém** kandidátním klíči (žádná **parciální** závislost).
* **3NF:** 2NF + neklíčové atributy vzájemně nezávislé (žádná **tranzitivní** závislost). Pro každou závislost: triviální, $\alpha$ je superklíč, nebo $\beta-\alpha$ je v kandidátním klíči.
* **BCNF:** 3NF + každá závislost je triviální nebo $\alpha$ je superklíč. Silnější než 3NF, ale nemusí zachovat funkční závislosti. Platí $\text{BCNF} \subset \text{3NF} \subset \text{2NF} \subset \text{1NF}$.
* **Dekompozice:** Rozklad schématu na menší; musí být **bezztrátová** (zachová data) a ideálně **zachovat funkční závislosti** ($\bigcup F_i^+ = F^+$).
* **Normalizace:** Dekompozice do normálních forem kvůli lepší manipulaci, méně redundanci a konzistenci. **Nezlepšuje výkon.**

## 5. SQL, transakce, dotazy
* **SQL:** Standardizovaný **neprocedurální** dotazovací jazyk pro relační databáze (IBM, standardy ANSI). Nerozlišuje velikost písmen.
* **Jazykové prvky:** **Příkaz** (statement), **dotaz** (query – vrací relaci), **klauzule** (clause), **predikát** (podmínka v 3VL: pravda/nepravda/neznámé), **výraz** (skalární hodnota).
* **Skupiny příkazů:** **DML** (manipulace dat – `INSERT/SELECT/UPDATE/DELETE`), **DDL** (definice – `CREATE/ALTER/DROP`), **DCL** (práva a transakce – `COMMIT/ROLLBACK/GRANT/REVOKE`).
* **Operátory:** `= <> < >`, `BETWEEN` (inkluzivní), `LIKE` (vzor), `IN`, `IS [NOT] NULL`, `IS NOT DISTINCT FROM`, `AS` (alias).
* **Datové typy:** `char(n)`, `varchar(n)`, `int`, `real`, `float(n)`, `date/time/timestamp`, `numeric(p,d)`, uživatelské (`CREATE TYPE`).
* **SELECT:** Odpovídá projekci. `SELECT` (povinné) – `FROM` (kartézský součin, povinné) – `WHERE` (selekce, nepovinné). `DISTINCT` bez duplicit, `ALL` s duplicitami.
* **INSERT / UPDATE / DELETE:** Vkládá/upravuje/maže záznamy z **právě jedné** tabulky; musí splňovat omezení sloupců. Pozor na vnořené dotazy v `WHERE`.
* **MERGE:** Kombinace `INSERT` a `UPDATE` (`WHEN MATCHED` / `WHEN NOT MATCHED`).
* **GROUP BY:** Roztřídí záznamy podle parametru, umožní agregační funkce. `WHERE` se provede **před** seskupením.
* **JOIN:** Spojuje tabulky. Typy: **inner**, **left/right/full outer**. Podmínky: `NATURAL`, `ON`, `USING` (bez nich kartézský součin).
* **HAVING:** Podmínka nad agregačními funkcemi, provede se **po** `WHERE`. Atributy mimo agregace musí být v `GROUP BY`.
* **Agregační funkce:** `COUNT` (jediná vrací 0 pro `NULL`, `COUNT(sloupec)` ignoruje `NULL`, `DISTINCT` pro unikáty), `AVG`, `SUM`, `MIN`, `MAX`. Implicitně berou celou tabulku jako jednu skupinu.
* **Vnořené SQL:** `IN/NOT IN`, `<op> SOME` (alespoň jedna), `<op> ALL` (všechny), `EXISTS/NOT EXISTS` (neprázdná/prázdná). Místo atributu musí vracet jednu hodnotu.
* **Trigger (spouštěč):** Akce provedená automaticky při události. **DML** (INSERT/UPDATE…), **DDL** (CREATE/DROP/ALTER), **logon** trigger. Často pro kontrolu integrity.
* **Uložená procedura:** Program uložený v DB (PL/SQL, T-SQL). Výhody: výkon (prováděcí plán v cache), nepřerušitelnost, vrstva zabezpečení, propojení procedur.
* **Integritní omezení:** `NOT NULL`, `UNIQUE`, `PRIMARY KEY` (NOT NULL + UNIQUE), `FOREIGN KEY`, `CHECK`, `DEFAULT`, `INDEX`. **Referenční integrita** cizím klíčem mezi podřízenou a nadřízenou tabulkou.
* **Transakce:** Posloupnost operací nad daty; mezi začátkem a koncem může být DB nekonzistentní, na konci musí být konzistentní.
* **ACID:** **Atomicity** (celá/nic), **Consistency** (zachová konzistenci), **Isolation** (neviditelnost mezivýsledků pro ostatní), **Durability** (změny přežijí výpadek).
* **Úrovně izolace:** Read uncommitted → Read committed → Repeatable read → Serializable. Postupně eliminují **dirty read**, **non-repeatable read**, **fantom**.
* **Fantom:** Nově vložený/smazaný řádek objevující se uprostřed transakce, ač logicky měl být zamčen. Může nastat i při striktním 2PL.
* **Stavy transakce:** Aktivní → částečně potvrzená → potvrzená; nebo aktivní/částečně potvrzená → chybující → zrušená.
* **Souběžné zpracování:** Vyšší propustnost a nižší odezva, ale nutné **zamykání** a řešení **deadlocku** (vzájemné čekání na zdroje – řeší se ukončením transakce).
* **Plán:** Pořadí instrukcí souběžných transakcí. **Serializovatelný** = ekvivalentní sériovému plánu.
* **Vyhodnocení dotazu:** 1) parsing + překlad do relační algebry, 2) **optimalizace** (nejlevnější plán dle statistik v katalogu), 3) **vyhodnocení** strojem.
* **Míra nákladů:** Dominují diskové přístupy (seek + čtení/zápis bloků). Více paměti snižuje čtení z disku. Zápis dražší než čtení.
* **Operace výběru:** **A1 lineární** ($E = b_r$, příp. $b_r/2$ na klíči), **A2 binární** ($E = \lceil\log_2 b_r\rceil + \lceil SC/f_r\rceil - 1$, jen na seřazeném klíči).
* **Index:** Zrychluje čtení, zpomaluje zápis. Záznam `|klíč|ukazatel|`. **Řazené** vs **hašovací** indexy.
* **Řazené indexy:** **Primární/shlukující** (určuje pořadí záznamů, řídký i hustý), **sekundární/neshlukující** (jiné pořadí, jen hustý). **Hustý** (záznam pro každou hodnotu klíče) vs **řídký** (jen některé).
* **Víceúrovňový index:** Řídký index nad primárním indexem (vnější) – když se index nevejde do paměti.
* **B⁺ strom:** Vyvážený $n$-ární strom, nejpoužívanější index. Stejná délka cest, vnitřní uzel $\lceil n/2\rceil$–$n$ potomků, list $\lceil(n-1)/2\rceil$–$n{-}1$ klíčů. Automatická lokální reorganizace.
* **Statické hašování:** **Kyblík** (bucket) z hašovací funkce $h: K \to B$. **Otevřené** (closed addressing, přetokové kyblíky) vs **uzavřené** (open addressing, `i++` při kolizi). Špatné pro **ranged queries**.
* **Dynamické hašování:** Mění hašovací funkci dle velikosti DB. **Rozšiřitelné hašování** – prefix $i$ bitů adresuje kyblík, tabulka adres se zdvojnásobuje/slévá.
