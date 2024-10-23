---
{"dg-publish":true,"permalink":"/Probability/"}
---

# Probability
## Additive law: Mutually exclusive events
p(A OR B)=p(A)+p(B)

**General rule:** The probability that A OR B occurs is the SUM of the individual probabilities minus the probability of **both** events combined

p(A OR B)=p(A)+p(B)-p(A and B)

**Eksempel:** Hvad er sandsynligheden for at slå enten et lige tal ELLER et tal højere end 3?

p(lige tal)=3/6
p(tal højere end 3)=3/6
p(tal≤3 som ikke er lige)=2/6

p(lige ELLER>3)=3/6+3/6-2/6=0,6667

Sandsynligheden at en hændelse ikke sker, er 1 minus sandsynligheden for at det sker:

p(ikke A)=1-p(A)

p(ikke A og ikke B)=1-(p(A)+p(B))
## Multiplicative law: Independent events
p(A AND B)=p(A)·p(B)

p(A AND B)=P(A, B)

**General rule:** The probability of the joint occurrence of two or more independent events is the product of their individual probabilities.

**Eksempel 1:** Hvad er sandsynligheden for at første terning bliver et lige tal og anden terning bliver et ulige tal?

p(1:lige tal)=3/6
p(2:ulige tal)=3/6

p(1:lige, 2:ulige)=3/6·3/6=9/36⇒1/4

**Eksempel 2:** Hvad er sandsynligheden for at 2 personer, der spiller ”sten, saks, papir”, får uafgjort 3 gange i træk (under antagelse af at sandsynlighed for de tre valg er ens og at valgene foretages uafhængigt)?

p(vind)=1/3
p(tab)=1/3
p(uafgjort)=1/3

p(uafgjort tre gange i træk)=1/3·1/3·1/3=1/27

## Eksempel
Tre børn modtager standardbehandling for ADHD. Antag at behandlingsudfaldende for de tre børn er uafhængige, og at sandsynligheden for, at behandlingen er en succes, er πA for barn A, πB for barn B og πC for barn C

**Hvad er sandsynligheden for at behandlingen er en *succes for alle tre børn?***
$p(\text{A AND B AND C})=π_A·π_B·π_C$

**Hvad er sandsynligheden for at behandlingen er en *succes for barn A*, men ikke for barn B og barn C?**
$p\text{(A, NOT B, NOT C)}=π_A·(1-π_B )·(1-π_C)$

**Hvad er sandsynligheden for at behandlingen er en *succes for Barn B*, men ikke for barn A og barn C?**
$p\text{(NOT A, B, NOT C)}=(1-π_A)·π_B·(1-π_C)$

**Hvad er sandsynligheden for at behandlingen er en *succes for barn C*, men ikke for barn A og barn B?**
$p\text{(NOT A, NOT B, C)}=(1-π_A)·(1-π_B)·π_C$

**Hvad er sandsynligheden for at behandlingen er en *succes for én og kun én* af de tre børn?**
$$p\text{(A, NOT B, NOT C)}+p\text{(NOT A, B, NOT C)}+p\text{(NOT A, NOT B, C)}=(π_A·(1-π_B )·(1-π_C ))+((1-π_A )·π_B·(1-π_C ))+((1-π_A )·(1-π_B )·π_C)$$

**Hvad er sandsynligheden for at behandlingen er en *succes for to og kun to* af de tre børn?**
$$p\text{(A, B, NOT C)}+p\text{(A, NOT B, C)}+p\text{(NOT A, B, C)}=(π_A·π_B·(1-π_C ))+(π_A·(1-π_B)·π_C )+((1-π_A )·π_B·π_C)$$
## Eksempel fra øvelse
![Pasted image 20241023095951.png](/img/user/attachments/Pasted%20image%2020241023095951.png)