---
{"dg-publish":true,"permalink":"/One-way ANOVA/"}
---

# One-way ANOVA
One-way ANOVA skal på statistik 2 kunne udføres "i hånden". Excel-udgaven er mere udførlig og kan lave de fleste udregninger for dig.

[[SPSS One-way ANOVA\|SPSS One-way ANOVA]]

ANOVA bruges til at sammenligne gennemsnit for tre eller flere grupper. Den minder om en t-test men mindsker risikoen for type 1 fejl ved først at lave én test der blot undersøger om der er signifikant forskel *et eller andet sted* mellem alle de sammenlignede grupper. Hvis testen er signifikant udføres Fisher's least significant difference (LSD) test for at finde frem til hvilke grupper forskellen er imellem.

![Pasted image 20241024094043.png](/img/user/attachments/Pasted%20image%2020241024094043.png)
Den afgørende værdi, *F* findes således: $$F=\frac{MS_{group}}{MS_{error}}$$
Denne kan sammenlignes med den kritiske værdi i tabel [[E3.png|E.3]].

$$MS_{\mathrm{group}}=\frac{\sum_{j=1}^kn_j\left(\overline{X}_j-\bar{X}_{\mathrm{gm}}\right)^2}{k-1}=\frac{SS_{\mathrm{group}}}{df_{\mathrm{group}}}$$
$$MS_{\mathrm{group}}=\frac{SS_{group}}{df_{group}}=\frac{SS_{group}}{k-1}$$

$$MS_{\mathrm{error}}=\frac{(n_1-1)s_1^2+(n_2-1)s_2^2+(n_3-1)s_3^2}{n_1+n_2+n_3-k}$$

$$MS_{\mathrm{error}}=\frac{SS_{\mathrm{error}}}{df_{\mathrm{error}}}=\frac{SS_{\mathrm{erro}}}{N-k}$$

$$SS_{\mathrm{total}}=\sum_{i=1}^{k}\sum_{i=1}^{n_{j}}\left(x_{ij}-\bar{X}_{\mathrm{gm}}\right)^{2}$$

$$SS_{Group}=\sum_{j=1}^{k}n_{j}\big(\bar{X}_{j}-\bar{X}_{\mathrm{gm}}\big)^{2}$$

$$SS_{\mathrm{error}}=SS_{\mathrm{total}}-SS_{\mathrm{group}}$$
$$\eta^2=\frac{SS_{group}}{SS_{total}}$$

$$\begin{aligned}
&SS_{\mathrm{error}}=SS_{\mathrm{total}}-SS_{\mathrm{group}} \\
&df_{\mathrm{total}}=N-1 \\
&df_\text{group}=k-1 \\
&df_\text{error}=N-1-(k-1)=N-k \\
&N=n_1+n_2+n_3
\end{aligned}$$

$$\begin{aligned}&k=\text{antal grupper}\\&\bar{X}_j=\text{middelværdi for gruppe j}\\&\bar{X}_{gm}=\text{Grand mean, den totale middelværdi}\\&n_j=\text{antallet af personer i gruppe j}\\&ss=\text{sum of squares}\\&df=\text{degrees of freedom}\end{aligned}$$

**konklusion:**
> 24 studerende blev tilfældigt inddelt i tre grupper og sat til at studere en tekst i 30 minutter, hvorefter de skulle besvare 10 multiple-choice spørgsmål. Grupperne studerede teksten med henholdsvis konstant, varierende eller ingen baggrundsstøj. En one-way ANOVA viste en signifikant effekt af baggrundsstøj på antal korrekte spørgsmål, F(2,21) = 3.5, p = .049, η2 = .25

## Fisher's least significant difference (LSD)
![Pasted image 20241024093649.png](/img/user/attachments/Pasted%20image%2020241024093649.png)
