WordChains.NET
==============
_Tester ut hvordan det er å implementere denne oppgaven i .NET_

Testkjøring
-----------
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

