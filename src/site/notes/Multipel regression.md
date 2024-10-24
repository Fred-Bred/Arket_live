---
{"dg-publish":true,"permalink":"/Multipel regression/"}
---

# Multipel regression

Den lineære model: $Y ̂=b_0+b_1 X_1+b_2 X_2+⋯+b_p X_p$

$b_0$: Skæringspunkt (intercept) - ved simpel lineær regression: a

$b_{1,2…}$: regressionskoefficient (korrigeret for de andre prædiktorer)
      - Effekten af en prædiktor på den afhængige variable Y for fasholdt værdi af de ændre prædiktorer

**Forskningsspørgsmål**:
> Hvad har betydning for graden af mødres selvsikkerhed
> Afhængig: Selvsikkerhed
> Uafhængige: Selvtillid, Graden af støtte som barn

## SPSS og fortolkning
![Pasted image 20241024091526.png](/img/user/attachments/Pasted%20image%2020241024091526.png)

![Pasted image 20241024091536.png](/img/user/attachments/Pasted%20image%2020241024091536.png)
Vi bruger standardiserede koefficienter når de to værdier sammenlignes. Det der ses, er at SelfEsteem har større effekt end MatCare. Det afspejler sig også i p-værdien, men dette er ikke altid tilfældet. Kan også bruges til at holde to modeller op imod hinanden.

![Pasted image 20241024091704.png](/img/user/attachments/Pasted%20image%2020241024091704.png)

Modellen med disse to prædiktorer forklarer altså 15,8% af variansen i Y (Confidence i eksemplet)
Flere prædiktorer betyder som regel højere forklaringsgrad (R2) men på Statistik 1 og 2 kan man antage at modellen med den største R2 er den bedste, hvis man skal sammenligne modeller.

Modellen kan altså beskrives således: $$\hat{Y}=b_{MatCare}X_{MatCare}+b_{SelfEsteem}X_{SelfEsteem}+a$$

**Konklusion:**
> En multipel regression viste at graden af støtte som barn (MatCare) ikke har en signifikant effekt på selvsikkerheden i rollen som mor senere i livet (Confidence), b = 0.057, t(89) = 1.297, p = .198. Derimod viste analysen en signifikant effekt af selvtillid før første barn (SelfEsteem) på selvsikkerheden i rollen som mor senere i livet (Confidence), b = 0.146, t(89) = 3.022, p = .003.

### Fortolkning af koefficienter
![Pasted image 20241024091856.png](/img/user/attachments/Pasted%20image%2020241024091856.png)

B-koefficienten indikerer hvor stor betydning hver prædiktor (uafhængige variable) udgør.
B-koefficienten ganget "med den skala som den ligger på" fortæller hvilken betydning det har at ligge hvorhenne på den tilhørende skala

I eksemplet er pige kodet som 0 og dreng som 1
Hvis man i sin model sætter 1 (dreng) ind i ledet for køn, reduceres værdien med -0,943. Modsat reduceres det samlede output ikke hvis 0 (pige) indsættes i ledet for køn (-0,943*0 vs -0,943*1).

B-koefficienter aflæses altid under Unstandardized Coefficients medmindre formålet er at sammenligne to modeller, i hvilket tilfælde der aflæses under Standardized Coefficients

