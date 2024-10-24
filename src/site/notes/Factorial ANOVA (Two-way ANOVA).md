---
{"dg-publish":true,"permalink":"/Factorial ANOVA (Two-way ANOVA)/"}
---

# Factorial ANOVA (Two-way ANOVA)
[[SPSS Factorial ANOVA\|SPSS Factorial ANOVA]]

![Pasted image 20241024152852.png](/img/user/attachments/Pasted%20image%2020241024152852.png)

## Formler
$$s_{\mathrm{total}}^2=MS_{\mathrm{total}}=\frac{SS_{\mathrm{total}}}{df_{\mathrm{total}}}$$
$$MS_A=\frac{SS_A}{df_A}\quad MS_B=\frac{SS_B}{df_B}\quad MS_{A\times B}=\frac{SS_{A\times B}}{df_{A\times B}}=\frac{SS_{A\times B}}{df_A\cdot df_B}$$
$$MS_{error}=\frac{SS_{error}}{df_{error}}$$
$$F_A=\frac{MS_A}{MS_{error}}\quad F_B=\frac{MS_B}{MS_{error}}\quad F_{A\times B}=\frac{MS_{A\times B}}{MS_{error}}$$

$$F_{0.05}(df_A,df_{error})\quad F_{0.05}(df_B,df_{error}) \quad F_{0.05}(df_{A\times B},df_{error})$$
$$\eta_p^2(A)=\frac{SS_A}{SS_A+SS_{error}}$$
## Effektstørrelse: $\eta_p^2$
η𝑝2 (partial eta-squared) beskriver, hvor stor en andel af variabiliteten i data, der forklares af en variabel (her A), når variabilteten forklaret af andre variable er udeladt.

## Interaktion
Nulhypotesen for interaktion: Variablerne er additive. Effekten af variabel1 + variabel2 er det samme som effkten af variabel1 alene + effekten af variabel2 alene

Finder vi en signifikant interaktion i et faktorielt design, har vi evidens for non-additive effekter.
"More than the sum" - "Less than the sum"

![Pasted image 20241024153158.png](/img/user/attachments/Pasted%20image%2020241024153158.png)![Pasted image 20241024153202.png](/img/user/attachments/Pasted%20image%2020241024153202.png)