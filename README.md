Markdown


Kopiera
# Hälsostudie – Del 2: Fördjupning och pipeline

## Beskrivning
I denna del bygger jag vidare på Del 1 genom att strukturera koden med funktioner och en klass **HealthAnalyzer**.  
Syftet är att göra analyserna mer organiserade, återanvändbara och att utöka med mer avancerade metoder.

## Steg i analysen
- Skapar en klass `HealthAnalyzer` som samlar alla analyser på ett ställe.  
- Implementerar metoder för:
  - **Beskrivande statistik** (medel, median, min, max).  
  - **Regressioner**:  
    - Enkel regression (ålder → blodtryck).  
    - Multipel regression (ålder + vikt → blodtryck).  
  - **PCA (Principal Component Analysis)** för att reducera komplexiteten och hitta mönster.  
  - **Visualiseringar**:  
    - BMI ↔ kolesterol (scatterplot).  
    - Heatmap över korrelationer.  
    - Stapeldiagram över medelblodtryck per kön.  

## Resultat
- **Regressioner:**  
  - Enkel regression visar att ålder har en positiv effekt på blodtrycket (R² ≈ 0.37).  
  - Multipel regression visar att både ålder och vikt bidrar positivt (R² ≈ 0.41).  

- **PCA:**  
  - PC1 ≈ 0.37 → första komponenten förklarar ca 37 % av variationen.  
  - PC2 ≈ 0.27 → andra komponenten förklarar ca 27 %.  
  - Tillsammans ≈ 64 % → två komponenter räcker för att behålla det mesta av informationen.  

- **Visualiseringar:**  
  - BMI ↔ kolesterol visar ett tydligt positivt samband.  
  - Heatmapen visar stark korrelation mellan vikt och BMI.  
  - Stapeldiagrammet visar att män och kvinnor har nästan samma medelblodtryck.  

## Målet
Visa att jag kan bygga en mer avancerad analys med hjälp av funktioner och klasser.  
Kombinationen av regressioner, PCA och visualiseringar ger en tydlig helhetsbild av hur olika faktorer hänger ihop med blodtryck och kolesterol.