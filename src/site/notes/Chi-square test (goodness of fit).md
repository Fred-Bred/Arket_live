---
{"dg-publish":true,"permalink":"/Chi-square test (goodness of fit)/"}
---

# Chi-square test
[[SPSS Chi-square\|SPSS Chi-square]]
[[SPSS Fisher's exact test\|SPSS Fisher's exact test]]

Forskningsspørgsmål:
> Er fordelingen af venstrehåndede for drenge og piger forskellig?

H0: Fordelingen af venstehåndede drenge og piger er ens.
$H_0:π_\text{{drenge.venstre}}=π_{\text{piger.venstre}}$

H1: Fordelingen af venstrehåndede drenge og piger er forskellig.

![Pasted image 20241023125712.png](/img/user/attachments/Pasted%20image%2020241023125712.png)

![Pasted image 20241023125719.png](/img/user/attachments/Pasted%20image%2020241023125719.png)

![Pasted image 20241023125737.png](/img/user/attachments/Pasted%20image%2020241023125737.png)

Konklusion:
> En χ2 test af to uafhængige proportioner (two-tailed, α=5%) viste at andelen af venstrehåndede drenge (40 ud af 400, 10%) var signifikant højere end andelen af venstrehåndede piger (42 ud af 709, 6%), χ2 (1)=6.17,  p< .05.

$H_1:π_\text{{drenge.venstre}} \neq π_{\text{piger.venstre}}$

$Z^2$ test: $Z^2 = \frac{(X - \mu)^2}{\sigma}$

Chi-square test: $$\chi^2=\sum\frac{(O-E)^2}E=\frac{\left(O_{R_1C_1}-E_{R_1C_1}\right)^2}{E_{R_1C_1}}+\frac{\left(O_{R_1C_2}-E_{R_1C_2}\right)^2}{E_{R_1C_2}}+\frac{\left(O_{R_2C_1}-E_{R_2C_1}\right)^2}{E_{R_2C_1}}+\frac{\left(O_{R_2C_2}-E_{R_2C_2}\right)^2}{E_{R_2C_2}}$$

O = Observed
E = Expected

**Slå $\chi^2$-værdien op i tabel E.1 og sammenlign med den kritiske værdi.**

Varians: $\sigma^2 = N \pi (1-\pi)$
$$\mu=N\pi$$
$\text{df} = (R-1)(C-1)$
R = antal rækker i tabellen
C = antal kolonner i tabellen

Forventede antal for den i'te række og j'te kolonne: $$E_{ij} = R_i \frac{C_j}{N}$$
![Pasted image 20241023130321.png](/img/user/attachments/Pasted%20image%2020241023130321.png)

## Fisher's exact test
[[SPSS Fisher's exact test\|SPSS Fisher's exact test]]
Hvis én eller flere af de forventede værdier er *mindre end 5* benyttes Fisher's exact test.
![Pasted image 20241023130645.png](/img/user/attachments/Pasted%20image%2020241023130645.png)

$$p=\frac{(6+b)!(c+d)!(6+c)!(b+d)!}{(a+b+c+d)!a!b!c!d!}$$

Sandsynligheden for at sample a venstrehåndede drenge ud af (a+b) drenge, når antallet af venstre- og højre-håndede i alt er hhv. (a+c) og (b+d)

## Goodness-of-fit
![Pasted image 20241023130613.png](/img/user/attachments/Pasted%20image%2020241023130613.png)
![Pasted image 20241023130629.png](/img/user/attachments/Pasted%20image%2020241023130629.png)