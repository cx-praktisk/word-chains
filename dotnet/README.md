WordChains.NET
==============
_Tester ut hvordan det er å implementere denne oppgaven i .NET_

Utkast til oppgave
------------------
Først presenterer vi problemet, så jobber folk sammen. Til hvert steg er det et par testeksempler som kan brukes. Tanken er at en koder opp mot en test, når denne funker byter man. Så finner nestemann en test som ikke funker og koder opp mot den, osv.

### Finn avstanden mellom ord
Her implementerer man noe som funker som (ABBA, ALBA) -> 1

### Finn alle ord med en gitt avstand i en liste med ord
Her finner man f.eks. (ABBA, [ALBA, SALT, KATT, ABVA]) -> [ALBA, ABVA]

### Finn kjeden mellom to ord i ordlisten
Her syr man det sammen slik at (ABBA, [ALBA, SALT, KATT, ABVA]) -> ABBA => ALBA

Noen jenkapunkter som man kan presentere ved å ha de i senere testsett:
* Sykler, AKA. man går frem og tilbake mellom to ord.

### Test med Scrabbleforbundet sin ordliste
Her kan det være at det dukker opp noen ting ja.

### Kan dere finne den korteste kjeden?
Bredde først leder kanskje frem?

### Kan dere gjøre det raskere?
Hvordan gjøre denne jobben kjappere?

Testkjøring uten støtte
-----------------------
1. _17:40_ - Lag en funksjon som lager alle ord som er en endring vekk fra det opprinnelige ordet
2. _18:00_ - Huff! Dette ble masse rot med `for` og `char[]` :-(
3. _18:15_ - Abort plan! Denne leder ikke frem.
4. _18:15_ - Beregn hvor mange forskjeller det er mellom to ord aka. distanse (ABBA/ALBA har distanse 1 osv.)
5. _??:??_ - Gitt en ordbok av `string[]`. Finn ordene i ordboka som har en gitt distanse fra et annet ord.
6. _??:??_ - Gitt en ordbok og to ord med samme lengde. Finn kjeden mellom ordene, hvor hvert ord er en gitt distanse unna.
7. _??:??_ - Hmm, kanskje bredde først, men DFS er så mye enklere å implementere rekursivt.
8. _??:??_ - Ohoi, jeg har ikke korrekt termineringsbetingelse, så nå har jeg en evig loop.
9. _??:??_ - CAT -> COT -> CAT. Ohoi! jeg har ikke tatt hensyn til sykler!
10. _??:??_ - Funker det nå?
11. _19:58_ - Det funker! :-D

