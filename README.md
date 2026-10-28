# Work Command Center · Web Demo

Egyszerűsített, magyar nyelvű interaktív bemutató, kizárólag kitalált adatokkal. Az eredeti app működési elvét mutatja meg; nem tartalmazza annak adatbázisát vagy mentéseit.

## 1 perces bemutató

1. **Mai nap:** válassz legfeljebb három fókuszt a csillagokkal.
2. Jelöld késznek a „Visszajelzések összegzése” lépést. A projekt haladása frissül.
3. **Projektek:** nyisd meg az Ügyfélportál projektet. Látható a projekt → feladat → következő lépés felépítés.
4. Egy feladat címére kattintva módosíts státuszt, céldátumot, várakozást vagy 10 perces lépést.
5. **Riportok:** nézd meg és másold ki a friss összefoglalót.
6. **Demó alaphelyzetbe:** bármikor újrakezdhető a bemutató.

## Működés és korlátok

- Statikus HTML/CSS/JavaScript, szerveroldali kód és külső függőség nélkül.
- A változások a saját böngésző localStorage tárolójába kerülnek (`wcc-public-demo-v1`). A látogatók egymástól független példányokat használnak.
- A demó induló dátumai az első megnyitás napjához képest készülnek. Az alaphelyzetbe állítás friss dátumokkal indít újra.
- A napi fókusz új napon nullázódik. A legutolsó módosítás visszavonható, amíg újabb módosítás vagy oldalfrissítés nem történik.
- Nyitott lépésekkel rendelkező feladat lezárásakor külön megerősítés jelenik meg; a kapcsolódó lezárás együtt vonható vissza.
- A projekt haladása a lezárt feladatok és lépések aránya. A mérföldkövek külön követhetők.
- A riport egy aktuális állapotkép, nem az eredeti app teljes napi/heti riportmodulja. A másolás nem küldi el senkinek.
- Nincs import, bejelentkezés, analitika vagy adatküldés. Valós vagy bizalmas adatot ne írj bele.

## GitHub Pages

A repó **Settings → Pages** menüjében:

- Source: **Deploy from a branch**
- Branch: **main**
- Folder: **/ (root)**
- **Save**

Minden hivatkozás relatív, ezért a webapp a repó almappás Pages-címén is működik.

## Helyi megnyitás

Nyisd meg az `index.html` fájlt egy modern böngészőben. A másoláshoz és a stabil helyi adattároláshoz ajánlott HTTP-kiszolgálót használni, például: `python3 -m http.server 8000`.
