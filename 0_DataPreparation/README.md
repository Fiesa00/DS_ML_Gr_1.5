# Data Preparation


Für das Bakery Sales Predictions wurden verschiedene Variablen vorbereitet, um diese in die jeweiligen Modelle einfließen zu lassen. Die Daten zu den Variabelen wurde per Internet-Recherche gefunden und einzeln als csv-Datei abgespeichert.

Folgende Variablen wurden erstellt:

- **Wetter** 
    - [Niederschlag](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/Wetter-Final.csv)
    - [realtiver Sonnenschein](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/Wetter-Final.csv)
    - [Schneehöhe](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/Wetter-Final.csv)
    - [relative Temperaturen nach jeweilger Jahreszeit (hoch, mittel, niedrig)](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/temperatur_umsatz_bin.csv)
    - [Tageslänge](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/Wetter-Final.csv) 
- [**Schul-/Semesterferien, Feiertage**](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/Ferien-Feiertage-Final.csv)
- [**Werktag**](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/test_weekday_codiert.csv)
- [**Monat**](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/temperatur_umsatz_bin.csv)
- [**Jahreszeit**](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/temperatur_umsatz_bin.csv)
- **Veranstaltungen**
    - [Heimspiel](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/Kiel_Heimspiele.csv)
    - [Weihnachtsmarkt](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/maekte_final.csv)
    - [Saisonmärkte (Herbst- und Frühlingsmarkt)](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/maekte_final.csv)
- [**Inflationsrate (jährlich)**](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/inflation.csv)
- [**Kreuzfahrt/Fährverkehr**](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/passagiere.csv)


Die Variable Preparations (Formatierung, Gruppierung und Binning) wurde in dem [Variablen_preparations](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/Variablen_preparations.ipynb) durchgeführt.


Zusätzlich wurden die gegeben csv-Dateien, wetter.csv, [kiwo.csv](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/kiwo.csv), und umsatz.csv eingelesen und diese mit den erstellten Variablen zusammengeführt. Dies fand im Notebook [Variable_merging](/workspaces/DS_ML_Gr_1.5/0_DataPreparation/Variable_merging.ipynb) statt.

Für die Modelle wurde [merged_data_new.csv](/workspaces/DS_ML_Gr_1.5/2_BaselineModel/merged_data_new.csv) verwendet.

