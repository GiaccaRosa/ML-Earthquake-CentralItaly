# 🧪 Lab Notebook - Amatrice-Norcia Project

| ID | Data | Commit | Modello & Parametri | Filtri Dati ($M_c$, Zone) | Risultato (b-value) | Note |
|:--:|:----:|:------:|:-------------------|:--------------------------:|:-------------------:|:-----|
| 00 | 07/01| - | Test Iniziale | $M_c > 1.0$ <br> Catalogo Collettini | In attesa... | Primo test di configurazione. |
| 01 | 08/01| DBSCAN_v1 | **DBSCAN** <br> `eps=1.0` <br> `min_samples=50` | $M_c = 1.0$ | Fault: 1.25 ✅ <br> Dist: 1.18 ⚠️ | Faglia isolata, ma evaporiti mescolate al fondo (b-value distributed basso). |
| 02 | 09/01| DBSCAN_Opt | **DBSCAN** <br> `eps=1.0` <br> `min_samples=20` | $M_c = 1.3$ | **Fault: 1.25** ✅ <br> **Dist: 1.76** ✅ | **TARGET RAGGIUNTO.** Isolamento Evaporiti riuscito. Match perfetto col paper. |
| 03 | 11/01| FASE_2 | **Spatial Cut** <br> (Separazione N/S) | Lat $> 42.76$ <br> (Zona Visso) | N. Eventi: <br> 204.594 | **Isolamento Nucleazione.** Separata la zona Nord (in preparazione) da Amatrice (post-sisma). |
| 04 | 11/01| FASE_3 | **Rolling b-value** <br> `window=2000` | 24 Aug - 26 Oct <br> (Pre-Visso) | **Trend Decrescente** 📉 <br> (Stress Aumenta) |Il b-value crolla prima del 26/10. Prova fisica del caricamento. |
