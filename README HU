# SmartHome Database System

**Microsoft SQL Server | Relációs adatbázis-tervezés | T-SQL | Üzleti intelligencia**

Relációs adatbázis-tervezési és -megvalósítási projekt egy fiktív okosotthon-telepítéssel foglalkozó vállalat, a Smart Homes számára. A projekt középpontjában az adatbázis-architektúra, az adattáblák közötti kapcsolatok, az üzleti folyamatok, az SQL-lekérdezések, az automatizált üzleti szabályok és az elemző riportok állnak.

## Projektáttekintés

A rendszer egy okosotthon-telepítéssel foglalkozó vállalat operatív és adminisztratív tevékenységeinek támogatására készült.

Egyetlen relációs adatbázis-struktúrában egyesíti az ügyfélkezelést, az ingatlanok, az okosotthon-eszközök és a telepítések nyilvántartását, a munkatársak beosztását, a beszállítók és a készletek kezelését, valamint a rendelések, számlák és fizetések adatait.

A megvalósítás a relációs adatbázisok alapelveit gyakorlati SQL-fejlesztéssel ötvözi, különös tekintettel az adatok konzisztenciájára, a normalizálásra, a referenciális integritásra és az üzleti szabályok érvényesítésére.

## Technológiai háttér

- **Microsoft SQL Server** – Relációs adatbázis-kezelés.
- **T-SQL** – Lekérdezések, tárolt eljárások és triggerek megvalósítása.
- **Visual Paradigm** – Egyed-kapcsolat diagram (ERD) tervezése.
- **SQL Server Management Studio (SSMS)** – Adatbázis-megvalósítás és SQL-lekérdezések futtatása.
- **Dashboard és adatvizualizáció** – Üzleti teljesítmény és működési eredmények bemutatása.

## Adatbázis-tervezés

Az adatbázis egyed-kapcsolat diagram (ERD) alapján készült, amely meghatározza az egyedeket, attribútumokat, elsődleges és idegen kulcsokat, valamint a közöttük lévő kapcsolatokat.

Az adatbázis főbb komponensei:

- CLIENTS & PROPERTIES – Ügyfél- és ingatlanadatok kezelése.
- STAFF & TEAMS – Munkatársi adatok és telepítőcsapatok beosztása.
- DEVICES & CONTROLLERS – Okosotthon-eszközök és kompatibilitási információk.
- INSTALLATIONS & DESIGNS – Telepítések és ügyfélspecifikus tervek nyilvántartása.
- SUPPLIERS & STOCK – Beszállítói kapcsolatok és készletkezelés.
- ORDERS & DEVICE_ORDERS – Beszerzések és eszközrendelések kezelése.
- INVOICES & PAYMENTS – Számlázás és pénzügyi tranzakciók kezelése.
- SENSOR_READINGS & DATACENTER – Szenzoradatok és adatnyilvántartás.
- MAINTENANCE_CALLOUTS – Karbantartási és szerviztevékenységek kezelése.

![DB Layout](./screenshots/DB%20Layout.png)

## Adatbázis-alapelvek

A megvalósítás az alábbi adatbázis-tervezési elveket alkalmazza:

- Első, második és harmadik normálforma (1NF, 2NF, 3NF).
- Funkcionális függőségek elemzése.
- Elsődleges és idegen kulcsok meghatározása.
- Összetett kulcsok és relációs kapcsolatok.
- Referenciális integritás biztosítása.
- Adattípusok kiválasztása és mezőszintű megszorítások.
- Egy-a-többhöz és több-a-többhöz kapcsolatok kialakítása.

## SQL-megvalósítás

A projekt több SQL-lekérdezést és adatbázis-műveletet tartalmaz, amelyek a T-SQL gyakorlati alkalmazását mutatják be.

| **Megvalósítás** | **Funkcionalitás** |
|---|---|
| Client_Cost_Total | A legmagasabb és legalacsonyabb ügyféloldali tervezési költség azonosítása. |
| WiFi_Order_Status | Wi-Fi-eszközök rendeléseinek elemzése beszállítók és rendelési státuszok szerint. |
| Weekly_Availability | A munkatársak elérhetőségének vizsgálata a következő hét napban. |
| Double_Booking_Avoidance | Adatbázis-trigger az egymással ütköző munkatársi beosztások megelőzésére. |
| Installation_Costs | Telepítési költségek számítása heti, havi és negyedéves időszakok alapján. |
| Dashboard | Üzleti teljesítmény és működési trendek vizualizációja. |

![Installation Creation](./screenshots/Intallations%20Table%20Creation.png)

![Installations Content](./screenshots/Intallations%20Table%20Content.png)

### Haladó SQL-technológiák

- Többtáblás JOIN műveletek.
- Aggregáló függvények és feltételes COUNT kifejezések.
- GROUP BY és HAVING.
- Dátumkezelés GETDATE() és DATEADD() függvényekkel.
- Tárolt eljárások és bemeneti paraméterek.
- Ablakfüggvények és PARTITION BY.
- Adatbázis-triggerek.
- Tranzakció-visszagörgetés és hibakezelés.
- Összetett kulcsok és relációs megszorítások.

![Installation Costs Query](./screenshots/Installation%20Costs%20Query.png)

![Installation costs per week, month, quarter](./screenshots/Installation%20costs%20per%20week,%20month,%20quarter.png)

## Tervezési döntések és fejlesztési kihívások

A megvalósítás során az eredeti adatbázisterv több ponton módosult annak érdekében, hogy megfeleljen a működési követelményeknek és a lekérdezések technikai igényeinek.

Néhány példa:

- További telepítési dátummezők bevezetése a dátumalapú lekérdezések támogatására.
- Az eszközrekordok bővítése vezérlőkompatibilitási és készletinformációkkal.
- A csapatok azonosítóinak és kulcsstruktúráinak módosítása.
- Egyedi munkatársi beosztást ellenőrző trigger létrehozása az átfedő telepítések kezelésére.

A fejlesztés során különböző adattípusok, NULL értékek, adatbázis-megszorítások és a sémamódosítások gyakorlati következményeinek vizsgálata is szerepet kapott.

Ezek a döntések a fejlesztési folyamat részét képezik, és bemutatják, milyen szempontokat igényel egy elméleti adatbázisterv működőképes rendszerré alakítása.

![Double Booking Avoidance](./screenshots/Double%20Booking%20Avoidance.png)

![Double booking avoidance proof](./screenshots/Double%20booking%20avoidance%20proof.png)

## Dashboard és üzleti intelligencia

A dashboard az üzleti működés több területét mutatja be:

- Ügyfél- és telepítési trendek.
- Eszközválaszték és telepítési aktivitás.
- Ügyfélköltések.
- Pénzügyi és működési eredmények.
- Lehetséges üzleti lehetőségek és ügyféltrendek.

A cél a relációs adatbázisban tárolt információk olyan üzleti szempontból értékes elemzésekké alakítása, amelyek támogathatják a működési és stratégiai döntéseket.

## Projekt dokumentációja

A repository tartalma:

- Adatbázis-terv és ER-diagramok.
- Funkcionális függőségek dokumentációja.
- SQL-lekérdezések és azok eredményei.
- Adatbázis-képernyőképek.
- Dashboard-vizualizációk.
- Projektbemutató videó (amennyiben elérhető).

![Screenshot 2026-11-09 155521](./screenshots/Screenshot%202026-11-09%20155521.png)

## Projekt háttere

A projekt eredetileg egy egyetemi tantárgy keretében készült.

Ez a repository az önállóan kidolgozott adatbázistervet, SQL-megvalósítást és technikai dokumentációt mutatja be személyes szakmai portfólió részeként.

**Microsoft SQL Server | T-SQL | Adatbázis-fejlesztés | Relációs adatmodellezés | Üzleti intelligencia**

## Adatvizualizáció és elemzés

A **Tableau** a Microsoft SQL Server adatbázishoz csatlakoztatva készült az adatok vizualizálására, az SQL-lekérdezések eredményeinek elemzésére és az üzleti információk szemléltetésére.

**SQL-lekérdezések:**
- Munkatársak dupla foglalásának megelőzése
- Telepítési költségek
- Heti munkatársi elérhetőség
- Wi-Fi-rendelések státusza

**Tableau-dashboardok és vizualizációk:**
- Telepítések alakulása időben
- Ügyfélköltések
- Tervekhez kapcsolódó telepítések időbeli alakulása
- Telepített eszköztípusok
- Telepítések városonként

![Tablou stats](./screenshots/Tablou%20stats.png)

![tablou client spenditure.png](./screenshots/tablou%20client%20spenditure.png)

![tablou device types installed](./screenshots/tablou%20device%20types%20installed.png)

![tablou installations by city](./screenshots/tablou%20installations%20by%20city.png)

A teljes projektről készült videóbemutató ami kérésre elérhető.

Szerzői jogok és felhasználási feltételek

Copyright © 2026 Major László. Minden jog fenntartva.

Ez a repository nyilvánosan elérhető portfólió- és oktatási bemutatási célokból.

A forráskód megtekintésre és értékelésre szolgál. A szerző előzetes írásbeli engedélye nélkül a projekt másolása, módosítása, terjesztése vagy kereskedelmi célú felhasználása nem engedélyezett.

A harmadik féltől származó könyvtárakra és függőségekre azok saját licencfeltételei vonatkoznak.
