# 🧠 Supervised Machine Learning – Kundanalys för marknadsföringskampanj

Detta projekt syftar till att förutsäga om en kund svarar på en marknadsföringskampanj, baserat på deras köpbeteende och demografiska data. Det är en fortsättning på en tidigare unsupervised klusteranalys (beskrivs efter Supervised ML), men här används supervised machine learning för att bygga och utvärdera prediktiva modeller.

## 🎯 Syfte

- Identifiera vilka variabler som påverkar kampanjrespons (`Response`)
- Bygga modeller som kan förutsäga vilka kunder som kommer att svara
- Utforska affärsnyttan av segmentering och prediktion

---
## 📁 Projektinnehåll

```bash
.
├── Supervised_EDA_and_Hypotheses.ipynb   # Notebook med hypoteser, EDA, feature engineering och uppdelning
├── X_train.csv                           # Features – träningsdata
├── X_test.csv                            # Features – testdata
├── y_train.csv                           # Målvariabel – träningsdata
├── y_test.csv                            # Målvariabel – testdata
├── .gitignore                            # Filer att ignorera i versionshantering
└── README.md                             # Projektbeskrivning

🔬 Hypoteser
Vi testade flera affärsdrivna hypoteser, t.ex:

Högre vin- och köttkonsumtion → större chans att svara

Färska kunder (lägre Recency) → mer benägna att svara

Fler webbköp → mer engagerade

Hög inkomst eller många barn → ev. lägre svarsfrekvens


## Visualiseringar (EDA) gjordes med boxplots och analyserades variabel för variabel.


Feature engineering och variabelval

Hypotesformulering

Exploratory Data Analysis (EDA)

Uppdelning i tränings- och testdata

Export av .csv-filer

Modellträning (Logistisk Regression, KNN m.fl.)

Utvärdering (accuracy, precision, recall, confusion matrix)

Modelloptimering

Tolkning av resultat och slutsats

🛠️ Användning
Klona repot eller ladda ner som zip

Öppna Supervised_EDA_and_Hypotheses.ipynb i Jupyter eller VS Code

Kör cellerna om du vill återskapa .csv-filerna (eller använd de färdiga)

Öppna nästa notebook för modellträning

Kör modeller och utvärdera resultat

📦 Krav
Python 3.x

Jupyter Notebook

Bibliotek: pandas, matplotlib, seaborn, scikit-learn

-----S

# Marketingcampaign
# 🧠 Kundsegmentering med Unsupervised Learning

Detta projekt analyserar ett marknadsföringsdataset med hjälp av unsupervised machine learning-tekniker som **PCA**, **KMeans** och **DBSCAN** för att identifiera kundsegment och affärsinsikter.

## 📁 Dataset
Datasetet kommer från Kaggle:
[Customer Personality Analysis](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)

Det innehåller information om kunders:
- Demografi (ålder, inkomst, barn etc.)
- Köpvanor
- Respons på kampanjer

## 🔧 Använda tekniker
- 📊 Exploratory Data Analysis (EDA)
- 📉 Principal Component Analysis (PCA)
- 📍 KMeans-klustring
- 🔎 DBSCAN-klustring
- 📐 Silhouette Score för klusterkvalitet
- 📈 Visualiseringar med Matplotlib och Seaborn

## 📌 Resultat
Projektet identifierade tre huvudsakliga kundkluster med olika köpmönster och affärspotential. DBSCAN användes för att upptäcka outliers.

**Topp 3 affärsinsikter:**
1. Premiumkunder (Kluster 1): hög inkomst och stark kampanjrespons.
2. Familjekunder (Kluster 0): låg köpkraft och svag respons – kräver annan strategi.
3. DBSCAN-outliers: potentiella VIP:er med avvikande beteende.

## 🖥️ Kör projektet lokalt

1. Klona repot:
```bash
git clone https://github.com/ditt-användarnamn/unsupervised-marketing-clustering.git
cd unsupervised-marketing-clustering
