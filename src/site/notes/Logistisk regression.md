---
{"dg-publish":true,"permalink":"/Logistisk regression/"}
---

# Logistisk regression
[[SPSS Logistisk regression\|SPSS Logistisk regression]]

Logistisk regression benyttes som Chi2 testen til at analysere en binær afhængig variabel, men er ikke begrænset til kun én kategorisk uafhængig variabel (mere generelt analyseværktøj). 

![Pasted image 20241024162910.png](/img/user/attachments/Pasted%20image%2020241024162910.png)

## Sandsynlighed (p) odds og odds ratio (OR)
**Sandsynlighed** er et mål for tilbøjeligheden hvormed en bestemt hændelse indtræffer.

**Odds** er ligesom sandsynlighed er mål for tilbøjeligheden hvormed en bestemt hændelse indtræffer.

Odds for at en hændelse indtræffer (Succes, S) er defineret som forholdet imellem sandsynligheden for at hændelsen indtræffer (Succes) og sandsynligheden for at hændelsen ikke indtræffer (Fiasko)

**Excel-arket kan hjælpe dig med at omregne mellem odds, OR og sandsynlighed og med at lave specifikke prædiktioner ud fra din model.**

$$odds(S)=\frac{p(Succes)}{p(Fiasko)}=\frac{p(S)}{1-p(S)}$$
$$odds(Fiasko)=\frac{1}{odds(Succes)}$$
$$OR=\frac{odds(2)}{odds(1)}$$
$$OR(Fiasko)=\frac{1}{OR(Succes)}$$
$$odds(1)=\frac{odds(2)}{OR}$$
$$odds(2)=odds(1)\cdot OR$$
$$p(S)=\frac{odds(S)}{1+odds(S)}$$

## Regressionsmodellen
$$\hat{\mathrm{odds}}(Y=1)=\mathrm{odds}_0\cdot\mathrm{OR}_1^{X_1}\cdot\mathrm{OR}_2^{X_2}\cdot...\cdot\mathrm{OR}_n^{X_n}$$
$$\hat{P}(Y=1)=\frac{\exp(b_0+b_1X_1+b_2X_2+\cdots+b_nX_n)}{1+\exp(b_0+b_1X_1+b_2X_2+\cdots+b_nX_n)}$$

**Konklusion:**
> En logistiske regression viste at bilister med høj social status var mere tilbøjelige til ikke at hold tilbage for fodgængere, OR = 1.472, p = .040, når der blev korrigeret for bilisternes estimerede køn, OR = 0.960, p = .906, og alder, OR = 0.852, p = .309. 
> Dette giver evidens for at konkludere at personer med høj social status er mere tilbøjelige til at udvise uetisk opførsel.

**Alternativ konklusion:**
> En logistisk regression viste at sandsynligheden for tegn på demens (MMSE score < 24) stiger med alderen, OR = 1.686, 95% CI = 1.052-2.702, p = .03.