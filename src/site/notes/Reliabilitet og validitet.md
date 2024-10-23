---
{"dg-publish":true,"permalink":"/Reliabilitet og validitet/"}
---

# Reliabilitet og validitet
![Pasted image 20241023085515.png](/img/user/attachments/Pasted%20image%2020241023085515.png)

## Recode into same variables
Nogle spørgeskemaer indeholder spørgsmål med modsatrettet kodning.
For at lave en samlet scorer (skalascorer), skal alle spørgsmål dog ”pege” i den samme retning.
![Pasted image 20241023085550.png](/img/user/attachments/Pasted%20image%2020241023085550.png)
![Pasted image 20241023085629.png](/img/user/attachments/Pasted%20image%2020241023085629.png)

For at regne en total score, selvom nogle spørgsmål har været modsatrettet kodet regnes til sidst en totaltscore:

## Compute variable
![Pasted image 20241023085721.png](/img/user/attachments/Pasted%20image%2020241023085721.png)![Pasted image 20241023085734.png](/img/user/attachments/Pasted%20image%2020241023085734.png)

## Reliabilitetstest: test-retest (gold standard)
Reliabilitet estimeres ved at gentage testen på de samme personer.
Reliabiliteten af testen er da givet som korrelationen (r) mellem skalascorerne for 1. og 2. test. 

Se [[Korrelation\|Korrelation]] og [[SPSS Pearson korrelation\|SPSS Pearson korrelation]]

![Pasted image 20241023085834.png](/img/user/attachments/Pasted%20image%2020241023085834.png)

## Reliabilitetstest: split-half
Anvendes når det ikke er muligt at gennemføre en test-retest. 
Grundprincip: Spørgeskemaet inddeles i to lige store grupper (som antages at måle på det samme). Herefter testes disse mod hinanden.

![Pasted image 20241023085909.png](/img/user/attachments/Pasted%20image%2020241023085909.png)![Pasted image 20241023085914.png](/img/user/attachments/Pasted%20image%2020241023085914.png)![Pasted image 20241023085950.png](/img/user/attachments/Pasted%20image%2020241023085950.png)
Korrelation mellem 1. og 2. halvdel: $r=0,752$

Spearman-Brown-korrektion: $\text{Split-half reliabilitet} = 0,859$

## Cronbachs alpha
Cronbach’s alpha (α) er gennemsnittet af alle mulige split-half reliabiliteter (dog benyttes en anden korrektion end spearman-brown).

$$\hat{\alpha}=\frac{k}{k-1}\cdot\left(1-\frac{\sum_{i=1}^{k}s_{i}^{2}}{s_{t}^{2}}\right)$$
$k$ = antal spørgsmål (items).

$s_i^2$ = std. afv. af scorerne for spørgsmål i.

$s_t^2$ = std. afv. af de totale (skala-) scorer.

![Pasted image 20241023090400.png](/img/user/attachments/Pasted%20image%2020241023090400.png)![Pasted image 20241023090405.png](/img/user/attachments/Pasted%20image%2020241023090405.png)

## Konfidensinterval for individuelle skalascorer
95% konfidensintervallet omkring den observerede skalascorer (X) angiver, indenfor hvilket interval vi med 95% sikkerhed kan forvente, at den faktiske skalascorer (T) befinder sig:
$$\text{CI}_{.95}=X±z_{.025} \times \text{SEM}$$

$$\text{SEM} = \text{SD} \times \sqrt{1- \text{Reliabilitet}}$$

SEM = Standard error of measurement
SD = Standardafvigelsen af skalacoren
Reliabilitet = Cronbachs alpha (eller anden måde)

## Validitet
**Kriterievaliditet** (Criterion-related validity):
- I hvilken grad scorerne for en test korrelerer med et kriterium, der er afgørende for brugen af testen som korrekt måleinstrument af et fænomen.
- F.eks., måler udslaget (scoren) på en løgnedetektor (GSR) faktisk om en person lyver (kriteriet)?
- En ny test valideres ofte op imod en eksisterende test, hvor det antages at den eksisterende test er ”golden standard”.
- Kriterievaliditet betragtes ofte som det klassiske validitetsbegreb.

**Indholdsvaliditet** (Content-related validity)
I hvilken grad en test måler alle aspekter af det fænomen, den har til hensigt at måle.
F.eks., kommer en eksamen ud i alle relevante dele af pensum?

**Konstruktvaliditet** (Construct-related validity)
I hvilken grad en test måler det teoretiske konstrukt, det har til hensigt at måle.
F.eks., er WAIS (IQ-testen) et validt mål for intelligens (teoretisk konstrukt)?