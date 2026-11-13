# Klasyfikacja potencjalnie niebezpiecznych asteroid — NASA NEO

Projekt edukacyjny z analizy danych i uczenia maszynowego w Pythonie, wykonany podczas kursu Data Science w infoShare Academy.

## Cel projektu

Zbudowanie i porównanie modeli klasyfikujących obiekty bliskie Ziemi na podstawie cech zawartych w zbiorze NASA NEO. Zmienną docelową jest oznaczenie `hazardous`.

## Zakres pracy

- Eksploracyjna analiza danych (EDA): rozkłady, braki danych, duplikaty i zależności między zmiennymi.
- Przygotowanie danych: skalowanie cech i balansowanie klas.
- Porównanie modeli: regresja logistyczna, Random Forest i XGBoost.
- Ocena modeli za pomocą Accuracy, Precision, Recall i F1-score.

Według podsumowania projektu najlepsze wyniki spośród porównanych modeli uzyskał XGBoost. Szczegóły analizy i wyniki znajdują się w notebooku.

## Technologie

Python · Jupyter Notebook · pandas · scikit-learn · XGBoost

## Pliki projektu

Pliki znajdują się w folderze [NASA](./NASA):

- [Notebook z analizą](./NASA/notebooks/analiza.ipynb)
- [Dane](./NASA/data)
- [Wymagane biblioteki](./NASA/requirements.txt)
- [Pierwotna dokumentacja projektu](./NASA/README.md)

## Uruchomienie

1. Pobierz repozytorium.
2. Przejdź do folderu `NASA`.
3. Utwórz i aktywuj wirtualne środowisko Pythona.
4. Zainstaluj biblioteki: `python -m pip install -r requirements.txt`.
5. Otwórz `notebooks/analiza.ipynb` w Jupyter Notebook.

Projekt ma charakter edukacyjny — nie służy do operacyjnej oceny zagrożeń astronomicznych.

## Autorka

Anna Gruszczyńska
