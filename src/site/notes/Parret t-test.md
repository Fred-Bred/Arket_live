---
{"dg-publish":true,"permalink":"/Parret t-test/"}
---

# Paired samples t-test
[[SPSS Paired samples t-test\|SPSS Paired samples t-test]]

"En paired samples t-test (parret t-test) er en one sample t-test af difference scorer"

![Pasted image 20241023174327.png](/img/user/attachments/Pasted%20image%2020241023174327.png)![Pasted image 20241023174331.png](/img/user/attachments/Pasted%20image%2020241023174331.png)

**Forskningsspørgsmål:** 
> Hvad er sandsynligheden for at trække et sample med en gennemsnitlig difference score (D ̅) eller med en mere ekstrem score under antagelse af nulhypotesen?

H0: $\mu_D=0$ eller $\mu_{EOT}=\mu_{Baseline}$
H1: $\mu_D \neq 0$ eller $\mu_{EOT} \neq \mu_{Baseline}$

**Konklusion:**
> En paired samples t test (two-tailed, α=.05) viste at symptomerne på skizofreni målt med PANSS blev reduceret signifikant fra X ̅=69.7 (SD=12.0) før terapi til X ̅=59.2 (SD=19.7) efter terapi, t(19)=3.67, p<.05, d=0.88

t-score: $$t=\frac{\overline{D}-\mu_D}{\left(\frac{S_D}{\sqrt{N}}\right)}=\frac{\overline{D}-\mu_D}{S_D}$$
Difference score: $D = X_{Baseline} - X_{EOT}$

Mean difference score: $\bar{D} = \sum_i \frac{D_i}{N}$

Gennemsnitlig ændring for populationen: $S_\bar{D}=\frac{S_D}{\sqrt{N}}$

Degrees of freedom: $df=N-1$

Cohen's d: $$\hat{d}=\frac{\bar{X}_{Baseline}-\bar{X}_{EOT}}{S_{Baseline}}$$

Konfidensinterval for difference score: $$CI_{.95}=\overline{D}\pm t_{.05(two-tailed)}\cdot\frac{s_{D}}{\sqrt{N}}$$
![E6.png](/img/user/attachments/E6.png)