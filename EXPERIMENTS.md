# 🧪 Lab Notebook - Amatrice-Norcia Project

| ID | Data | Commit | Modello & Parametri | Filtri Dati ($M_c$, Zone) | Risultato (b-value) | Note |
|:--:|:----:|:------:|:-------------------|:--------------------------:|:-------------------:|:-----|
| 00 | 07/01| - | Test Iniziale | $M_c > 1.0$, Catalogo Collettini et al | In attesa... | Primo test di configurazione |
| 01 | 08/01| DBSCAN_v1 | **DBSCAN** <br> `eps=1.0 km` <br> `min_samples=50` | $M_w \ge 1.0$ <br> (Tan et al. 2021) | **On-Fault:** 1.25 ✅ <br> **Distributed:** 1.18 ⚠️ | **Successo.** La faglia del Vettore è isolata correttamente (b=1.25). Il valore Distributed è più basso del previsto perché include la faglia di Norcia nel "rumore". |
