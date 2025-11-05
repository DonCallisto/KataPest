# Kata... what?

Kata è un termine mutuato dalle arti marziali. È la ripetizione di un set di movimenti provati e riprovati al fine di
renderli automatici come un riflesso. 

Il termine Code Kata è attribuito a Dave Thomas.

Applicato al TDD, aiuta a perfezionare il feedback loop "RED - GREEN - REFACTOR". Il feedback loop R.G.R. aiuta a riflettere
sul design di ciò che stiamo scrivendo. Lo scopo del Kata non è quello di creare design emergente ma di praticare il
feedback loop al fine di utilizzarlo in progetti reali, in cui, il design può emergere più facilmente.

# Constraints... li vogliamo? Quanti? Scegliamoli insieme

## Baby Steps

Regole:

1) Settiamo un timer breve (5 minuti?)
2) Scrivere esattamente un solo test
   1) Se il timer suona e il test è rosso: checkout e si riparte
   2) Se il timer non è suonato: resetta e passa al prossimo test
3) Resetta il timer
4) Torna al 2

## Ensemble Programming

Regole:

1) Gruppi piccoli <5 persone
2) Un driver; non entra nelle decisioni, scrive solo codice
3) Tanti navigator che pensano alla soluzione da applicare. In caso di disaccordo, decide un navigator designato all'inizio.

## Minimalist

Regole:

1) Coppie di 2
2) Uno scrive solo il test
3) L'altro scrive solo il codice per far passare il test
4) Entrambi fanno refactor

## Mute Ping-Pong

Regole:

Come il minimalist ma con un vincolo in più: **la coppia non può comunicare se non attraverso il codice** (e no... non valgono
i commenti sul codice)

Setup a git repository (or use another SCM that supports resets)
Setup a timer for 2 minutes interval when you start
Write exactly one test
If the timer rings and the test is red then revert and start over
If you finish your test earlier: no problem, reset the timer and continue
Restart timer
Go to 3.

# RUN IT!

1) docker compose build
2) docker compose up -d
3) docker exec -it kata-pest bash
4) composer install

You can now run Kata-Test with `./vendor/bin/pest`/