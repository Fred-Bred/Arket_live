---
{"dg-publish":true,"permalink":"/Power i t-tests/"}
---

# Power i t-tests
![Pasted image 20241023093024.png](/img/user/attachments/Pasted%20image%2020241023093024.png)
![Pasted image 20241023092506.png](/img/user/attachments/Pasted%20image%2020241023092506.png)

## One-sample t-test
[[One sample t-test\|One sample t-test]]

**Spørgsmål: Hvad er effektstørrelsen (Cohen's d) for studiet?**
$$\hat{d}=\frac{\bar{X}-\mu_0}{s}$$

**Spørgsmål: Hvis vi gentager samme studie med samme n, hvad er det bedste bud på t-score?**
*Find non-centrality parameter δ*

$$\delta = \hat{d} \sqrt{N}$$
**Spørgsmål: Hvad er post-hoc power af dette studie?**
Aflæs tabel E.5 ud fra $\delta$ og dit signifikansniveau

**Spørgsmål: Hvis du gentager samme studie med et andet n, hvilken power ville du så opnå?**
$$\delta = \hat{d} \sqrt{N}$$

Aflæs i E.5

**Spørgsmål: Antag at du vil gentage studiet. Hvor stort et n skal du have, for at opnå en specifik power (i.e. 80%)**
$$n=\frac{\delta^2}{\hat{d}^2}$$

## Paired samples t-test
[[Parret t-test\|Parret t-test]]

**Spørgsmål: Hvad er effektstørrelsen (Cohen's d) for studiet?**
$$\hat{d}=\frac{\bar{D}}{S_D}$$

**Spørgsmål: Hvis vi gentager samme studie med samme n, hvad er det bedste bud på t-score?**
*Find non-centrality parameter δ*

$$\delta = \hat{d} \sqrt{N}$$
**Spørgsmål: Hvad er post-hoc power af dette studie?**
Aflæs tabel E.5 ud fra $\delta$ og dit signifikansniveau

**Spørgsmål: Hvis du gentager samme studie med et andet n, hvilken power ville du så opnå?**
$$\delta = \hat{d} \sqrt{N}$$

Aflæs i E.5

**Spørgsmål: Antag at du vil gentage studiet. Hvor stort et n skal du have, for at opnå en specifik power (i.e. 80%)**
$$n=\frac{\delta^2}{\hat{d}^2}$$
## Independent sample t-test
[[Uparret t-test\|Uparret t-test]]

**Spørgsmål: Hvad er effektstørrelsen (Cohen's d) for studiet?**
$$\hat{d}=\frac{\bar{X}_1-\bar{X}_2}{S_p}$$

**Spørgsmål: Hvis vi gentager samme studie med samme n, hvad er det bedste bud på t-score?**
*Find non-centrality parameter δ*

$$\delta = \hat{d} \sqrt{\frac{N}{2}}$$
**Spørgsmål: Hvad er post-hoc power af dette studie?**
Aflæs tabel E.5 ud fra $\delta$ og dit signifikansniveau

**Spørgsmål: Hvis du gentager samme studie med et andet n, hvilken power ville du så opnå?**
$$\delta = \hat{d} \sqrt{\frac{N}{2}}$$

Aflæs i E.5

**Spørgsmål: Antag at du vil gentage studiet. Hvor stort et n skal du have, for at opnå en specifik power (i.e. 80%)**
$$n=\frac{\delta^2}{\hat{d}^2}$$
