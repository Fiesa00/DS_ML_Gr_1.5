# Baseline Model

Lineare Regression (Ordinary Least Squares) wird genutzt, um schon einmal die Features für das neuronale Netzwerk einzugrenzen. 

merged_data_new.csv ist die Datei, die alle Variablen und sonstige Daten erhält.
Es gibt je ein Baseline Model für jede Warengruppe (W1 bis W6) sowie ein Back-up (/workspaces/DS_ML_Gr_1.5/2_BaselineModel/Baseline-Model Backup.ipynb).
BM-Data_export fügt die verschiedenen Vorhersagen der Warengruppen zusammen und erstellt eine für die Kaggle-Abgabe geeignete Datei.(/workspaces/DS_ML_Gr_1.5/2_BaselineModel/BM-Data_export.ipynb)

Die Features für die verschiedenen Warengruppen sind:
W1 Brot (/workspaces/DS_ML_Gr_1.5/2_BaselineModel/Baseline-Model W1.ipynb): 
Sommer
Winter
Monday
Tuesday
Wednesday
Thursday
Friday
Saturday
Sunday
Temp_average
Temp_warm
Temp_cold
Feiertage
Semesterferien
Schulferien
Weihnachtsmarkt
Heimspiel
Markt
KielerWoche


W2 Brötchen (/workspaces/DS_ML_Gr_1.5/2_BaselineModel/Baseline-Model W2.ipynb):
Frühling
Sommer
Herbst
Winter
Werktag
Temp_average
Temp_warm
Temp_cold
Feiertage
Semesterferien
Schulferien
Weihnachtsmarkt
Heimspiel
Markt
KielerWoche

W3 Croissant (/workspaces/DS_ML_Gr_1.5/2_BaselineModel/Baseline-Model W3.ipynb):
Sommer
Winter
Monday
Wednesday
Thursday
Saturday
Sunday
Temp_average
Temp_warm
Temp_cold
Feiertage
Semesterferien
Schulferien
Weihnachtsmarkt
Markt
Sonnenschein
Niederschlag
Tageslaenge

W4 Konditorei (/workspaces/DS_ML_Gr_1.5/2_BaselineModel/Baseline-Model W4.ipynb):
Sommer 
Herbst
Monat
Werktag
Saturday
Temperatur
Temp_cold Niederschlag
Schneehoehe
Sonnenschein
Feiertage
Semesterferien
Schulferien
Weihnachtsmarkt
Heimspiel 
Inflationsrate

W5 Kuchen (/workspaces/DS_ML_Gr_1.5/2_BaselineModel/Baseline-Model W5.ipynb):
Sommer
Herbst
Winter
Wednesday
Friday
Saturday
Sunday
Temp_average
Semesterferien
Werktag
Markt
KielerWoche
Sonnenschein
Niederschlag
Tageslaenge

W6 Saisonbrot (/workspaces/DS_ML_Gr_1.5/2_BaselineModel/Baseline-Model W6.ipynb):
Monat
Werktag
Freitag
Temperatur 
Sonnenschein
Weihnachtsmarkt


