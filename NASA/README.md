# Projekt: Wykrywanie potencjalnie niebezpiecznych asteroid (NASA NEO Dataset)

## Cel projektu  
Celem projektu było zbudowanie modelu klasyfikacyjnego, który potrafi wykrywać potencjalnie niebezpieczne asteroidy na podstawie danych NASA NEO (Near Earth Objects).  

## Etapy pracy  
1. **EDA (Exploratory Data Analysis)**  
   - Analiza rozkładów zmiennych numerycznych i kategorycznych.  
   - Sprawdzenie braków danych i duplikatów.  
   - Wizualizacja zależności pomiędzy cechami a zmienną docelową (`hazardous`).  

2. **Preprocessing**  
   - Skalowanie cech numerycznych i balansowanie klas.  
   - Usunięcie zbędnych kolumn (`id`, `name`) — jako początkująca uznałam je za nieistotne dla trenowania, nie przewidując wtedy, że mogłyby ułatwić późniejszą identyfikację asteroid.  

3. **Modelowanie**  
   - Przetestowane algorytmy: Logistic Regression, Random Forest, XGBoost.  
   - Porównanie przy użyciu metryk: Accuracy, Precision, Recall, F1-score.  
   - Najlepsze wyniki uzyskał **XGBoost**, zapewniając wysoką skuteczność w wykrywaniu potencjalnie niebezpiecznych asteroid.  

4. **Wnioski**  
   - Najważniejsze cechy wpływające na klasyfikację to: `est_diameter_max`, `relative_velocity` i `miss_distance`.  
   - Rekomendowany do dalszego wykorzystania jest **XGBoost**, ze względu na najlepsze wyniki równoważące precyzję i czułość.  
   - Projekt pozwolił mi jako początkującej przećwiczyć różne techniki EDA, preprocessing i modelowania.  


## Instrukcje uruchamiania

## Klonowanie repozytorium

### Opcja A — przez HTTPS
```bash
git clone https://github.com/infoshareacademy/jdszr20-miniprojekty.git
cd jdszr20-miniprojekty/miniprojekt-2
git checkout Anna-Gruszczynska

### Opcja B — przez SSH (zalecane)

Wymaga dodanego klucza SSH do GitHuba.

git clone git@github.com:infoshareacademy/jdszr20-miniprojekty.git
cd jdszr20-miniprojekty/miniprojekt-2
git checkout Anna-Gruszczynska


Tipy:
- Jeśli `ssh -T git@github.com` zwróci „Permission denied (publickey)”, upewnij się, że klucz jest dodany w GitHub oraz że działa agent:
  ```bash
  eval "$(ssh-agent -s)"
  ssh-add ~/.ssh/id_ed25519

Utworzenie i instalacja środowiska

python -m venv venv

# Windows (Git Bash)

source venv/Scripts/activate

# Windows (PowerShell/CMD)

.\venv\Scripts\activate

# macOS/Linux

source venv/bin/activate


## Instalacja zależności

Zalecane: Python 3.11+. Najpierw utwórz i aktywuj wirtualne środowisko, potem zainstaluj paczki z `requirements.txt`.

Windows (PowerShell, cmd)

```bash
python -m venv venv
.\venv\Scripts\activate
python -m pip install -r requirements.txt

Windows (Git Bash)

python -m venv venv
source venv/Scripts/activate
python -m pip install -r requirements.txt

macOS / Linux

python3 -m venv venv
source venv/bin/activate
python -m pip install -r requirements.txt

Weryfikacja

python -c "import pandas, sklearn, xgboost; print('OK')"

Aktualizacja pliku

python -m pip freeze > requirements.txt

Uruchomienie
Notebook:

jupyter notebook analiza.ipynb

