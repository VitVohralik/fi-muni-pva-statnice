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
