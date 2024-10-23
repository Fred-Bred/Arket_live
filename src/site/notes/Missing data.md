---
{"dg-publish":true,"permalink":"/Missing data/"}
---

# Missing data
Der er overordnet tre måder data kan mangle på:
- Missing completely at random (MCAR)
- Missing at random (MAR)
- Missing not at random (MNAR)

Det bedste vi kan gøre er at undgå missing data ved at lave et forskningsdesign, der minimerer risikoen: varighed, målevariabler, ulejlighed for deltagere osv.

Hvis der alligevel er missing data kan vi bruge imputation:
- Metoder fra pensum
	- Best case scenario
	- Worst case scenario
	- Mixed case scenario
- Metoder der ikke er på pensum
	- Last observation carried forward
	- Baseline observation carried forward
	- Mean imputation
	- Jump to reference

## Missing Comletely At Random (MCAR)
- Mangel er uafhængig af både observerede variable og uobserverede parametre, dvs. den er fuldkommen tilfældig.
- Svarer omtrent til, at ”hunden har spist 20 % af data”
- Kræver gode argumenter, fx at patienten er flyttet					

Det kræver meget gode argumenter, for at man kan påråbe MCAR. Det er sjældent at vi kan gøre det.					

*Hvis data er MCAR, kan vi forsvare at ignorere det og lave en complete case analyse	*

*Overvej dog hvad der sker med konfidensintervallet, hvis vi ignorerer missing data. Når N bliver mindre, bliver konfidensintervallet bredere. Mindre N betyder mindre power.*

# Missing At Random (MAR)
Mangel er forbundet med observerede variabler

*Vi har en formodning om hvad der er på spil. Manglen er afhængig af en variabel vi har målt på (eksempelvis selvmordstanker)*

*Hvis vi ignorerer, at der mangler data, og laver en complete analysis, bliver resultatet biased.*

*Da vi kender variablen som manglen relaterer sig til, kan vi "gætte" os til hvad den manglende data ville have været. Altså en data driven imputation*

**Eksempel:**
![Pasted image 20241023101527.png](/img/user/attachments/Pasted%20image%2020241023101527.png)
- Mangel er forbundet med observerede variabler (her Selvmordstanker)
- Data driven imputation: hvis en patient har udtrykt selvmordstanker, er der nok ikke sket en reduktion i HAMD
- Denne tilgang eliminerer ikke bias, men gør i det mindste, at vi ikke overestimerer behandlingseffekten

*Vi fjerner ikke bias. Men i det mindste kommer vi ikke til at sige den nye behandling er bedre end den gamle*

## Missing Not At Random (MNAR)
Mangel er forbundet med variabler, som vi ikke har målt eller ukendte parametre.

Dette scenario er det mest hyppige og det mest vanskelige!

*Vi har en idé om at det hænger sammen med selvmord, men vi har ikke målt på det.	*

**Eksempel:**
![Pasted image 20241023101815.png](/img/user/attachments/Pasted%20image%2020241023101815.png)

# Hvad kan vi gøre ved missing data?
## Best case scenario
*Alle manglende datapunkter er successer*

**Grundlæggende antagelse:**				
Patienterne er droppe ud, fordi de føler sig helbredt

**Hvornår er dette for optimistisk?**				
Hvis missing data overvejende er i interventionsgruppen?

**Eksempel:**
![Pasted image 20241023101953.png](/img/user/attachments/Pasted%20image%2020241023101953.png)

*Når alle missing er i gruppen med den nye behandling, er det meget problematisk hvis vi bare laver dem til succeser. Så kommer vi til at overestimere effekten*
![Pasted image 20241023102008.png](/img/user/attachments/Pasted%20image%2020241023102008.png)

## Worst case scenario
*Alle manglende datapunkter er failures*

**Grundlæggende antagelse:**
Patienterne er droppe ud, fordi de ikke føler behandlingen virker			

**Hvornår er dette for optimistisk?**
Hvis missing data overvejende er i kontrolgruppen			

**Eksempel:**
![Pasted image 20241023102146.png](/img/user/attachments/Pasted%20image%2020241023102146.png)

*Hvis missing data er i kontrolgruppen, altså den gamle behandlingsform, får det også den nye behandling til at se bedre ud end den måske er.*
![Pasted image 20241023102311.png](/img/user/attachments/Pasted%20image%2020241023102311.png)
## Mixed case scenario
*Alle manglende datapunkter i interventionsgruppen er failures*
*Alle manglende datapunkter i kontrolgruppen er succeser*

**Grundlæggende antagelse:**
Patienterne i interventionsgruppen er droppet ud, fordi de ikke føler, behandlingen virker
Patienterne i kontrolgruppen er droppet ud, fordi de føler sig helbredt				

*Dette er den mest konservative tilgang*

**Eksempel:**
![Pasted image 20241023102455.png](/img/user/attachments/Pasted%20image%2020241023102455.png)

*Det mindst gode scenarie, og det er nok ikke realistisk. Men det er det mest konservative scenarie. Risikoen for at man siger den nye er bedre, uden at være det, er mindst mulig.*

![Pasted image 20241023102205.png](/img/user/attachments/Pasted%20image%2020241023102205.png)

*Hvis de to grupper ligger langt fra hinanden, vil man trække data tættere på hinanden*

![Pasted image 20241023102230.png](/img/user/attachments/Pasted%20image%2020241023102230.png)
*Hvis de to grupper ligger tæt på hinanden, vil mixed case hive dem væk fra hinanden. (Den nye bliver dårligere og den gamle bliver bedre)*

## Last Observation Carried Forward - Baseline Observation Carried Forward
*Manglende data imputes vha. tidligere observationer*

**Grundlæggende antagelse:**				
- Der sker ingen ændring over tid (vi antager, at H0 er sand)

Giver skævvridning af data når:
- Vi forventer spontan forbedring (fx ved depression)
- Vi forventer spontan forværring (fx ved demens)

**Eksempel:**
![Pasted image 20241023102632.png](/img/user/attachments/Pasted%20image%2020241023102632.png)
*Patient 2: Vi mangler en followup, derfor tager vi den sidst målte data og trækker med ned. (det betyder vi antager at H0 er sand, fordi vi siger der ikke er en forskel)*

*Patient 3: Her mangler vi både post-treatment og followup. Her antager vi virkelig at der ikke er nogen forskel.*

## Mean imputation
*Alle manglende datapunkter imputes med den respektive gruppes mean*

**Grundlæggende antagelse:**				
- Patienterne, der er droppet ud, er ligesom de resterende patienter (altså MCAR)

Giver bias ved:
- Ved MAR og MNAR (Altså, der er en grund til, at der mangler data

**Eksempel:**
![Pasted image 20241023102801.png](/img/user/attachments/Pasted%20image%2020241023102801.png)

*Overvej hvad der sker med konfidensintervallet:
Variansen ændrer sig. Hvis vi putter data ind som ligger på mean, varierer data mindre. Dermed indsnævrer vi konfidensintervallet. På den måde er der større risiko for at man forkaster H0.*

## Jump to reference
*Alle manglende datapunkter imputes med kontrolgruppens mean*

**Grundlæggende antagelse:**
- Patienterne, der er droppet ud, klarer sig i hvert fald ikke bedre end kontrolgruppen

I hvilke tilfælde er dette for optimistisk ?				
- Hvis den nye behandling er skadelig, $π_{Ny} < π_{Kontrol}$

**Eksempel:**
![Pasted image 20241023102951.png](/img/user/attachments/Pasted%20image%2020241023102951.png)

*Hvis den nye behandling er dårligere end kontrolgruppen, og man blot indfører kontrolgruppens mean, trækker man behandlingens mean ind mod kontrolgruppen. Det øger risikoen for at man laver en Type I fejl (man forkaster H0 selvom H1 ikke er bedre)*