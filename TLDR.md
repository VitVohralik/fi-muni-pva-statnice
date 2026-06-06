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
