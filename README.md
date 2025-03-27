# Hex Game Upgrade

## 📌 Inhoud
- [**Over**](#Over)
- [**Doelstellingen**](#Doelstellingen)
   - [**Data opslaan**](#Data_oplsaan)
   - [**Implementeren van AI**](#Implementeren-van-ai)
   - [**AI vs AI**](#AI-vs-AI)
- [**Installatie**](#Installatie)
- [**Algoritme**](#Algoritme)
- [**Trainen**](#Trainen)
- [**Gebruik**](#Gebruik)
- [**Conclusie**](#Conclusie)

## Over
In dit project gaan we machine learning AI toevoegen aan ons vorig project [HEX_AI_GAME](https://github.com/BramDe/HEX_AI_GAME). Hiervoor maken we een adaptie van de AlphaGo AI. De AI zal leren van gespeelde games en hieruit de beste openingszetten en vervolgzetten berekenen door gewichten toe te kennen aan mogelijke zetten.

## Doelstellingen

1. **Data opslaan**  
   We implementeren een systeem om data van gespeelde games op te slaan. Deze data zal gebruikt worden om de AI te trainen en strategieën te optimaliseren.

2. **Implementeren van AI**  
   We voegen een algoritme toe dat de spelregels correct uitvoert en zetten maakt die binnen de regels passen.

3. **AI vs AI**  
   De AI zal in staat zijn tegen zichzelf te spelen om snellere en betere leermethoden te ontwikkelen.

4. **Trainen**  
   De AI wordt getraind met data van eerdere games. Het leerdoel is dat de AI op termijn een menselijke speler consistent kan verslaan.

## Installatie
1. **Clone de repository**:
   ```sh
   git clone https://github.com/jouw-gebruikersnaam/hex-ai-game.git
   ```
2. **Installeer Pipenv om afhankelijkheden te beheren**:
   ```sh
   pip install pipenv
   ```
3. **Installeer afhankelijkheden** (gebruik `--skip-lock` vanwege een recente regressie in Pipenv):
   ```sh
   pipenv install -r requirements.txt --skip-lock
   ```
4. **Activeer de virtuele omgeving**:
   ```sh
   pipenv shell
   ```
5. **Start het spel**:
   ```sh
   python main.py
   ```
   
## Algoritme
De AI is gebaseerd op een aangepaste versie van AlphaGo, specifiek herschreven voor het Hex-spel. Dit omvat:
- Monte Carlo Tree Search (MCTS) om de meest veelbelovende zetten te evalueren.
- Een neuraal netwerk dat getraind wordt met opgeslagen speldata om strategieën te verbeteren.
- Zelfspelende simulaties waarbij de AI zijn eigen zetten analyseert en optimaliseert.
- Een leerproces waarbij de AI als doel heeft om op termijn menselijke spelers te verslaan.

## Trainen
We kunnen onze AI trainen door deze games tegen zichzelf te laten spelen. We kunnen per model dat we maken kiezen hoeveel games er gepseeld worden, hoeveel keer de AI deze games bekijkt (als dit te veel is word de AI verzadigd, als deze te weinig is heeft de AI te weinig informatie.) We kunnen kiezen hoeveel data models de AI aanmaakt per run.
  
## Gebruik
- Start het spel en speel tegen de AI.
- Laat de AI tegen zichzelf spelen voor training.
- Analyseer opgeslagen speldata om patronen te ontdekken.

## Conclusie
Dit project combineert kunstmatige intelligentie en strategische gameplay om een AI te ontwikkelen die zelfstandig leert en zich aanpast. Door gebruik te maken van een aangepaste versie van AlphaGo voor Hex, creëert de AI een dynamische en steeds verbeterende strategie. Met voortdurende training en optimalisatie zal de AI uiteindelijk een niveau bereiken waarop het menselijke spelers kan verslaan. Dit project biedt niet alleen een uitdagend spel, maar ook een leerzame ervaring op het gebied van machine learning en AI-ontwikkeling.





