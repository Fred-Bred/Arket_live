---
{"dg-publish":true,"permalink":"/Uparret t-test/"}
---

# Independent samples t-test
[[SPSS Independent samples t-test\|SPSS Independent samples t-test]]

Independent samples t test bliver brugt til at sammenligne målinger (scorer) efter behandling/terapi (a.k.a., end of treatment, post-treatment) for to grupper med forskellige patienter.

**Forskningsspørgsmål:**
> Hvad er sandsynligheden for at trække to samples med en forskel i middelværdi på X ̅Ctr-X ̅Lid eller med en mere ekstrem forskel under antagelse af nulhypotesen (μCtr-μLid=0)?

**Konklusion:**
> En independent samples t test (two-tailed, α=.05) viste at efter 9 måneders behandling var procentdelen af stavelser, hvor der stammes, signifikant mindre for de børn, der havde fuldt Lidcombe programmet, X ̅Lid=1.5 (SD=1.4), sammenlignet med børn, der havde modtaget standard-behandlingen, X ̅Ctr=3.9 (SD=3.5), t(45)=3.13, p=.003, d=0.96. Forskellen på middelværdierne i de to grupper var på 2.3% med et 95% konfidensinterval på 0.8 til 3.9.

==OBS:== Homogenitet eller heterogenitet af varianser?

**Homogenitet af varians:** $\sigma_1^2 = \sigma_2^2$
Hvis variansen i den ene gruppe $S_1^2$ **ikke** er mere end 4 gange større end variansen i den anden gruppe  $S_2^2$.
$S_1^2$ og $S_2^2$ er så ens at vi kan benytte $S_P^2$ ("pooled" varians). Da udregnes t-score som:
$$t=\frac{(\bar{X}_{Ctr}-\bar{X}_{Treat})-(\mu_{Ctr}-\mu_{Treat})}{\sqrt{\frac{S_p^2}{n_{Ctr}}+\frac{S_p^2}{n_{Treat}}}}=\frac{(\bar{X}_{Ctr}-\bar{X}_{Treat})-(\mu_{Ctr}-\mu_{Treat})}{\sqrt{S_p^2\cdot(\frac1{n_{Ctr}}+\frac1{n_{Treat}})}}$$

**Heterogenitet af varians:** $\sigma_1^2 \neq \sigma_2^2$
Hvis variansen i den ene gruppe $S_1^2$ er mere end 4 gange større end variansen i den anden gruppe $S_2^2$
$S_1^2$ og $S_2^2$ er så forskellige at vi ikke kan benytte $S_P^2$ ("pooled" varians"). I så fald udregnes t-scoren som:
 $$t=\frac{(\bar{X}_{Ctr}-\bar{X}_{Treat})-(\mu_{Ctr}-\mu_{Treat})}{S_{\bar{X}_{Ctr}-\bar{X}_{Treat}}}=\frac{(\bar{X}_{Ctr}-\bar{X}_{Treat})-(\mu_{Ctr}-\mu_{Treat})}{\sqrt{\frac{S_{Ctr}^{2}}{n_{Ctr}}+\frac{S_{Treat}^{2}}{n_{Treat}}}}$$

**Den kritiske værdi aflæses i tabel E.6 nedenfor**
### Andre formler
Degrees of freedom: $df=(n_{Ctr}-1)+(n_{Treat}-1)$

Mean af forskellen: $\mu_{\bar{X}_1-\bar{X}_2}=\mu_1-\mu_2$

Standardafvigelse af forskellen: $$S_{\bar{X}_{Ctr}-\bar{X}_{Treat}}=\sqrt{\frac{S_{Ctr}^{2}}{n_{Ctr}}+\frac{S_{Treat}^{2}}{n_{Treat}}}$$

Varians af forskellen: $S_{\bar{X}_{Ctr}-\bar{X}_{Treat}}^2=\frac{S_{Ctr}^2}{n_{Ctr}}+\frac{S_{Treat}^2}{n_{Treat}}$

Pooled varianser: $$S_p^2=\frac{(n_{Ctr}-1)\cdot S_{Ctr}^2+(n_{Treat}-1)\cdot S_{Treat}^2}{n_{Ctr}+n_{Treat}-2}$$

Cohen's d: $$\hat{d}=\frac{(\bar{X}_{Ctr}-\bar{X}_{Treat})}{\sqrt{S_p^2}}$$
Konfidensinterval for difference scorer: $$\begin{aligned}&CI_{.95}=(\bar{X}_{Ctr}-\bar{X}_{Treat})\pm t_{.05(two-tailed)}\cdot S_{\bar{X}_{Ctr}-\bar{X}_{Treai}}\\&CI_{.95}=(\bar{X}_{Ctr}-\bar{X}_{Treat})\pm t_{.05(two-tailed)}\cdot\sqrt{S_{p}^{2}\cdot(\frac{1}{n_{Ctr}}+\frac{1}{n_{Treat}})}\end{aligned}$$

![E6.png](/img/user/attachments/E6.png)

