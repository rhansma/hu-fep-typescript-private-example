# Access modifiers in Typescript
Zoals besproken in de les is het in Typescript mogelijk om net als bij bijvoorbeeld Java een access modifier toe te voegen aan methods of fields. In tegenstelling tot bij Java is het echter niet mogelijk om deze volledig af te dwingen. Aangezien Typescript uiteindelijk naar Javascript gecompileerd wordt zal het uiteindelijk naar een formaat gecompileerd worden waar access modifiers niet bekend zijn. 

Dit is goed te zien als je kijkt naar de files in de folder "output", de file eindigt op _private is het resultaat van de code zoals in scripts/alert.ts beschreven waar de methode sendMe private is. De file eindigt op _public is gecompileerd met de code van alert.ts met als enige wijziging dat de methode sendMe public is gemaakt. Probeer het zelf maar.

Als bewijs hebben we een knop gemaakt die op de html-pagina die gebruik maakt van de private methode sendMe van Alert. Als je op knop klikt zie je dat er gewoon een alert getoond wordt, terwijl de methode private is.