# Vaja v Excelu - Frekvenca velikih potresov

Veliki potresi so potresi z magnitudo nad 7. **Kako pogosto pa do takih potresov pride?** Na to vprašanje bomo v okviru te vaje odgovorili z zanimivimi nalogami, hkrati pa se bomo naučili veliko uporabnih funkcij Excela.
## Veliki potresi

V Združenih državah Amerike se vsako leto zgodi med 10 in 15 velikih in približno en ogromen (magnituda nad 8) potres. Da se zares zavemo, kako močan je ogromen potres: potres z magnitudo 8 je približno 32-krat močnejši kot potres z magnitudo 7. To pomeni, da je ogromen potres vsaj 1000-krat močnejši kot potres z magnitudo 6!


## **Naloge** 
Podatki, na katerih slonijo sledeče naloge so malce starejši, zato je poleg te PDF datoteke za vas pripravljena tudi excel datoteka, kjer so za vas zbrani vsi potrebni podatki.
## Naloga 1, List 1
Pred vami so zbrani podatki o številu velikih potresov med leti 1970 in 1999 v ZDA. 

> Izračunajte število let, med katerimi so izbrani podatki in število vseh potresov. Izračunajte tudi povprečno število potresov na leto. Podatki naj bodo zaokroženi na eno decimalno mesto.

**NAMIG:**
Podatke lahko izračunate ročno ali pa uporabite excelove funkcije COUNT, SUM in AVERAGE. Za zaokroževanje se uporablja funkcija ROUND.

**DODATNO:** Iz stolpca B izbrišite kakšen podatek in ga nadomestite z izbrano črko. Premislite, kaj se zgodi.

Ob koncu naloge 1 bi morali dobiti sledeče podatke:


<img src=slika2.png alt="Naloga 1" width=150>

___

## Naloga 2, List 2
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
## Naloga 3, List 3
>Uredite podatke o potresih od največjega do najmanjšega. Izračunajte ***maksimum, minimum in obseg*** števila potresov.

**NAMIG:**
Podatkov vam ni potrebno urejati na roke. Le izberite vse podatke, jih skopirajte v izbran stolpec in izberite možnost **Sort**. Ne pozabite, da podatke urejate glede na število potresov in ne glede na leto.

Za ***maksimum in minimum*** uporabite funkcij MAX in MIN (funkciji uporabite na stolpcu B), ***obseg*** pa izračunajte kot razliko zgornjih dveh.


List po koncu naloge 3:

<img src=slika4.png alt="Naloga 3" width=300>

___

## Naloga 4, List 3
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

## Naloga 5, List 3
**Mediana** je srednja vrednost zaporedja števil, ki razdeli števila, razvrščena po velikosti, na dve enaki polovici po številu elementov.

**Kvartil** je ena od 3 vrednosti, ki delijo množico na štiri enake dele.

>Izračunajte število vseh podatkov, sredinsko pozicijo ter pozicijo prvega in tretjega kvartila.

**NAMIG:** Za 30 podatkov je sredinska pozicija enaka $$\frac{31}{2},$$ za pozicijo prvega kvartila $$\frac{31}{4},$$ za pozicijo tretjega pa $$\frac{31}{\frac{3}{4}}.$$

Za računanje mediane in kvartilov obstajajo tudi excel formule:

>Izračunajte mediano in vse tri kvartile s formulama **MEDIAN** in **QUARTILE**.

**RAZMISLEK:** Kaj ugotovite o srednjem kvartilu (Q2)?

Izgled lista 3 po nalogi 5:

<img src=slika8.png alt="Naloga 5" width=300>

___

## Naloga 6, List 4
**Percentil** je število, ki nam pove odstotek podatkov, ki imajo nižjo vrednost od izbranega podatka.

Excel z uporabo percentilov računa kvartile.

Mediana je 50. percentil, ker je 50% podatkov nižjih od nje. Q1 je torej 25. percentil, Q2 pa 75. percentil.

Na Listu 4 imate podatke urejene po velikosti z dodano razvrstitvijo od spodaj navzgor. 

>Ob danih podatkih izračunajte percentile za vse vrednosti. Podatki naj bodo zaokroženi na dve decimalni mesti.

**NAMIG:** Za leto 1970 je prava formula za računanje perecntilov.jkhsjhkcjhklhdshkjkjndsf