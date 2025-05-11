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