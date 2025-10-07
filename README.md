# Predikcija-kategorije-proizvoda-na-osnovu-naslova
🧠 Automatizovana klasifikacija proizvoda po kategorijama

Ovaj projekat razvijen je kao deo praktičnog zadatka iz oblasti mašinskog učenja i obrade prirodnog jezika (NLP).
Cilj je automatizovati proces kategorizacije proizvoda na osnovu njihovih naslova (Product Title), čime se značajno smanjuje potreba za ručnim razvrstavanjem proizvoda u online trgovinama.

🎯 Cilj projekta

Kreirati model koji, na osnovu unetog naslova proizvoda, automatski predviđa kojoj kategoriji proizvod pripada (npr. Mobile Phones, Laptops, Fridge Freezers itd).
Ovim pristupom omogućava se:

brži unos proizvoda,

manje grešaka u klasifikaciji,

bolje korisničko iskustvo prilikom pretrage i filtriranja proizvoda.

⚙️ Tehnički detalji

Model je razvijen u Python-u korišćenjem sledećih tehnologija:

pandas, scikit-learn, numpy, joblib, matplotlib

TF-IDF vektorizacija teksta

Logistic Regression kao osnovni klasifikacioni algoritam

📊 Rezultati

Model postiže visoku tačnost na test podacima (≈ 90%) i uspešno prepoznaje većinu kategorija na osnovu naslova.
Posebno dobro funkcioniše za jasno definisane kategorije (npr. telefoni, kamere, mikrotalasne), dok greške uglavnom nastaju kod sličnih klasa (npr. Fridge vs Fridge Freezer).

📁 Struktura projekta
product_classifier_project/
├── model.pkl                         # trenirani model (TF-IDF + LogisticRegression)
├── train_model.py                     # skript za treniranje i čuvanje modela
├── predict_category.py                # interaktivni skript za testiranje
├── product_classification_notebook.ipynb  # analiza i treniranje
├── products.csv                       # skup podataka
├── requirements.txt                   # zavisnosti
└── README.md                          # dokumentacija projekta

▶️ Pokretanje

Instaliraj zavisnosti:

pip install -r requirements.txt


Pokreni interaktivni test modela:

python predict_category.py --model model.pkl


Unesi naziv proizvoda (npr. iPhone 7 32GB Gold) i model će prikazati predloženu kategoriju.

🔮 Dalji razvoj

Dodavanje naprednijih NLP modela (BERT, DistilBERT)

Analiza grešaka i balansiranje kategorija

Razvijanje API servisa (FastAPI/Flask) za integraciju u web aplikaciju

Implementacija web interfejsa za testiranje modela

👨‍💻 Autor

Projekat kreiran kao deo praktičnog zadatka iz mašinskog učenja.
Struktura i dokumentacija su organizovane u skladu sa principima timskog rada i spremne za dalji razvoj i nadogradnju.
