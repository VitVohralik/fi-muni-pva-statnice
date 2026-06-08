# Teorie výpočetní složitosti

> **Teorie výpočetní složitosti** se zabývá efektivitou výpočtů, tj. tím, kolik výpočetních zdrojů je nutné spotřebovat na vyřešení **rozhodnutelných** problémů.

- **Výpočetní model** je nejčastěji **Turingův stroj**.
- **Délka výpočtu** je počet kroků výpočetního modelu (redukční kroky, atomické operace, …) pro korektní algoritmus a korektní vstup.

# Složitost algoritmu versus složitost problému

## Složitost algoritmu

> **Složitost algoritmu** vyjadřuje náročnost algoritmu na výpočetní zdroje (čas, paměť, počet procesorů, …).

Podle požadovaných zdrojů rozlišujeme různé míry složitosti $\Rightarrow$ v **nejhorším**, **průměrném** nebo **nejlepším** případě.

- **Časová složitost algoritmu** je funkce, která pro každou velikost vstupu vrací délku **nejdelšího** výpočtu na všech možných datech této velikosti.
- **Prostorová složitost algoritmu** je funkce, která pro každou velikost vstupních dat je rovna velikosti paměti výpočtu zabírajícího **největší paměť** na všech možných datech této velikosti.

> **Definice (prostorová složitost):** Mějme algoritmus $\mathcal{A}$. Prostorová složitost algoritmu $\mathcal{A}$ je funkce $Space_{\mathcal{A}} : \mathbb{N} \to \mathbb{N}$ taková, že pro libovolné $n \in \mathbb{N}$ klademe
> $$Space_{\mathcal{A}}(n) = \max\{cells_{\mathcal{A}}(x) \mid |x| = n\}.$$

## Složitost problému

> **Složitost problému** je složitost **optimálního** algoritmu řešícího tento problém.

- **Časová složitost problému** je časová složitost algoritmu, který řeší daný problém (i na nejpomalejších datech) **nejrychleji**. Bere se v úvahu nejhorší případ (vstup).
- **Prostorová složitost problému** je prostorová složitost algoritmu, který řeší daný problém (i na nejméně příznivých datech) na **nejmenším** prostoru paměti. Bere se v úvahu nejhorší případ (vstup).

Prostorová složitost problému je tedy dána složitostí „prostorově nejefektivnějšího" (vzhledem k asymptotické notaci) algoritmu, který tento problém rozhoduje. Problémy se pak kategorizují do **prostorových složitostních tříd**.

> Prostorovou složitost lze zkoumat pomocí TS se **dvěma páskami** – read-only vstupem a pracovní read-write páskou.

# Asymptotická notace

Pro porovnávání složitosti problému se využívá **asymptotická $O$-notace** (worst-case). Pro každou funkci $g : \mathbb{N} \to \mathbb{R}_0^+$ zavedeme následující množiny funkcí:

- $\mathcal{O}(g) = \{ f \mid \exists c > 0, n_0 \in \mathbb{N} : \forall n \geq n_0 : f(n) \leq c \cdot g(n) \}$
  Množina funkcí rostoucích „**nejvýše tak rychle**" jako $g$.
- $\Omega(g) = \{ f \mid \exists c > 0, n_0 \in \mathbb{N} : \forall n \geq n_0 : c \cdot g(n) \leq f(n) \}$
  Množina funkcí rostoucích „**alespoň tak rychle**" jako $g$.
- $\Theta(g) = \{ f \mid \exists c_1 > 0, c_2 > 0, n_0 \in \mathbb{N} : \forall n \geq n_0 : c_1 \cdot g(n) \leq f(n) \leq c_2 \cdot g(n) \} = \mathcal{O}(g) \cap \Omega(g)$
  Množina funkcí rostoucích „**stejně rychle**" jako $g$.

Díky tomu můžeme dělit algoritmy do **složitostních tříd**: lineární, kvadratická atd.

| Notace | Typ složitosti |
|--------|----------------|
| $\mathcal{O}(n^k)$ | polynomiální |
| $\mathcal{O}(k^n)$ | exponenciální |

> **Definice (polynomiální algoritmus):** Algoritmus $\mathcal{A}$ má **nejvýše polynomiální** časovou složitost (zkráceně $\mathcal{A}$ je **polynomiální**), pokud existuje konstanta $k \in \mathbb{N}$ taková, že $Time_{\mathcal{A}}(n) \in \mathcal{O}(n^k)$.

> **Definice (exponenciální algoritmus):** Algoritmus $\mathcal{A}$ má **nejvýše exponenciální** časovou složitost, pokud existuje konstanta $k \in \mathbb{N}$ taková, že $Time_{\mathcal{A}}(n) \in \mathcal{O}(2^{n^k})$.

**Polynomiální algoritmy** jsou považovány za **efektivní** (v teorii i v praxi).

# Složitostní třídy

Dělení do tříd podle nejhoršího případu **časové** složitosti:

- **P** (PTIME / Polynomial Time) zahrnuje problémy, které jsou polynomiálně řešitelné nějakým **deterministickým** polynomiálním algoritmem (na DTS).
	- Např. SSSP, minimální kostry, řazení, rozhodnutí prvočíselnosti.
	- Faktorizace v kryptografii spoléhá na to, že její řešení **nespadá** do třídy P.
- **EXP** (Exponential Time) zahrnuje problémy, které jsou exponenciálně řešitelné nějakým deterministickým exponenciálním algoritmem.
- **NP** (Nondeterministic Polynomial Time) zahrnuje problémy řešitelné **nedeterministickým** polynomiálním algoritmem.
	- Zda problémy NP spadají také do P (tj. zda $P = NP$), je dosud **nevyřešené**.
	- Stejně tak se neví, zda $NP = EXPTIME$.

Dělení podle **prostorové** složitosti:

- **PSPACE** zahrnuje problémy, které lze vyřešit pomocí **polynomiálního** prostoru (paměti).
- **EXPSPACE** zahrnuje problémy, které lze vyřešit pomocí **exponenciálního** prostoru.

## Třída NP

> **Definice:** Rozhodovací problém je řešitelný v **nedeterministickém polynomiálním čase**, jestliže existuje nějaký nedeterministický polynomiální algoritmus, který tento problém rozhoduje. Třída všech takových problémů se značí **NPTIME**, nebo též jen **NP**.

**NP třídy** náleží **nedeterministickým** Turingovým strojům. Jejich záběr je přirozeně širší, protože NTS potřebuje méně kroků než DTS, díky možnosti vykonávat více větví „naráz" – resp. **prozřetelnému výběru** správné větve.

- **P je vlastně jen specifickým případem NP.**
- Každý výsledek NP algoritmu lze **verifikovat v P čase**.

> **Pozitivní instance** problému je konkrétní případ, který má odpověď „ano". Tzn. pro tuto instanci existuje řešení, které splňuje všechny podmínky/kritéria definované problémem.

K pozitivním instancím NP problémů existují tzv. **polynomiálně verifikovatelné certifikáty**. Jsou to důkazy, že dané instance jsou pozitivní, a korektnost tohoto důkazu je ověřitelná v polynomiálním čase.

> **Příklad:** sečtení prvků u SUBSET-SUM lze provést s lineární složitostí. Nalezení té správné podmnožiny už je ale obtížnější.

> **P vs. NP** $\Rightarrow$ *Pokud lze rychle ověřit správnost výsledku, lze tento výsledek také rychle nalézt?*

**Důkazem**, že problém patří do složitostní třídy, je zkonstruování příslušného stroje, který daný problém řeší. Např. DTS pro třídu P, NTS pro třídu NP, …

### Příklad: obsahuje pole číslo 7?

Uvažme problém: rozhodnout, zda dané vstupní pole $P$ délky $n$ obsahuje číslo 7.

**Deterministický** algoritmus složitosti $\mathcal{O}(n)$:

```
i ← 1;
while i ≤ n do
    if P[i] == 7 then return True;
    else i ← i + 1;
return False
```

**Nedeterministický** algoritmus složitosti $\mathcal{O}(1)$:

```
i ← Oracle({1, …, n});
if P[i] == 7 then return True;
else return False;
```

## Vztahy mezi třídami

> **Věta:** Platí $P \subseteq NP \subseteq EXPTIME$.

**Idea:** první inkluze plyne přímo z definice (P je speciální případ NP). Druhá plyne z toho, že každý NTS lze simulovat deterministickým strojem, který má max. exponenciálně horší složitost.

## Savitchova věta

> **Savitchova věta:** Pro každou časově konstruovatelnou funkci $f(n)$ platí
> $$SPACE(f^2(n)) \supseteq NSPACE(f(n)).$$

Nedeterministický stroj s prostorovou složitostí $N$ lze simulovat deterministickým strojem s prostorovou složitostí $N^2$.

- Představme si, že NTS počítá všechny větve backtrackingu „naráz", zatímco DTS postupně.

# Polynomiální redukce

**Redukce** (viz [[10-Rozhodnutelnost|otázka 10]]) sama o sobě **nelze** použít k porovnání složitosti, protože **zanedbává počet spotřebovaných výpočetních zdrojů**.

> Zápis $A \leq B$ čteme jako „$A$ se redukuje na $B$".

> **Polynomiální redukce** umožňuje převod jednoho rozhodovacího problému na jiný takovým způsobem, že pokud máme polynomiální algoritmus pro řešení druhého problému, můžeme jím řešit i první problém.

Aby šlo o polynomiální redukci, musí převod mezi problémy spadat do **PTIME**.

> **Definice:** Mějme dva jazyky (problémy) $L_1 \subseteq \Sigma_1^*$ a $L_2 \subseteq \Sigma_2^*$. Řekneme, že funkce $f : \Sigma_1^* \to \Sigma_2^*$ je **polynomiální redukcí** problému $L_1$ na problém $L_2$, jestliže platí:
> - $f$ je počítaná nějakým deterministickým Turingovým strojem s **polynomiální** časovou složitostí,
> - pro libovolné $w \in \Sigma_1^*$, pro které platí $w \in L_1$, platí i $f(w) \in L_2$,
> - pro libovolné $w \in \Sigma_1^*$, pro které platí $w \notin L_1$, platí i $f(w) \notin L_2$.
>
> Řekneme, že problém $L_1$ se **polynomiálně redukuje** na problém $L_2$, píšeme $L_1 \leq_p L_2$, jestliže existuje redukce problému $L_1$ na problém $L_2$.

> **Důsledek:** Pokud $L_2$ patří do PTIME a $L_1 \leq_p L_2$, pak $L_1$ patří také do **PTIME**.

# Těžkost a úplnost problému

## NP-Hard (těžké problémy)

> **Těžké (NP-Hard)** problémy jsou takové, že se na ně **polynomiálně redukuje každý** problém třídy NP.

- Samotný těžký problém ale **nemusí** být součástí třídy NP.

## NP-Complete (úplné problémy)

> **Úplné (NP-Complete)** problémy patří do **NP-Hard** a zároveň do **NP**.

- Platí tedy, že každý **úplný** problém je **těžký**, ale ne každý těžký je úplný.
- Na NP-úplné problémy se polynomiálně redukují **všechny** problémy z NP.
- Pokud by se našlo P řešení pro jeden NP-úplný problém, **celá NP třída by se „zhroutila"** do P.

> **Věta:** Pokud by nějaký NP-úplný problém byl řešitelný v deterministickém polynomiálním čase, pak by platilo $P = NP$.

> **Věta:** Žádný EXPTIME-úplný problém není řešitelný v deterministickém polynomiálním čase.

> **Věta (důkaz NP-úplnosti redukcí):** Je-li $L \in NP$ a existuje-li NP-úplný problém $L'$ takový, že $L' \leq_p L$, pak i $L$ je NP-úplný.

Důkaz NP-úplnosti „od nuly" je obtížný $\Rightarrow$ dělá se to jen pro určité **kanonické** NP-úplné problémy, na které se pak ostatní problémy redukují.

## P vs. NP – dva možné světy

| $P \neq NP$ | $P = NP$ |
|-------------|----------|
| P $\subsetneq$ NP $\subsetneq$ NP-Hard, NP-Complete tvoří „vrchol" NP mimo P | $P = NP = NP\text{-Complete}$, vše splývá |
![[p-np.png|365]]
# Známé problémy

## P problémy

- **Výpočet největšího společného dělitele** (NSD)
- **Rozhodnutí prvočíselnosti**

## NP problémy

- **Faktorizace** $\Rightarrow$ nalezení prvočíselného rozkladu.
	- Na faktorizaci staví **asymetrická šifra**.
	- Ověření lze provést polynomiálně (prostě ta prvočísla vynásobíme).
- **Izomorfismus grafů** $\Rightarrow$ rozhodnutí, zda jsou 2 grafy izomorfní.
- **SUBSET-SUM** – INPUT: konečná množina $M$ obsahující celá čísla, celé číslo $t$. OUTPUT: *True*, pokud existuje podmnožina $X \subseteq M$ taková, že součet prvků množiny $X$ je $t$; jinak *False*.
- **Celočíselné programování** – rozhodnout, zda daná soustava lineárních nerovnic má řešení v oboru celých čísel.
- **SAT** (splnitelnost výrokové formule) – rozhodnout, zda lze proměnným v dané výrokové formuli přiřadit pravdivostní hodnoty tak, aby se celá formule vyhodnotila na *True*.

## NP-úplné problémy

- **3SAT** je NP-úplný problém splnitelnosti výrokových formulí (booleovské formule).
	- V praxi existují algoritmy, které řešení zvládnou ve většině případů rychle (**SAT-solvery**).
- **Problém obchodního cestujícího (TSP):** najít v zadaném ohodnoceném úplném grafu kružnici, která prochází všemi vrcholy a má **minimální cenu** (nejkratší hamiltonovská kružnice).
	- Optimalizační varianta je **NP-Hard**.
	- Rozhodovací varianta „Existuje hamiltonovská kružnice kratší než $x$?" je **NP-úplná**.
- **Problém batohu** – úloha kombinatorické optimalizace: umístit podmnožinu předmětů (každý má váhu a cenu) do přepravky omezené kapacity tak, aby cena nákladu byla **maximální**. NP-úplný.
- **VERTEX-COVER** – INPUT: neorientovaný graf $G = (V, E)$, přirozené číslo $k$. OUTPUT: *True*, pokud existuje množina vrcholů $C \subseteq V$ taková, že $|C| \leq k$ a každá hrana grafu je incidentní nějakému vrcholu z $C$; jinak *False*.
- **CLIQUE** – INPUT: neorientovaný graf $G = (V, E)$, přirozené číslo $k$. OUTPUT: *True*, pokud existuje množina vrcholů $C \subseteq V$ taková, že $|C| \geq k$ a každé dva různé vrcholy z $C$ jsou spojeny hranou; jinak *False*.

## EXP problémy

- **Šachy**

## Nerozhodnutelné problémy

- **Halt** (zároveň NP-Hard)
- **CFG-Equality**
