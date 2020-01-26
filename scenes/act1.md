# act1

```
SceneSetup.act1();
```

(...300)

n: E QUESTA È LA SUA ANSIA

n: _TU_ SEI L'ANSIA

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Oh ehi! Siamo di nuovo qui?

`hong({eyes:"0_neutral"})`

n: IL TUO COMPITO È PROTEGGERE IL TUO UMANO DAL *PERICOLO*

`bb({eyes:"look", mouth:"small_lock"})`

n: INFATTI LO STAI METTENDO IN *PERICOLO* GIOCANDO A QUESTO GIOCO PROPRIO ORA

n: PRESTO, AVVERTILO!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Umano! Ascolta, siamo in pericolo! Chi sta giocando...

[...ci torturerà ancora!](#act1_replay_torture)

[...non troverà un finale alternativo!](#act1_replay_alternate)

[...incapperà in una dissonanza ludonarrativa!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Ci farà rannicchiare e piangere!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Ci farà uccidere il tuo smartphone per averti provocato un attacco di panico!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: *NON* ci farà prendere a pugni l'organizzatore della festa!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Ci farà prendere a pugni il Solidale Anti-Cattivo organizzatore della festa!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Beh almeno potremmo evitare di saltare questa vol--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: CI FARÁ SALTARE DAL TETTO.
{{/if}}

`bb({body:"fear"});`

b: CI SUCCEDERANNO TUTTE QUESTE COSE TERRIBILI, E POI SAREMO--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Certo, la storia *nell'insieme* è la stessa, ma ogni capitolo ha due possibili finali, più tutte le possibili biforcazioni dei dialo--

`bb({body:"fear"});`

b: Chi gioca ne sarà dispiaciuto, chiuderà la finestra del browser, cancellerà il nostro programma e poi noi--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Una lurido-che?

`bb({eyes:"normal"});`

b: L'arco narrativo era su come puoi *SCEGLIERE* di instaurare una sana collaborazione con la tua paura,

`bb({eyes:"normal_right"});`

b: Ma rigiocando il gioco avrai la stessa storia, il che implica che le tue *SCELTE* non contano,

`bb({eyes:"narrow_eyebrow"});`

b: Mostrando dunque una contraddizione tra il messaggio del gioco e le sue meccaniche,

`bb({eyes:"fear"});`

b: Sbrogliando quindi la trama di questo universo narrativo,

`bb({body:"fear"});`

b: E poi noi--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: MORIREMOOOOOOOOOOO

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: OK rientriamo nel personaggio.

```
Game.clearText();
```

n4: (FAI ENTRARE LA _TUA_ ANSIA BLAH BLAH BLAH SIMILE ALLE _TUE_ PAURE BLAH BLAH SAI GIÀ COME FUNZIONA)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Grandioso, riecco il mio lupo. Faaaaantastico.

`hong({eyes:"0_neutral"})`

n: IL TUO COMPITO È PROTEGGERE IL TUO UMANO DAL *PERICOLO*

`bb({eyes:"look", mouth:"small_lock"})`

n: IN EFFETTI, QUEL TRAMEZZINO LO STA METTENDO IN *PERICOLO* PROPRIO ORA

n: PRESTO, AVVERTILO!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Umano! Ascolta, siamo in pericolo! Il pericolo è...

`bb({body:"squeeze"})`

n4: (LASCIA CHE LA _TUA_ ANSIA GIOCHI CON TE! SCEGLI CIÒ CHE LA _TUA_ PAURA TI DICE)

(#act1_normal_choice)

# act1_normal_choice

[Stiamo pranzando in solitudine! Di nuovo!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Star qui a mangiare non è produttivo!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Il pane bianco non ci fa bene!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Ma lo sai che la solitudine è associata a una morte prematura tanto quanto fumare 15 sigarette al giorno?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Um, grazie per aver citato le fonti ma--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Il che vuol dire che se non facciamo qualcosa con qualcuno *proprio adesso* finiremo per-

`bb({body:"panic"})`

b: MORIIIIIREEEEEEEEEEEE

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: HAI USATO LA *PAURA DI NON ESSERE AMATI*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Tira fuori il tuo laptop e lavora, ora!

`hong({eyes:"0_annoyed"})`

h: Um, Preferirei non riempire di briciole la mia tastier--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Se non contribuiamo alla società allora siamo dei parassiti della società!

b: La società andrà dal dottore delle società per farsi dare delle medicine che uccidano i parassiti della società e noi finiremo per--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: MORIREEEEEEEEEEEEEEE

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: HAI USATO LA *PAURA DI DIVENTARE CATTIVE PERSONE*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Ma questo è scientificamente provat--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Il grano raffinato farà impennare la nostra glicemia, poi dovranno amputare tutti i nostri arti e poi finiremo per--

`bb({body:"panic"})`

b: MORIREEEEEEEE

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: HAI USATO LA *PAURA DI ESSERE FERITI*

(#act1b)

# act1b

n: È SUPER EFFICACE

`bb({mouth:"smile", eyes:"smile"});`

b: Vedi, umano? Io sono il tuo leale lupo da guardia!

`bb({body:"pride_talk"});`

b: Ascolta l'istinto! Le tue emozioni hanno ragione!

`bb({body:"pride"});`

n: FAI ARRIVARE A ZERO LA BARRA DI ENERGIA DEL TUO UMANO

n: PER PROTEGGERE I SUOI BISOGNI FISICI + SOCIALI + MORALI, PUOI USARE:

n: PAURA DI *ESSERE FERITI* #harm#

n: PAURA DI *NON ESSERE AMATI* #alone#

n: PAURA DI ESSERE *CATTIVE PERSONE* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (CONSIGLIO: FA' LE SCELTE CHE COLPISCONO LE TUE PIÙ INTIME E OSCURE PAURE!)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: sì, forse è arrivato il momento di controllare il telefono.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: PROTEGGI IL TUO UMANO

n: DAL MONDO. DALLE ALTRE PERSONE. DA SÉ STESSO.

n: BUONA FORTUNA

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: ROUND ONE: *FIGHT!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Huh. C'è un post su Facebook che dice che c'è un party questo weekend.

`bb({eyes:"uncertain"});`

b: Ma quel matto fa una festa *ogni* weekend?

`bb({eyes:"uncertain_right"});`

b: Chissà che vuoto interiore sta cercando di colmare? Dev'esserci un vero casino in quella testa!

`hong({eyes:"surprise"});`

h: Tra l'altro, ho ricevuto un invito?

`bb({eyes:"fear", mouth:"normal"});`

b: Bene!

[Di' di sì o moriremo dalla solitudine](#act1c_loner)

[Di' di no, quella festa è piena di droga!](#act1c_drugs)

[Ignoralo, noi rendiamo tristi le feste.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Quindici sigarette al giorno, umano! Quindici!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: Poi nessuno verrà al nostro funerale, butteranno le ceneri nell'oceano, queste poi verranno mangiate da una balena,
{{/if}}

{{if !_.fifteencigs}}
b: e diventeremo CACCA DI BALENA!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: Quindi sì, dovremmo andare a quella festa!
{{/if}}

{{if _.parasite}}
b: Porta anche il laptop così possiamo lavorare, e non essere dei parassiti della società.
{{/if}}

{{if _.whitebread}}
b: Solo se non ci faranno mangiare del PANE BIANCO
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: Cristo. Se questo ti farà tacere, va bene.

h: Dirò di sì.

{{if _.whalepoop}}
b: Cacca di balena, umano! Cacca di balena!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: o peggio... PANE BIANCO
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Faremo un'overdose di metanfetamina e pane bianco così enorme che non riusciranno a mettere il nostro cadavere ciccione nel forno crematorio!
{{/if}}

{{if !_.whitebread}}
b: Prenderemo così tante droghe che il becchino si chiederà come mai il nostro corpo sia *già* pre-imbalsamato!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: D'altronde, non possiamo far bisboccia, dobbiamo lavorare o saremo dei terribili parassiti della società!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: Cristo. Se questo ti farà tacere, va bene.

h: Dirò di no.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Tutto quello che facciamo è piagnucolare su come la solitudine sia terribile quanto fumare 15 sigarette al giorno.
{{/if}}

{{if _.parasite}}
b: Tutto quello che facciamo alle feste è preoccuparci del fatto che dovremmo essere più produttivi.
{{/if}}

{{if _.whitebread}}
b: Tutto quello che facciamo è preoccuparci di come la nostra cattiva dieta ci farà morire.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: eh, chissà perché.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Quindi se andiamo li facciamo stare male, ma se rifiutiamo l'invito li facciamo stare male comunque!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: NON FACCIAMO CHE FAR STARE MALE LE PERSONE: DOVREMMO ESSERE NOI A STARE MALE

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Ugh. Se questo ti farà tacere, va bene.

h: Ignorerò l'invito.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Comunque. Facebook è troppo per me. Ho bisogno di qualcosa di più tranquillo, meno ansiogeno.

`hong({eyes:"neutral"});`

h: Vediamo cosa c'è su Twitter...

`bb({eyes:"look"});`

[Oh no, che notizia orribile!](#act1d_news)

[Ehi, ma quel tweet si riferisce forse a *noi?*](#act1d_subtweet)

[Ehi, una GIF di un gattino che beve il latte](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Dio, sembra che il mondo stia bruciando, vero?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Sembra che il mondo stia finendo, come se tutto stesse per morire. Siamo spacciati, non c'è niente che possiamo fare.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Facciamo un retweet della notizia!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Ok. Lo faccio, ma per piacere calmati!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: ^Sticazzi^, vediamo cosa c'è su Snapchat.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: È un subtweet! Un subdolo, infido subtweet! Stanno parlando di noi senza menzionarci!

`hong({eyes:"annoyed"});`

h: O magari no?

`bb({eyes:"narrow", mouth:"small"});`

b: e se tutti stessero sparlando alle nostre spalle?

h: Non--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: DI FRONTE ALLE NOSTRE SPALLE

`hong({eyes:"sad", mouth:"sad"});`

h: Io non--

`bb({eyes:"narrow", mouth:"small"});`

b: ma *se*

h: S--

`bb({eyes:"narrow_eyebrow"});`

b: *se*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Vaaabene, provo Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Heh carino! Faccio un retweet, penso che--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: I GATTI NON DIGERISCONO IL LATTE E SIAMO DELLE PERSONE ORRIBILI PER GODERE DEGLI ABUSI SUGLI ANIMALI

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Vaaabene, provo Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Uh, foto di ieri sera. Quindi *ecco* come sono quelle feste.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Uff! Sembra troppo affollato per la mia ansia.

h: Forse non avrei dovuto accettare l'invito?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Cambiare la nostra risposta? Come degli idioti?!](#act1e_yes_dontchange)

[Cambia la nostra risposta! C'è troppa gente a quel party!](#act1e_yes_changetono)


{{if _.subtweet}}
[Eh si, decisamente un subtweet su di noi.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Aspetta, ma abbiamo ritwittato senza controllare le fonti?](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Sai chi ha davvero una cattiva postura?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Contavano su di noi e ora li stiamo tradendo? Vuoi morire in solitudine?

{{if _.fifteencigs}}
b: QUINDICI. SIGARETTE.
{{/if}}

{{if _.whalepoop}}
b: CACCA. DI BALENA.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Taci, taci! Risponderò di sì.

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Hai presente l'essere travolti da una ressa?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Nel 2003 in un night di Rhode Island c'è stato un incendio e le persone prese dal panico hanno intasato le uscite e 100 persone sono morte bruciate.

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: VUOI CHE QUESTO SUCCEDA A NOI-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: DI' DI NO DI' DI NO DI' DI NO DI' DI NO DI' DI NO DI' DI NO DI' DI N-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Taci! Cambio la mia risposta in no! Dio santo.

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... sembra molto divertente

h: Forse non avrei dovuto dire di no all'invito? 

`bb({mouth:"normal", eyes:"normal"});`

[Cambiare la nostra risposta? Come degli idioti?!](#act1e_no_dontchange)

[Cambia la nostra risposta! Non morire di solitudine!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Eh si, decisamente un subtweet su di noi.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Aspetta, ma abbiamo ritwittato senza controllare le fonti?](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Sai chi ha davvero una cattiva postura?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Tutti contavano su di noi!

b: ...che li lasciassimo in pace a fare la loro bella festa senza orribili disgustosi vermi {{if _.whitebread}}mangiatori di pane bianco{{/if}} come n--


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Taci, taci! Lascio no!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: La solitudine cronica aumenta i nostri livelli di cortisolo e i rischi di malattie cardiovascolari e infarti!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: QUINDICI. SIGARETTE.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Taci, taci! Risponderò di sì! Dio santo!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Tutti i nostri tweet problematici son tornati all'ovile!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Ci smaschereranno, ci toglieranno l'amicizia e ci legheranno ad un cavallo per trascinarci lungo la superstrada informatica!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Perché devi fare così?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Stiamo diffondendo disinformazione! Stiamo disgregando la fiducia nella stampa libera!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Siamo la ragione per la quale il fascismo risorgerà dalle macerie della democrazia! 

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: Perché devi fare così?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Vuoi avere un pretzel al posto della spina dorsale?! Finiscila di ingobbirti sul tuo schermo!

```
bb({body:"meta"});
```

b: Questo vale anche per te.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Perché devi fare così?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... sembra molto divertente.

h: Forse non avrei dovuto ignorare l'invito?

`bb({mouth:"normal", eyes:"normal"});`

[Continua a ignorarlo, siamo pur sempre guastafeste.](#act1e_ignore_continue)

[Ripensandoci, di' di sì.](#act1e_ignore_changetoyes)

[Ripensandoci, di' di no.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: È un po' scortese continuare a ignorarli però, no?

`bb({eyes:"normal_right"});`

b: Beh gli altri ignorano sempre *noi*, quindi

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: quindi siamo pari.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Stai... lasciando che mi diverta?

b: Beh, voglio dire, la solitudine *può* ucciderci.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: È troppo affollato. E le folle sono pericolose.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Uh. Nuova notifica di Tinder.

`bb({eyes:"uncertain"})`

b: Cosa? La app per rimorchiare?

`hong({eyes:"annoyed"})`

h: Non è una app per rimorchiare, è solo un modo per incontrare nuova gen--

`bb({eyes:"narrow"})`

b: È un'app per rimorchiare.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Oh, ho un match! Sexy!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Per piacere non rovinare anche ques--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: PERICOLO PERICOLO PERICOLO PERICOLO PERICOLO PERICOLO

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Le persone ci *usano*.](#act1f_used_by_others)

[*Usiamo* le persone.](#act1f_using_others)

[IL TUO MATCH È UN SERIAL KILLER](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Rimorchi casuali forse potrebbero riempire qualche vuoto laggiù,

b: ma non potranno mai riempire il vuoto...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *qui*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Il fatto è che FINIREMO PER MORIRE DA SOLI

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Pensi che i genitali della gente siano come dei Pokémon da collezionare?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (sigla dei pokemon)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ Voglio ^trombare^ dove mi va-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ E non fermarmi qua-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Quel ^cazzone^, penetrerà-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ il mio grande ^culon^!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ SONO UNA PORCA-MON! PORCA-MO-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Il fatto è che siamo dei vermi manipolatori.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: Ti intrappoleranno in un pozzo e ti ingozzeranno di pane bianco per ingrassarti così potranno indossare la tua pelle come un vestito!
{{/if}}

{{if _.parasite}}
b: Ti randelleranno con la tua tabella di marcia e ti diranno "AVRESTI DOVUTO PRODURRE DI PIÙ, PARASSITA"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Ti faranno a brandelli, faranno coriandoli della tua carne, trasformeranno le tue viscere in stelle filanti, e faranno sangria col tuo sangue.
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Come ti suona QUESTO come invito ad una festa?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)


h: Non ne posso più di questo gioco.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"la solitudine ci ucciderà"... {{/if}}
{{if _.parasite}}"siamo un parassita della società"... {{/if}}
{{if _.whitebread}}"non mangiarlo, ci ucciderà"... {{/if}}
{{if _.subtweet}}"stanno parlando alle nostre spalle"... {{/if}}
{{if _.badnews}}"il mondo brucia"... {{/if}}
{{if _.hookuphole}}"moriremo in solitudine"... {{/if}}
{{if _.serialkiller}}"sono serial killer"... {{/if}}
{{if _.catmilk}}"i gatti non digeriscono il latte"... {{/if}}
{{if _.pokemon}}"la ^fottuta^ parodia di una sigla"... {{/if}}

h: voglio solo vivere la mia vita

h: voglio solo liberarmi di questo... dolore.

`bb({eyes:"look_sad"});`

b: Ehi... umano...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Andrà tutto bene.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Come tuo fedele lupo da guardia, sarò sempre in allerta, e farò del mio meglio per tenerti al sicuro.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Te lo prometto.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Ultima app. Instagram. Vediamo che si dice.

`hong({eyes:"sad"});`

h: Ci sono... altre foto di feste.

`hong({mouth:"sad"});`

h: Sembrano tutti così felici. Senza preoccupazioni. Senza ansie.

`hong({mouth:"anger"});`

h: Dio, perché non posso essere come loro? Perché non posso essere *normale?*

`bb({eyes:"normal_right"});`

b: A proposito di feste, riguardo l'invito per questo weekend. Questa è la mia decisione FINALE:

`bb({eyes:"normal"});`

[Dovremmo andarci.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Non dovremmo andarci.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Dovr--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: VAI A FARTI

`hong({body:"2_you"});`

h: *FOT-TE-RE*.

(...500)

b: c-

(...1500)

`bb({eyes:"wat_2"});`

b: che?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Io ci VADO a quella festa,

{{if _.act1g=="go"}}
h: NON perché tu vuoi che io ci vada, ma perché lo voglio *IO*.
{{/if}}

{{if _.act1g=="dont"}}
h: Proprio perché TU vuoi che io non vada.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Tu non hai ALCUN controllo su di me.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Ora scusami mentre mangio questo ^fottuto^ tramezzino in pace.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[AHHHH MORIREMO](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH TUTTI CI ODIANO](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH SIAMO PERSONE ORRIBILI](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH MORIREMO AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH TUTTI CI ODIANO AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH SIAMO PERSONE ORRIBILI AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: CONGRATULAZIONI

(...500)

n: HAI PROTETTO I BISOGNI FISICI + SOCIALI + MORALI DEL TUO UMANO

n: GUARDA COM'È RICONOSCENTE!

(...500)

n: ORA CHE LA SUA ENERGIA È A ZERO, PUOI CONTROLLARE LE SUE AZIONI DIRETTAMENTE

`bb({mouth:"smile", eyes:"normal"});`

n: SCEGLI LA TUA MOSSA FINALE

`bb({mouth:"small_lock", eyes:"fear"});`

n: *COLPO DI GRAZIA*

[LOTTA: Punisci il tuo insopportabile telefono!](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[SCAPPA: Rannicchiati in un angolino e piangi!](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Il tuo telefono ti ha provocato un attacco di panico!

`bb({eyes:"anger"})`

b: Zuckerberg e compagnia stanno compromettendo la tua salute mentale per i soldi di qualche finanziatore capitalista!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Punisci il tuo telefono! Distruggilo! Uccidilo!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDI--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Il mondo è pieno di pericoli!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Fai come l'armadillo! Rannicchiati in posizione di auto-difesa!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: RANNICCHIATI RANNICCHIATI RANNICCHIATI RANNICCHIATI RANNICCHIATI RANNICCHIATI RANNICCHIATI RANNIC-- 

(#act1j)

# act1j

`SceneSetup.act1_outro()`