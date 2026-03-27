# ip2-project-2026
Samostalni projekat iz predmeta Istraživanje podataka 2 na Matematičkom fakultetu.

## Napomena

Pre pokretanja sveski, neophodno je otpakovati arhivu `communities+and+crime+unnormalized.zip` kako bi se dobio fajl `CommViolPredUnnormalizedData.txt`, koji predstavlja polazni skup podataka.

## Struktura projekta

### `data/`
Sadrži raznolike verzije skupa podataka nastale tokom preprocesiranja — od originalnih podataka sa imputiranim vrednostima, do transformisanih i PCA-redukovanih verzija koje se koriste u klasterovanju.

### `notebooks/`
Sadrži Jupyter sveske koje pokrivaju sve faze analize: preprocesiranje i eksploratornu analizu podataka (`01_preprocessing_eda.ipynb`), primenu algoritama klasterovanja (`02_clustering.ipynb`) i evaluaciju rezultata (`03_evaluation.ipynb`).

### `figures/`
Sadrži sve vizuelizacije generisane tokom analize — distribucije atributa, PCA projekcije, rezultate klasterovanja i dr.

### `results/`
Pokretanjem sveske `02_clustering.ipynb`, u direktorijum `results/` biće upisani `.pkl` fajlovi (`results_kmeans.pkl`, `results_agglomerative.pkl`, `results_dbscan.pkl`, `results_clarans.pkl`, `results_birch.pkl`, `results_cure.pkl`, kao i `all_results.pkl` koji ih sve objedinjuje). `.pkl` fajlovi su serijalizovani Python objekti koji čuvaju rečnike sa rezultatima svakog algoritma klasterovanja, što omogućava učitavanje rezultata u svesci `03_evaluation.ipynb` bez ponovnog pokretanja klasterovanja.

## Dokumentacija

### `seminarski_rad.pdf`
Tekstualni deo seminarskog rada koji detaljno opisuje tok analize i interpretaciju dobijenih rezultata.
