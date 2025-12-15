# kaloz_kocka_beadando_12.15
README.md
🏴‍☠️ Kalóz Kocka Játék

Ez egy egyszerű mobil dobókocka játék Androidra, ahol két játékos verseng, hogy ki gyűjt össze előbb 20 pontot. A játék az ún. “Dönts okosan” játékon alapul, ahol a kockadobások és a kockázat fontos szerepet játszanak.

Játékszabályok

A játékot két játékos játszhatja, felváltva.

Minden körben a játékos legfeljebb 3 dobást tehet.

Minden dobott szám hozzáadódik a kör pontjaihoz, kivéve, ha 1-est dob:

Ha 1-est dob, az adott kör pontjai elvesznek, és a következő játékos következik.

A játékos bármikor megállhat, ekkor a kör pontjait hozzáadja az összpontjaihoz, és a következő játékos jön.

A játékot az a játékos nyeri, aki először eléri a 20 pontot.

Telepítés

Android Studio telepítése szükséges.

Hozz létre egy új projektet a csomag névvel: com.example.beadando1215.

Másold a MainActivity.java fájlt a java/com/example/beadando1215/ könyvtárba.

Másold a activity_main.xml fájlt a res/layout/ könyvtárba.

Másold a dobókocka képeket (dice1.png … dice6.png) és a háttérképet (hatter.jpeg) a res/drawable/ könyvtárba.

Futtasd az alkalmazást egy Android eszközön vagy emulátoron.

UI elemek

Dobókocka kép: A dobott számnak megfelelő képet jeleníti meg.

Kör pontja: Megmutatja az aktuális körben szerzett aranyat.

Összpontok: Külön-külön a két játékos összegyűjtött pontjait mutatja.

Dobás gomb: Dob a kockával.

Stop gomb: Megállítja a kört, és hozzáadja a körpontot az összpontokhoz.

Legutóbbi dobás: Megmutatja az utolsó dobást és az aktuális kör pontjait.

Fontos változók

currentPlayer – aktuális játékos (0 = Kalóz 1, 1 = Kalóz 2)

korArany – aktuális kör pontjai

osszPont – játékosok összpontjai

dobasszam – dobások száma egy körben (max 3)

Kód működése

dobas() – kockadobás kezelése, 1-es dobás esetén kör elvesztése.

megall() – kör véglegesítése és pontok hozzáadása.

jatekosValtas() – váltás a következő játékosra.

frissitUI() – az összes TextView frissítése a képernyőn.

gyozelem() – felugró ablak a nyertes játékosról.

ujJatek() – visszaállítja az összes változót az új játékhoz.
