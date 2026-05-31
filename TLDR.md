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
