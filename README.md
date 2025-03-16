# 074_Liveability_Hungarian_microregions  
🔍 Melyik magyar kistérség a legélhetőbb? 📊
📌 Az OpenStreetMap adatai és a 🐍python segítségével elkészítettem a Magyarországi kistérségek élhetőségi indexét. A cél egy olyan térkép létrehozása volt, amely különböző életminőségi faktorokat figyelembe véve rangsorolja a magyar kistérségeket. Persze tudom, hogy egy Liveability index sokkal több adatból tevődik össze, de itt csak azokkal tudtam számolni, amik az OpenStreetMapről letölthetők.
💡 Milyen adatok alapján készült az elemzés?
 ✅ Népesség és népsűrűség
 ✅ Parkok és zöldterületek aránya
 ✅ Iskolák és múzeumok száma
 ✅ Úthálózat hossza
🛠 Módszertan
1️⃣egy webscraping szkript írása, amely Magyarország kistérségeinek listáját és népességét gyűjti ki a Wikipédiáról és Excel fájlba menti az adatokat 📊
2️⃣ezen lista alapján a kistérségek adatainak letöltése az OpenStreetMap-ről, majd mentése egy mappába (870 fájl, 162MB) innen töltjük majd be
3️⃣maga a fő program megírása, ami a geopandas, osmnx, matplotlib és contextily segítségével térképi elemzést végez. Az adatok normalizálása után egy súlyozott indexet számítottam, amely alapján vizuálisan is ábrázoltam az eredményeket.
📌 Az eredmény egy térkép, amely megmutatja, hogy Magyarország mely kistérségei kínálnak kedvezőbb életkörülményeket.
