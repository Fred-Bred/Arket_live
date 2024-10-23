---
{"dg-publish":true,"permalink":"/Faktoranalyse/"}
---

# Faktoranalyse

## Formålet med faktoranalyse
- At forklare et bagvedliggende mønster blandt et sæt af korrelationer, typiskt mellem et stort antal forskellige tests eller spørgsmål i et spørgeskema.
- Input til en faktoranalyse er en korrelationsmatrise mellem tests (eller spørgsmål), der allesammen korrelerer mere eller mindre indbyrdes.
- Output fra en faktoranalyse er et mindre antal af faktorer, som ikke korrelerer indbyrdes.
- Den psykologiske fortolkning af faktorerne afgøres ude fra hvilke tests (eller spørgsmål), der bidrager til hver faktor.

## Eigenværdier og % forklaret varians
**Eigenværdi:** hvor meget faktoren forklarer af den totale variansen for alle observerede variable.

$\text{Eigenværdi}_{faktor1}=r_{faktor1,variabel1}^2+r_{faktor1,variabel2}^2$

**%VariansFaktorX**: Hvor meget en faktor forklarer af varians i gennemsnit, for hver af variablerne.
Var tallet 0,828, ville den underliggende faktor i gennemsnit forklare 82,8% af variansen i hver af variablerne

$\text{\%varians}_{faktor1}=\frac{r_faktor1^2+r_faktor2^2}{2}$

**Eksempel for eigenværdier med 4 faktorer:**
![Pasted image 20241023122111.png](/img/user/attachments/Pasted%20image%2020241023122111.png)

*Note:* faktor 3 og 4 er sorteret fra under *Extraction* fordi deres eigenværdi er under 1.

## SPSS
![Pasted image 20241023122200.png](/img/user/attachments/Pasted%20image%2020241023122200.png)
**Kaisers kriterium:** En ofte brugt regel (Kaisers kriterium) er, at man kun beskæftiger sig med faktorer, der har en eigenværdi over den gennemsnitlige værdi for eigenværdier.
Dvs. faktorer, der har en eigenværdi over 1 (SPSS standard)

I nogle opgaver kan du i stedet blive bedt om at finde i forhold til et fastsat antal faktorer. Det kan du vælge i SPSS ved at markere Fixed number of factors i stedet.

![Pasted image 20241023122252.png](/img/user/attachments/Pasted%20image%2020241023122252.png)![Pasted image 20241023122318.png](/img/user/attachments/Pasted%20image%2020241023122318.png)
**Faktorvægt:** Hvor meget en variabel vægter i en specifik faktor (aflæses i komponent matricen)

**Eigenværdierne:** Angiver hvor meget hver faktor forklarer af den totale varians for alle observerede variable.
$$\text{Eigenværdi}_{\text{Fak}1}=r_{\text{fak}1,\text{ord}}^2+r_{\text{fak}1,\text{inf}}^2+r_{\text{fak}1,\text{blok}}^2+r_{\text{fak}1,\text{mat}}^2=0.806^2+0.715^2+(-0.593)^2+(-0.524)^2=1.78$$
$$\text{Eigenværdi}_{\text{Fak}2}=r_{\text{fak}2,\text{ord}}^2+r_{\text{fak}2,\text{inf}}^2+r_{\text{fak}2,\text{blok}}^2+r_{\text{fak}2,\text{mat}}^2=0.430^2+0.570^2+0.652^2+0.702^2=1.428$$

$$\begin{aligned}&\%\mathrm{varians}_{\mathbf{fak}1}=\frac{\mathrm{Eigenværdi}_{\mathbf{fak}1}}{4}=\frac{1.780}{4}=0.44 (44\%)\\&\%\mathrm{varians}_{\mathbf{fak}2}=\frac{\mathrm{Eigenværdi}_{\mathbf{fak}2}}{4}=\frac{1.427}{4}=0.36 (36\%)\\&\%\mathrm{varians}_{\mathbf{fak}1+\mathbf{fak}2}=0.44+0.36=0.80 (80\%)\end{aligned}$$

![Pasted image 20241023122340.png](/img/user/attachments/Pasted%20image%2020241023122340.png)

**Kommunaliteterne (communalities):** Angiver hvor meget de udtrykne faktorer tilsammen forklarer af variansen for hver af de observerede variable.

$$\text{Kommunalitet}_{\text{ordforråd}}=r_{\text{faktor}1,\text{ordforråd}}^2+r_{\text{faktor}2,\text{ordforråd}}^2=0.806^2+0.430^2=0.834\mathrm{~(83.4\%)}$$
$$\text{Kommunalitet}_{\text{information}}=r_{\text{faktor}1,\text{information}}^2+r_{\text{faktor}2,\text{information}}^2=0.715^2+0.570^2=0.836\left(83.6\%\right)$$
$$\text{Kommunalitet}_{\text{blokmønstre}}=r_{\text{faktor}1,\text{blokmønstre}}^2+r_{\text{faktor}2,\text{blokmønstre}}^2=(-0.593)^2+0.652^2=0.776\mathrm{~(77.6\%)}$$
$$\text{Kommunalitet}_{\text{matriser}}=r_{\text{faktor}1,\text{matriser}}^2+r_{\text{faktor}2,\text{matriser}}^2=(-0.524)^2+0.702^2=0.767(76.7\%)$$
## Scree plot
Scree-plottet er en grafisk repræsentation af faktorernes eigenværdier, der kan tydeliggøre, hvor mange faktorer der skal medtages.

![Pasted image 20241023122926.png](/img/user/attachments/Pasted%20image%2020241023122926.png)

## Rotation
For at opnå højere korrelationer med faktorerne, er det nyttigt at benytte sig af rotation.

![Pasted image 20241023124858.png](/img/user/attachments/Pasted%20image%2020241023124858.png)![Pasted image 20241023124901.png](/img/user/attachments/Pasted%20image%2020241023124901.png)
![Pasted image 20241023124907.png](/img/user/attachments/Pasted%20image%2020241023124907.png)

Det ses af komponentmatricen at faktorernes vægtning er øget med rotationen.

![Pasted image 20241023124924.png](/img/user/attachments/Pasted%20image%2020241023124924.png)![Pasted image 20241023124931.png](/img/user/attachments/Pasted%20image%2020241023124931.png)

![Pasted image 20241023124942.png](/img/user/attachments/Pasted%20image%2020241023124942.png)

Det ses at den kummulative forklaringsgrad i den roterede og ikke-roterede vægtning er den samme, men at fordelingen er forskellig.

Foretages der en rotation, rapporteres der altid for de roterede værdier.

I datasæt med mange variabler, kan det være fordelagtigt at *suppress* små koefficienter for at danne overblik:
![Pasted image 20241023125016.png](/img/user/attachments/Pasted%20image%2020241023125016.png)![Pasted image 20241023125020.png](/img/user/attachments/Pasted%20image%2020241023125020.png)

Her ses et eksempel hvor "støjen" er fjernet fra tabellen
![Pasted image 20241023125032.png](/img/user/attachments/Pasted%20image%2020241023125032.png)