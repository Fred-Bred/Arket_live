---
{"dg-publish":true,"permalink":"/SPSS Logistisk regression/"}
---

# SPSS Logistisk regression
![Pasted image 20241024163729.png](/img/user/attachments/Pasted%20image%2020241024163729.png)![Pasted image 20241024163734.png](/img/user/attachments/Pasted%20image%2020241024163734.png)![Pasted image 20241024163807.png](/img/user/attachments/Pasted%20image%2020241024163807.png)

*Exp(B) svarer til Odds Ratio (OR)*
*Regressionsmodellen opstilles med brug af enten B eller Exp(B)-værdierne*

**Konfidensinterval for OR:**
Med 95% sandsynlighed vil populationens odds ratio være inkluderet i konfidensintervallet:

CI95 = [1.052;2.702]

Hvis 95% CI ikke inkluderer 1, er OR signifikant for alpha = 5% (two-tailed).

![Pasted image 20241024163944.png](/img/user/attachments/Pasted%20image%2020241024163944.png)

Nagelkerke $R^2$ er en pseudo-$R^2$ som kan sammenlignes med den vi bruger i multipel regression. Den beskriver hvor god den logistiske model er til at forklare fordelingen af 0'er og 1'er for den binære afhængige variabel.

**Konklusion:**
For at konkludere aflæses outputtet under sig. og Exp(B)
> En logistiske regression viste at bilister med høj social status var mere tilbøjelige til ikke at hold tilbage for fodgængere, OR = 1.472, p = .040, når der blev korrigeret for bilisternes estimerede køn, OR = 0.960, p = .906, og alder, OR = 0.852, p = .309.
> 
> Dette giver evidens for at konkludere at personer med høj social status er mere tilbøjelige til at udvise uetisk opførsel.