---
{"dg-publish":true,"permalink":"/One sample t-test/"}
---

# One sample t-test
[[SPSS One sample t-test\|SPSS One sample t-test]]

Forskningsspørgsmål:
> Er gennemsnittetsscoren for et sample $\bar{X}$  trukket fra en population med middelværdi μ og ukendt standard afvigelse.

H0: Personer med misbrugsproblemer har en gennemsnitlig HAMD score som er *lig* cutoff: $μ_{\text{misbrug}} = \text{cutoff}$

H1: Personer med misbrugsproblemer har en gennemsnitlig HAMD score som er *forskellig fra* cutoff: $μ_{\text{misbrug}} \neq \text{cutoff}$


![Pasted image 20241023105608.png](/img/user/attachments/Pasted%20image%2020241023105608.png)

t-score: $$t=\frac{\bar{X}-\mu_{\bar{X}}}{\left(\frac{s}{\sqrt{N}}\right)}=\frac{\bar{X}-\mu_{\bar{X}}}{S_{\bar{X}}}$$
**Aflæs i tabel E.6 om t-værdien er højere end den kritiske værdi**
Beslutningsregel: Hvis p ≤ α -> H0 forkastes
Beslutningsregel: Hvis p > α -> H0 fastholdes

Middelværdi for populationen: $\mu_{\bar{X}}=\mu$

Standardafvigelse for populationen: $S_{\bar{X}}=\frac{S}{\sqrt{N}}$

Degrees of freedom: $\text{df} = N-1$

Konklusion:
> En t test viste at de fire personer med misbrugsproblemer har en gennemsnitlig HAMD score (X ̅=14.25) som ikke er signifikant forskellig fra cutoff til let depression på 13, t(3)=2.60,  p> .05 (two-tailed).

![Pasted image 20241023110238.png](/img/user/attachments/Pasted%20image%2020241023110238.png)