# Az INFORMATIKA ÉS TÁVKÖZLÉS ágazathoz tartozó 
- 5 0613 12 03 SZOFTVERFEJLESZTŐ ÉS –TESZTELŐ SZAKMA
- 5 0612 12 02INFORMATIKAI RENDSZER- ÉS ALKALMAZÁSÜZEMELTETŐ TECHNIKUS SZAKMA

ágazati alapvizsga python vizsgájára felkészítő egyszerű feladatok,
de bármelyik programozási nyelv megismeréséhez használhatóak

A python megoldások: https://github.com/borossandor27/pythonGyakorloFeladatok.git

A megoldások nem a nyelv szépségét kívánják bemutatni, nem használják ki az összes nyelvi lehetőséget, hanem a sikeres vizsgához szükséges ismereteket próbálják bemutatni

## ***f00*** Kéktúra 
Az Országos Kéktúra Magyarország északi részén végighaladó folyamatos, jelzett
turistaút. A Kéktúrának a Balaton-Felvidéken is több, rövidebb idő alatt bejárható túrája van. Egy ilyen túra adatait kell feldolgoznia ebben a feladatban.
- ```kektura.csv``` állomány beolvasása után egyszerű kimutatások készítése

## ***f01*** Expedíció 
Valamikor a távközlés hőskorában egy ritka farkasfaj tudományos megfigyelésére
expedíciót szerveztek a sarkkörön túlra. A magukkal vitt rádió csak napi egy adásra volt alkalmas, arra is csak 90 időegységig, időegységenként egy karaktert továbbítva.
Az expedíció rádiósának üzeneteit több rádióamatőr is igyekezett lejegyezni. A feladatban a rádióamatőrök által lejegyzett üzeneteket kell feldolgoznia.
A ```veetel.txt``` fájl tartalmazza a rádióamatőrök által feljegyzett üzeneteket.

## ***f02*** Ötszáz 
Egy apróságokat árusító boltban minden árucikk darabja 500 Ft. Ha egy vásárlás során
valaki egy adott árucikkből több darabot is vesz, a második ára már csak 450 Ft, a harmadik pedig 400 Ft, de a negyedik és további darabok is ennyibe kerülnek, tehát az ár a harmadik ugyanazon cikk vásárlása után már nem csökken tovább.

## ***f03*** Tesztverseny 
Egy közismereti versenyen a versenyzőknek 13+1, azaz összesen 14 tesztfeladatot tűznek ki. A versenyzőknek minden feladat esetén négy megadott lehetőség (A, B, C, D) közül kell a helyes választ megjelölniük. A versenybizottság garantálja, hogy tesztlapon minden kérdéshez pontosan egy helyes válasz tartozik. A kitöltött tesztlapokat elektronikusan rögzítik, a visszaélések elkerülése végett a versenyzőket betűkből és számokból álló kóddal azonosítják.

## ***f04*** Társalgó
Egy színház társalgójában még a délelőtti próbák alatt is nagy a forgalom. A színészek hosszabb-rövidebb beszélgetésekre térnek be ide, vagy éppen csak keresnek valakit. A feladatban a társalgó ajtajánál 9 és 15 óra között felvett adatokat kell feldolgoznia.

## ***f05*** Levenshtein-távolság
A következő algoritmus két, maximum 25 karakter hosszú karakterláncról megállapítja,
hogy mekkora a Levenshtein-távolságuk, azaz minimálisan hány karakterenkénti művelet
(beszúrás, törlés, csere) kell ahhoz, hogy az egyik karakterláncot a másikra átalakítsuk. Kódolja az algoritmust a választott programozási nyelven! 

## ***f06*** Pontok 
Ebben a feladatban egy szöveges állományban x, y koordinátákkal megadott pontokat kell vizsgálnia. Minden pont adata külön sorba került a forrásállományban a sorszámuk
alapján...

## ***f07*** Shell rendezés
A következő algoritmus a Shell rendezés algoritmusával rendezi az N elemű (N<100)
vektorban megadott számokat növekvő sorrendben.
Kódolja az algoritmust a választott programozási nyelven! Az elkészült program
forráskódját mentse shellsort néven!

A megoldás során vegye figyelembe a következőket:
- A választott programozási nyelvtől függően eltérő jelölésű operátorokat,
adattípusokat és függvényeket kell alkalmaznia.
- A ”div” az egészosztás operátora.
- Az egész típusú változókhoz és vektorokhoz használjon 32 bites előjeles adattípust!

```
Eljárás ShellRendezes(a:Tömb[0..N] Egész)
> Változó gap, n, i, j, x, y : Egész
> gap := 1
> n := a.Hossz //a vektor elemszáma
> Ciklus amíg (gap * 2 <= n)
> gap := gap * 2
> Ciklus vége
> gap := gap - 1
>Ciklus
>i := 0
>Ciklus amíg ((i <= gap) ÉS (i + gap < n))
>j := i + gap
>Ciklus amíg (j < n)
>x := a[j]
>y := j – gap
>Ciklus amíg ((x > -1) ÉS (x < a[y]))
>a[y + gap] := a[y]
>y := y – gap
>Ciklus vége
>a[y + gap] := x
>j := j + gap
>Ciklus vége
>i := i + 1
>Ciklus vége
>gap := gap div 2
>amíg (gap > 0)
>Ciklus vége
Eljárás vége
Program shellsort
Változó t: Tömb[0..9] Egész
t[0] := 63
t[1] := 54
t[2] := 33
t[3] := 45
t[4] := 23írásbeli vizsga, II. összetevő 8 / 20 2016. október 17.
1621
Informatikai alapismeretek — emelt szint Azonosító
jel:
t[5] := 99
t[6] := 43
t[7] := 10
t[8] := 35
t[9] := 87
ShellRendezes(t)
Ciklus i:=0 -tól 9 –ig (+1 lépésközzel)
Ki: t[i]
Ciklus vége
Program vége
