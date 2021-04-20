

# Vaja v Excelu - Frekvenca velikih potresov
### Kazalo
1. [Uvod](#uvod)
2. [Veliki potresi](#potresi)
3. [Naloge](#naloge)
   1. [Naloga 1](#prva)
   2. [Naloga 2](#druga)
   3. [Naloga 3](#tretja) 
   4. [Naloga 4](#cetrta)
   5. [Naloga 5](#peta)
   6. [Naloga 3](#sesta) 
4. [Ugotovitve](#ugot) 
5. [Dodatne naloge](#dodat)

## Uvod <a name="uvod"></a>
Veliki potresi so potresi z magnitudo nad 7. **Kako pogosto pa do takih potresov pride?** Na to vprašanje bomo v okviru te vaje odgovorili z zanimivimi nalogami, hkrati pa se bomo naučili veliko uporabnih funkcij Excela.
## Veliki potresi <a name="potresi"></a>

V Združenih državah Amerike se vsako leto zgodi med 10 in 15 velikih in približno en ogromen (magnituda nad 8) potres. Da se zares zavemo, kako močan je ogromen potres: potres z magnitudo 8 je približno 32-krat močnejši kot potres z magnitudo 7. To pomeni, da je ogromen potres vsaj 1000-krat močnejši kot potres z magnitudo 6!


## Naloge <a name="naloge"></a>
Podatki, na katerih slonijo sledeče naloge so malce starejši, zato je poleg te PDF datoteke za vas pripravljena tudi excel datoteka, kjer so za vas zbrani vsi potrebni podatki.
### **Naloga 1, List 1** <a name="prva"></a>
Pred vami so zbrani podatki o številu velikih potresov med leti 1970 in 1999 v ZDA. 

> Izračunajte število let, med katerimi so izbrani podatki in število vseh potresov. Izračunajte tudi povprečno število potresov na leto. Podatki naj bodo zaokroženi na eno decimalno mesto.

**NAMIG:**
Podatke lahko izračunate ročno ali pa uporabite excelove funkcije COUNT, SUM in AVERAGE. Za zaokroževanje se uporablja funkcija ROUND.

**DODATNO:** Iz stolpca B izbrišite kakšen podatek in ga nadomestite z izbrano črko. Premislite, kaj se zgodi.

Ob koncu naloge 1 bi morali dobiti sledeče podatke:


<img src=slika2.png alt="Naloga 1" width=150>

___

### **Naloga 2, List 2** <a name="druga"></a>
**Odklon** podatkov predstavlja razliko med njihovo vrednostjo in povprečjem vseh podatkov. 
V nalogi 2 si poglejmo povprečen odklon in varianco populacije.

> Izračunaj odklon števila potresov (stolpec D) in kvadrate odklona (stolpec E). Podatke izračunaj na eno eno decimalno mesto natančno.
> >Izračunaj tudi povprečje odklonov in njegovih kvadratov.
> > Izračunaj tudi kvadratni koren povprečja kvadratov odklonov.

Povprečje odklonov bo seveda enako 0. 
Povprečje kvadratov odklonov imenujemo **varianca populacije**, njegov kvadratni koren pa **standardni odklon populacije**.

Za izbrana podatka obstaja tudi posebna excel formula:

>Izračunaj varianco in standardni odklon z uporabo formul =VARPA(D2:D31) in =STDEVPA(D2:D31). 
>> Podobno izračunaj tudi ***standardni odklon in varianco vzorca*** s formulami VAR in STDEV in premisli, kaj podatka pomenita.

Ob koncu naloge 2 bi moral vaš list izgledati takole:

<img src=slika3.png alt="Naloga 2" width=300>

___
### **Naloga 3, List 3** <a name="tretja"></a>
>Uredite podatke o potresih od največjega do najmanjšega. Izračunajte ***maksimum, minimum in obseg*** števila potresov.

**NAMIG:**
Podatkov vam ni potrebno urejati na roke. Le izberite vse podatke, jih skopirajte v izbran stolpec in izberite možnost **Sort**. Ne pozabite, da podatke urejate glede na število potresov in ne glede na leto.

Za ***maksimum in minimum*** uporabite funkcij MAX in MIN (funkciji uporabite na stolpcu B), ***obseg*** pa izračunajte kot razliko zgornjih dveh.


List po koncu naloge 3:

<img src=slika4.png alt="Naloga 3" width=300>

___

### **Naloga 4, List 3** <a name="cetrta"></a>
**Modus** je vrednost, ki se najbolj pogosto pojavlja v množici vrednosti.
>Izračunajte **modus**. Prav tako izračunajte, kolikokrat je bilo letno:
  - 16 potresov, 
  - 15 potresov,
  - manj kot 16 potresov, 
  - vse, razen 16 potresov.

**NAMIG:** Za računanje ***modusa*** obstaja funkcija MODE (uporabite jo na stolpcu B), za število pojavljanj 16 potresov pa funkcijo COUNTIF.

*COUNTIF* deluje sledeče:
  - COUNTIF(obseg,16) vam poda število pojavljanj 16 v obsegu,
  - COUNTIF(obseg,">16") vam poda, kolikokrat se pojavi vrednost višja od 16,
  - COUNTIF(obseg,"<>16") pa vam poda število vrednosti, ki niso enake 16.
  
> Izračunajte tudi število potresov, ki so se zgodili v letih, ko se je zgodilo 16 potresov, ter število potresov, ki so se zgodili v letih, ko ni bilo 16 potresov.

**NAMIG:** Uporabite funkcijo SUMIF, ki deluje na enak način kot COUNTIF.

Izgled lista 3 po koncu naloge 4:

<img src=slika5.png alt="Naloga 4" width=200>

___

### **Naloga 5, List 3** <a name="peta"></a>
**Mediana** je srednja vrednost zaporedja števil, ki razdeli števila, razvrščena po velikosti, na dve enaki polovici po številu elementov.

**Kvartil** je ena od 3 vrednosti, ki delijo množico na štiri enake dele.

>Izračunajte število vseh podatkov, sredinsko pozicijo ter pozicijo prvega in tretjega kvartila.

**NAMIG:** Za 30 podatkov je sredinska pozicija enaka $$\frac{31}{2},$$ za pozicijo prvega kvartila $$\frac{31}{4},$$ za pozicijo tretjega pa $$\frac{31}{\frac{4}{3}}.$$

Za računanje mediane in kvartilov obstajajo tudi excel formule:

>Izračunajte mediano in vse tri kvartile s formulama **MEDIAN** in **QUARTILE**.

**RAZMISLEK:** Kaj ugotovite o srednjem kvartilu (Q2)?

Izgled lista 3 po nalogi 5:

<img src=slika8.png alt="Naloga 5" width=300>

___

### **Naloga 6, List 4** <a name="sesta"></a>
**Percentil** je število, ki nam pove odstotek podatkov, ki imajo nižjo vrednost od izbranega podatka.

Excel z uporabo percentilov računa kvartile.

Mediana je 50. percentil, ker je 50% podatkov nižjih od nje. Q1 je torej 25. percentil, Q2 pa 75. percentil.

Na Listu 4 imate podatke urejene po velikosti z dodano razvrstitvijo od spodaj navzgor. 

>Ob danih podatkih izračunajte percentile za vse vrednosti. Podatki naj bodo zaokroženi na tri decimalna mesta.

**NAMIG:** Za leto 1970 je prava formula za računanje perecntilov $$(F2-1)/(COUNT(B2:B31)-1).$$ 
Pri pisanju formul ne pozabite na pravilno uporabo znaka $.

Percentili bi morali izgledati takole:

<img src=slika23.png alt="Naloga 6, 1. del" width=300>

Lahko ugotovimo:
  - 75. percentil se zgodi med vrednostjo 20 in 21 ter je bližje slednji, 
  - 25. percentil se zgodi med vrednostjo 11 in 13 ter je bližje vrednosti 11.

Obe ugotovitvi se skladata z izračunom kvartilov v prejšnji nalogi.


Iz percentilov zdaj ni težko izračunati še vrednosti kvartilov z **interpolacijo**.

> Izračunajte kvartile s formulo (za zgornji kvartil):
> $$E10+(0.75-G10)/(G9-G10)*(E9-E10).$$
Za mediano in spodnji kvartil sta formuli zelo podobni, določite ju sami.

***Vaša naloga je s tem zaključena!***

Zadnji del bi moral izgledati takole:

<img src=slika10.png alt="Naloga 6, 2. del" width=300>

___

## Ugotovitve <a name="ugot"></a>

Kaj vse smo izvedeli o velikih potresih v ZDA med leti 1970 in 1999?

- Na leto se je povprečno zgodilo več kot 16 velikih potresov.
- Modus in mediana sta 16.
- Leta 1970 se je zgodilo največ potresov, kar 29, najmanj pa leta 1989 (6), kar nam da obseg 23.
- Q3 je bil 20,75, Q1 pa 11,5, kar nam da medkvartilni obeseg v vrednosti 9,25.

## Dodatne naloge <a name="dodat"></a>

Če želita, lahko podobne naloge izvedete tudi na podatkih o potresih med leti 1940 in 1969, ki jih dobite na [spletni strani](https://seattlecentral.edu/qelp/sets/039/039.html).













<script>
MathJax = {
  tex: {
    inlineMath: [['$', '$'], ['\\(', '\\)']]
  }
};
</script>
<script id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js">
</script>