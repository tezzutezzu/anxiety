# act2

`SceneSetup.act2();`

{{if _.badnews && !_.factcheck}}
(#act2-preamble-news1)
{{/if}}

{{if _.badnews && _.factcheck}}
(#act2-preamble-news2)
{{/if}}

{{if _.catmilk}}
(#act2-preamble-cat)
{{/if}}

(#act2-preamble-tinder)


# act2-preamble-news1

```
publish("act2",["dee",3]);
```

s: Ma hai *letto* quella notizia riguardo quella cosa orribile successa da qualche parte?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: C-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Dio odio i notiziari. Tutto senzionalismo e clickbait.

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: b-bella festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Vero, ma sono solo alla ricerca di incentivi. Il *vero* problema sono le persone che ci cliccano su quei titoli.

```
publish("act2",["dee",3]);
```

s: Chi condividerebbe mai una notizia del genere facendo star male tutti i propri amici?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh... vero, no?

(#act2-preamble-end)


# act2-preamble-news2

```
publish("act2",["dee",3]);
```

s: Ma hai *letto* quella "notizia" che sta diventando virale?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: c-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Sì, completamente falsa. Mi domando come faccia la gente a crederci e a condividerla...

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: b... bella festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Sul serio. Dai, ci sei? Almeno googla per fare fact-checking?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh... vero, no?

(#act2-preamble-end)


# act2-preamble-cat

```
publish("act2",["dee",3]);
```

s: Come stavo dicendo, l'Impianto Industriale Memetico sfrutta i gatti.

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: c-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Elabora un po' questa tua tesi.

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: b-bella festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Beh, ho visto qualcuno ritwittare una GIF di un gatto che beveva latte ieri.

```
publish("act2",["dee",3]);
```

s: Non digeriscono quella ^merda^! Chi ritwitterebbe *maltrattamenti su animale* in quel modo?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, vero no?

(#act2-preamble-end)


# act2-preamble-tinder

```
publish("act2",["dee",1]);
```

s: E quindi sì, non ha mai risposto!

```
publish("act2",["dee",0]);
publish("act2",["party_hong","next"]);
```

h2: c-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Anche se eravate compatibili su Tinder?

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: b-bella festa...

```
publish("act2",["party_hong","next"]);
```

{{if _.serialkiller}}
(#act2-preamble-serialkiller)
{{/if}}

{{if _.hookuphole}}
(#act2-preamble-hookuphole)
{{/if}}

{{if _.pokemon}}
(#act2-preamble-pokemon)
{{/if}}

# act2-preamble-serialkiller

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Eh si! Non so, magari pensavano fossi un *serial killer* o qualcosa del genere. Che paranoici.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, vero no?

(#act2-preamble-end)


# act2-preamble-hookuphole

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Ma che ne so, forse pensano che rimorchiare qualcuno non possa riempire il vuoto nel loro cuore?

s: Finiscila di fare il santarellino! Apri la mente, poi apri le cosce!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, vero no?

(#act2-preamble-end)


# act2-preamble-pokemon

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Boh! Non era così figo poi, ma sarebbe stata una bella chiappata!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Gotta Catch 'Em All!™

(#act2-preamble-end)


# act2-preamble-end

```
Game.clearText();
publish("act2-out-1");
music(null, {fade:1});
```

(...3000)

```
music('battle', {volume:0.5});
publish("hp_show");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

n: ROUND TWO: *FIGHT!*

[Oh no, tutti ci odiano!](#act2a_social)

[Stavi *sbavando* sul pel di carota?](#act2a_perv)

[Dai, parliamo del significato della vita.](#act2a_meaning)

# act2a_social

`bb({eyes:"sad"})`

b: Stiamo affliggendo tutti con la nostra seriosità!

`bb({eyes:"shock", body:"two_up"})`

b: Stiamo uccidendo l'atmosfera! Siamo degli assassini di atmosfere di primo grado!

`bb({eyes:"normal", body:"normal"})`

b: Umano, dobbiamo andarcene, *ora*. Prima che--

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: È molto più attraente di noi, che significa che se solo *guardiamo*, poi---

`bb({eyes:"shock", body:"two_up"})`

b: SIAMO DEI VISCIDONI

`bb({body:"normal"})`

b: Siamo dei vermi, dei viscidi, dei terribili, luridi schifosissimi perv--

```
_.a2_first_danger = 'perv';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2a_meaning

`bb({body:"one_up", eyes:"normal_r"})`

b: Alla fine, cosa possiamo fare che abbia sia davvero d'impatto?

`bb({body:"normal", eyes:"sad"})`

b: Contribuire all'umanità? Tutte le grandi opere deperiscono allo stesso modo di Osimandia. L'amore? Sarà sfaldato dalla morte.

`bb({eyes:"sad_r"})`

b: E quanta morte c'è attorno a noi! *Noi* moriremo. *Tutti i nostri cari* moriranno.

`bb({eyes:"shock", body:"two_up"})`

b: Cavolo, la Seconda Legge della Termodinamica dice che persino il nostro *universo* morirà!

`bb({eyes:"suspect", body:"normal"})`

b: Oh, "la morte ci fa apprezzare la vita"? È come dire che la schiavitù è buona perché ci fa apprezzare la libertà!

`bb({body:"one_up"})`

b: Oh, "sei tu che devi creare il significato della tua vita"? Questo è quello che i cultisti e i cospirazionisti fanno!

`bb({eyes:"shock", body:"two_up"})`

b: La vita non ha senso, la morte non ha senso, persino il *senso* non ha senso! Cosa dovrebbe fare un mortale--

```
_.a2_first_danger = 'meaning';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2b

`bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"suspect"})`

b: Um... mi puoi sentire, umano?

`bb({eyes:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"shock", mouth:"small_talk", body:"chest", MOUTH_LOCK:true})`

b: *GASP*

`bb({mouth:"small_talk"})`

b: DEVO AVVERTIRTI CHE...

[C'è *ancora* pericolo!](#act2b_louder)

{{if _.a2_first_danger=="social"}}
[C'è un *altro* pericolo sociale!](#act2b_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[C'è un *altro* pericolo morale!](#act2b_different_moral)
{{/if}}

[Stai ignorando il pericolo! È pericoloso!](#act2b_ignore)

# act2b_louder

`_.a2_first_choice = "louder"`

{{if _.a2_first_danger=="social"}}
(#act2b_louder_social)
{{/if}}

{{if _.a2_first_danger=="perv"}}
(#act2b_louder_perv)
{{/if}}

{{if _.a2_first_danger=="meaning"}}
(#act2b_louder_meaning)
{{/if}}

# act2b_louder_social

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: LE EMOZIONI SONO CONTAGIOSE! SE NON TE NE VAI INFETTERAI TUTTI CON LA TUA MALATTIA MENTALE!

b: Creerai un'epidemia fatale della SINDROME DEL TRISTONE

`bb({eyes:"suspect", body:"normal", mouth:"normal"})`

b: Dobbiamo uscire di qui ed andare in quarantena per sempre in una piccola stanza con Netflix e consegne di cibo a domicilio!

```
_.a2_second_danger = "netflix";
_.a2_attack_2 = "solitudine";
_.a2_hoodie_callback = "quarantena";
```

(#act2c)

# act2b_louder_perv

`bb({eyes:"suspect", body:"two_up", mouth:"normal"})`

b: NON FARE IL VISCIDO, È CONTRO LA LEGGE!

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: Legge sul Viscidume, Sezione 74.5: (1) Tutte le persone che continuano a guardare (a) quelle spalle muscolose (b) quel culetto delizioso (2) saranno tacciate di essere

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: "DEI GRAN PERVERTITI SCHIFOSI"

```
_.a2_second_danger = 'law';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "the law";
```

(#act2c)

# act2b_louder_meaning

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: Veramente, anche se hai un nobile scopo nella tua vita, puoi *comunque* continuare a incasinare tutto!

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Alfred Nobel voleva la pace nel mondo e che i popoli si capissero a vicenda. Quindi decise di rendere più facile viaggiare

`bb({eyes:"normal_r"})`

b: Quindi aveva bisogno di creare in modo poco costoso le gallerie per i treni. Quindi ha inventato una cosa chiamata "dinamite"....

`bb({body:"one_up", eyes:"normal"})`

b: che fu usata nella prima Guerra Mondiale per UCCIDERE MILIONI DI PERSONE

`bb({body:"two_up", eyes:"shock"})`

b: È L'EFFETTO FARFALLA, UMANO! QUANTE PERSONE STAI INVOLONTARIAMENTE UCCIDENDO ORA?

```
_.a2_escond_danger = 'butterfly';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "World War I";
```

(#act2c)

# act2b_different_social

`_.a2_first_choice = "different"`

`bb({eyes:"normal_r", body:"point", mouth:"normal"})`

b: In realtà, sai cosa è peggio dell'essere rifiutato dagli altri? Piacere a *tutti*.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: Ovvero, diventare uno di *questi* animali da festa sempre alla ricerca del piacere.

`bb({body:"normal", mouth:"small"})`

b: Una vita superficiale con amici superficiali che ti conoscono solo in modo superficiale!

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Umano, scappiamo da questi zombi ricerca-piacere prima che ci trasformino in uno di loro!

```
_.a2_second_danger = 'zombies';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "zombies";
```

(#act2c)

# act2b_different_moral

`_.a2_first_choice = "different"`

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: La gente muore di carestie e genocidi *in questo momento* e noi siam qui a far festa!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Un saggio una volta disse: "l'unica cosa necessaria affinché il male trionfi è che le brave persone non facciano nulla."

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: NON STIAMO FACENDO NULLA

`bb({mouth:"small"})`

b: FACENDO FESTA, STIAMO AIUTANDO *HITLER*.

```
_.a2_second_danger = 'hitler';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "Hitler";
```

(#act2c)

# act2b_ignore

`_.a2_first_choice = "ignore"`

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Pensi di essere al sicuro solo perché hai tolto le batterie al rilevatore di monossido di carbonio?

`bb({eyes:"suspect_r"})`

b: Non sentirai neanche l'odore del gas! Semplicemente ti addormenterai e--

`bb({body:"scream_c_1"})`

b: MORIRAIIIIIIIII

```
_.a2_second_danger = 'ignore';
_.a2_attack_2 = "harm";
_.a2_hoodie_callback = "carbon monoxide";
```

(#act2c)

# act2c

```
hong({body:"ignore_sweat"});
bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true});
```

b: ...

`bb({eyes:"happy", mouth:"smile", body:"chest"})`

b: Oh grazie a Dio, credo tu possa sentirmi di nuovo!

`bb({eyes:"closed", body:"point"})`

b: DEVO AVVERTIRTI CHE

{{if _.a2_first_choice=="louder"}}
[C'è *ancora* pericolo!](#act2c_louder)
{{/if}}

{{if _.a2_first_choice!="louder"}}
[C'è *ancora* pericolo!](#act2c_louder)
{{/if}}

{{if _.a2_first_danger=="social"}}
[C'è un *altro* pericolo sociale!](#act2c_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[C'è un *altro* pericolo morale!](#act2c_different_moral)
{{/if}}

[Hai controllato il drink prima di berlo?](#act2c_punch)

#act2c_louder

{{if _.a2_second_danger=="netflix"}}
(#act2c_louder_netflix)
{{/if}}

{{if _.a2_second_danger=="law"}}
(#act2c_louder_law)
{{/if}}

{{if _.a2_second_danger=="butterfly"}}
(#act2c_louder_butterfly)
{{/if}}

{{if _.a2_second_danger=="zombies"}}
(#act2c_louder_zombies)
{{/if}}

{{if _.a2_second_danger=="hitler"}}
(#act2c_louder_hitler)
{{/if}}

{{if _.a2_second_danger=="ignore"}}
(#act2c_louder_ignore)
{{/if}}

# act2c_louder_netflix

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: In realtà, Netflix e consegne a domicilio non sono abbastanza! Infetteremo anche quelli delle consegne!

`bb({body:"one_up", mouth:"small"})`

b: Dobbiamo trasferirci in qualche eremo e farci consegnare il cibo coi droni!

`bb({body:"two_up", mouth:"normal"})`

b: E poi dovrebbero far sterilizzare i droni per eliminare i germi della SINDROME DEL TRISTONE

`_.a2_attack_3 = "alone";`

`_.a2_hoodie_callback = "a quarantine";`

(#act2d)

# act2c_louder_law

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: Il GRAN VISCIDO PERVERTITO sarà condannato a 72 ore in uno di quei dispositivi di umiliazione pubblica medievali.

b: a meno che le gogne non lo *eccitino*

`bb({body:"scream_a_1"})`

b: perché sono dei GRAN VISCIDI PERVERTITI

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the law";`

(#act2d)

# act2c_louder_butterfly

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: EFFETTO FARFALLA! Stai usando dei bicchieri di plastica non bio-degradabili?

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: BAM, PERCOLATI TOSSICI DALLA DISCARICA UCCIDONO UN BAMBINO

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: Stai sudando e ti sta scoppiando il cuore?

`bb({body:"scream_a_1"})`

b: BAM, DISTRUGGI IL SISTEMA SANITARIO NAZIONALE E MILIONI DI PERSONE MUOIONO

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the butterfly effect";`

(#act2d)

# act2c_louder_zombies

`bb({body:"normal", mouth:"small", eyes:"angry"})`

b: Questi zombi ricerca-piacere barcolleranno verso di te borbottando,

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: METTI UN MI PIAAACEEE, METTI UN MI PIAAACEEE

`bb({body:"scream_a_1"})`

b: Poi ti MORDERANNO e ti trasformeranno in uno MACHO SENZACERVELLO e/o una CAGNA SVAMPITA!

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "zombies";`

(#act2d)

# act2c_louder_hitler

`bb({body:"scream_a_1"})`

b: I NAZI SONO RITORNATI A MARCIARE SULLE STRADE

`bb({body:"one_up", mouth:"smile", eyes:"happy"})`

b: Dicendo *meno male che quelle 'brave persone' scansafatiche si stanno 'rilassando' e 'prendendo cura di sé'!*

`bb({body:"point", mouth:"smile", eyes:"happy_r"})`

b: *

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "Hitler";`

(#act2d)

# act2c_louder_ignore

`bb({body:"normal", mouth:"normal", eyes:"normal_r"})`

b: Ora che ci penso, sappiamo se questo palazzo *ha* un rilevatore di monossido di carbonio?

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: E se ci stessero avvelenando *IN QUESTO MOMENTO*?

`bb({body:"scream_a_1"})`

b: NON RIUSCIREMMO NEANCHE A VEDERE LA MORTE AVVICINARSI. SEMPLICEMENTE CESSEREMO DI ESISTERE PER SEMP-

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "carbon monoxide";`

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: E se fossimo *basilarmente incapaci* di essere amati, o di amare?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se qualcosa si fosse rotto irreversibilmente tanto tempo fa dentro di noi? O non fosse mai esistito?

`bb({body:"scream_a_1"})`

b: AAH NON STIAMO BENE! STIAMO A PEZZI, A PEZZI, A PEZZI!

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: E se fossimo *fondamentalmente marci*?

`bb({body:"one_up", eyes:"sad"})`

b: Gli altri almeno hanno una predisposizione a fare del bene, noi quando facciamo del "bene" solo perché ci vergognamo o ci sentiamo in colpa.

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se fosse nella nostra natura ferire gli altri? E se non potessimo essere *nient'altro* che un peso per coloro che ci sono vicini?

`bb({body:"scream_a_1"})`

b: AAH NON STIAMO BENE! STIAMO A PEZZI, A PEZZI, A PEZZI!

`_.a2_attack_3 = "bad";`

(#act2d)

# act2c_punch

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Non sono irrazionale. La gente droga i drink *per davvero*. Questa è una cosa che succede.

`bb({eyes:"suspect"})`

b: Umano, ti fa male la testa? Ti senti le gambe molli? Penso che stiamo morendo.

`bb({body:"scream_a_1"})`

b: AHHH STIAMO MORENDO! MORENDO MORENDO MORENDO MOREN--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "punch bowls";`

(#act2d)

# act2d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"attacked"});
attack("20p", _.a2_attack_1);
```

(...401)

```
hong({body:"attacked_2"});
attack("20p", _.a2_attack_2);
```

(...401)

```
hong({body:"attacked_3"});
attack("20p", _.a2_attack_3);
```

(...1001)

h: C^AAACCHI^O!

h: C^ACCHI^O C^ACCH^ISSIMO *C^AAACCHIOO^O*

`bb({body:"two_up", mouth:"smile", eyes:"happy"});`

b: Evviva Umano! Sono così felice che tu mi senta di nuovo!

`bb({body:"normal", mouth:"small", eyes:"sad"})`

b: Perché mi stavi ignorando?

`hong({body:"facepalm"})`

h: Dio santo, brutto imbecille.

`hong({body:"facepalm_2"})`

h: Conosci quella storia dei nativi americani?

h: "Ci sono due lupi dentro di te, uno è la speranza, l'altro è la disperazione. Quale lupo vince? Quello a cui dai da mangiare."

```
hong({body:"facepalm_3"});
bb({eyes:"normal"});
```

h: Stavo cercando di *farti morire di fame* sadica testa di ^cazzo^.

`hong({body:"smile", mouth:"smile"})`

h: Chi se ne frega, mi concentrerò sul pensiero positivo.

h: *Io ho amore. Io ho valore. Io ho intelligenza. Io ho bellezza. Io sono speciale.*

`bb({eyes:"suspect"});`

[Accidenti, che narcisismo!](#act2d_narcissist)

[Sai che il pensiero positivo è stato *confutato?*](#act2d_disproven)

[Oddio, non attribuire storielle a caso alle popolazioni indigene](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Anzi, addirittura è *nocivo* per le persone con bassa autostima!

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: È stato stabilito da uno studio scientifico ben strutturato, con un trial in cui lo sperimentatore non era al corrente di chi fosse in quale gruppo.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Risultato: se soffri di bassa autostima, ripeterti questo tipo di affermazioni ti fa sentire *peggio* che se non dicessi proprio niente!

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Wood 2009, Psychological Science. Controllalo pure su Google Scholar, umano,

`bb({body:"scream_b_1"})`

b: ALLORA SMETTILA DI DIFFONDERE DISINFORMAZIONE

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_narcissist

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Hai *bisogno* di prendere atto umilmente dei tuoi stessi difetti per poter crescere come persona!

`bb({body:"two_up", eyes:"suspect"})`

b: Non puoi semplicemente spruzzare deodorante in una stanza ammuffita! Nascondere i tuoi difetti, a lungo andare, ti renderà una persona peggiore.

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: Per fortuna, io, come tuo leale lupo da guardia, posso avvertirti dei tuoi difetti. E in questo momento, è--

`bb({body:"scream_b_1"})`

b: TUTTO. TUTTO È SBAGLIATO.

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: I nativi Americani sono delle *persone reali*, non dei "buoni selvaggi" che puoi buttare in una conversazione per rendere il tuo consiglio da biscotto della fortuna più *esotico*.

`bb({eyes:"suspect_r"})`

b: Stai riducendo persone con un'identità e culture complesse a degli slogan da cartolina! Questo è "razzismo benevolo"!

`bb({body:"scream_b_1"})`

b: FINISCILA DI ESSERE RAZZISTA, CRETINO STRABICO

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2e

h: ^PORCA MISERIA^

`hong({body:"yell", mouth:"yell"})`

h: Sai cosa? Tu sei *irrazionale*.

h: Tutti sanno che le emozioni sono irrazionali! Specialmente la paura!

`hong({body:"facepalm_2"})`

h: Sei un inutile scarto del processo evolutivo, come l'appendice o i denti del giudizio!

`hong({body:"yell", mouth:"yell"})`

h: ^Cazzo^, tutta questa metafora del lupo da guardia è una stupidaggine! Sei solo un pugno di sostanze neuro-chimiche nella mia testa.

`hong({body:"cross", mouth:"cross"})`

h: Quindi perché dovrei dare ascolto a un misero, irrazionale, inesistente pezzo di ^merda^ come te?!

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Cristo, Umano. Questo fa davvero male.](#act2e_hurtful)

[Io sono un sentimento. I sentimenti hanno valore.](#act2e_valid)

[Umano, siamo *entrambi* "solo sostanze chimiche."](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: Io sono *parte* di te, sai. Quando dici certe cose, ferisci *te*.

`bb({body:"scream_a_1"})`

b: Perché ti fai del male, umano? SMETTI DI FARTI DEL MALE.

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2e_rational

`bb({body:"normal", mouth:"normal", eyes:"normal_r"});`

b: Le tue più recondite motivazioni sono dopamina, le tue gioie più grandi sono serotonina.

`bb({body:"one_up"});`

b: Le tue memorie sono pesi sinaptici, la tua ragione sono segnali elettrici soggetti a guasti.

`bb({eyes:"normal", body:"normal"});`

b: Quindi se il mio essere "solo sostanze chimiche" significa che *io* sono irrazionale... allora questo significa che *tu* sei irrazionale!

`bb({body:"two_up", eyes:"shock"});`

b: E se siamo tutt'e due *irrazionali*, allora non riusciremo *mai* a capire come raggiungere la completezza e la felicità!

`bb({body:"scream_a_1"})`

b: AAAH STIAMO A PEZZI! A PEZZI, A PEZZI, A PEZZI--

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2f)

# act2e_valid

`bb({body:"normal", mouth:"normal", eyes:"suspect"});`

b: Un attimo... "loro" dicono che i sentimenti hanno valore, che dovresti sempre accettare le tue emozioni.

`bb({eyes:"suspect_r"});`

b: Ma "loro" dicono anche che le emozioni sono irrazionali, che non ci si può fidare delle emozioni.

`bb({eyes:"angry"});`

b: Oh cavolo, "loro" ci hanno mentito per tutto il tempo!

`bb({body:"scream_a_1"})`

b: "LORO" CI NUTRONO DI CONTRADDIZIONI PER RENDERCI DIPENDENTI DAL COMPLESSO INDUSTRIALE DELL'AUTO-AIUTO

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2f

`hong({body:"defeated", MOUTH_LOCK:true});`

h: ...

h: Odio tutto questo. Dio se fa male, *odio* tutto questo.

h: Non posso placarti. Non posso ignorarti. Non posso combatterti.

`bb({eyes:"suspect"});`

h: Non importa quanti sforzi faccia, non riesco a sbarazzarmi di--

`bb({body:"cry_1"});`

b: Beh, forse NON *DOVRESTI* SBARAZZARTI DI ME.

`bb({body:"cry_2"});`

b: Come pensi che *IO* mi senta, umano?!

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: Ce la sto mettendo tutta per essere il tuo lupo da guardia, ma tu continui a vedermi come il Lupo Cattivo!

b: Quindi io mi sforzo *ancora di più* per avvertirti del pericolo! *Più* pericoli! *Altri* pericoli!

`bb({eyes:"cry_2"})`

b: Ma non importa quanto io mi impegni, tu credi *comunque* che io sia tuo nemico.

`bb({body:"cry_5"});`

b: Dove sto sbagliando?!

`bb({body:"cry_2"});`

b: Lo *so* che faccio schifo come lupo da guardia. Ma ci sto *provando*, umano!

`bb({body:"cry_3"});`

b: ...ci sto provando.

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: Non devi seguire i miei avvertimenti, o essere d'accordo con me, non devi neanche *apprezzarmi*.

`bb({eyes:"cry_r_2"});`

b: Io... Tutto ciò che voglio è che tu sia paziente con me.

`bb({eyes:"cry_r_3"});`

b: Voglio solo che tu ti sieda con me per un po', invece di allontanarti e--

```
bb({eyes:"cry_r_4"});
hong({body:"listen"});
```

r: Ehi.

```
hong({body:"look"});
Game.clearText();
publish("act2-in-2");
publish("hp_hide");
music('party1', {volume:0.4, fade:2});
```

(...2000)

```
publish("act2",["party_hunter",2]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Sembra che tu sia nel bel mezzo di una lotta interiore.

```
publish("act2",["party_hunter",3]);
publish("act2",["party_hong",13]);
```

h2: Era così ovvio?

```
publish("act2",["party_hunter",4]);
publish("act2",["party_hong",14]);
```

r: Stavi, ehm, parlottando con la tua felpa di {{_.a2_hoodie_callback}} o qualcosa del genere.

```
publish("act2",["party_hunter",13]);
publish("act2",["party_hong",15]);
sfx("rustle", {volume:0.6});
setTimeout(function(){
	publish("act2",["party_hong",16]);
	sfx("concrete_step3", {volume:0.6});
},401);
setTimeout(function(){
	publish("act2",["party_hong",17]);
	sfx("concrete_step4", {volume:0.6});
},801);
```

h2: Oddio, sono un disastro...

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Ehi, mica solo tu. L'ansia è super-comune.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r: Diamine, proprio ieri ho sentito che qualcuno del campus ha avuto un esaurimento nervoso e ha distrutto il proprio telefono!
{{/if}}

{{if _.act1_ending=="flight"}}
r: Diamine, proprio ieri ho sentito che qualcuno si è appallottolato tipo armadillo e si messo a piangere in pubblico!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Ascolta, so che vuol dire avere quell'animale in testa.

```
publish("act2",["party_hunter",8]);
```

r: *Tutti* lo sappiamo. Ecco perché do una festa ogni weekend: per dimenticare le nostre paure, dimenticare quell'animale.

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: Ma la mia ansia...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: Non preoccuparti. Io ero come te. Poi ho trovato un piccolo trucchetto per zittire quella voce negativa per sempre...

```
publish("act2",["party_hunter",3]);
Game.clearText();
music(null, {fade:1});
```

(...2001)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",22]);
sfx("rustle");
```

(...2501)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",23]);
sfx("rustle2");
```

(...1001)

```
publish("act2",["party_hunter",11]);
```

r: La mia miscela personale. È un po' più forte di... beh, di qualsiasi cosa sia legale, veramente.

```
publish("act2",["party_hunter",12]);
publish("act2",["party_hong",24]);
```

r: Alla goccia, raga!

```
hong({body:"hold"});
bb({body:"normal", mouth:"small", eyes:"wat"});
Game.clearText();
Game.WORDS_HEIGHT_BOTTOM = -1;
publish("act2-out-3");
publish("hp_show");
```

(...3500)

[Oddio.](#act2g_1) `Game.OVERRIDE_CHOICE_LINE=true`

[Questo non è un buon modo di reagire.](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

[Non accettare drink dagli sconosciuti.](#act2g_3) `Game.OVERRIDE_CHOICE_LINE=true`

# act2g_1

b: O--

(#act2g)

# act2g_2

b: L--

(#act2g)

# act2g_3

b: N--

(#act2g)

# act2g

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"forward", mouth:"forward"});
bb({body:"frazzled", mouth:"frazzled", eyes:"frazzled"});
```

h: Mmm, che bouquet sopraffino!

h: Un forte sentore di "chiudi il becco, voce nella testa" con un leggero retrogusto di "non sentire mai più nulla"!

b: Questo è male, umano. Molto, molto male.

[È *esattamente* così che iniziano le dipendenze.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[Lo *sapevo* che l'ospite era un vero caso umano!](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[E poi ci potrebbero essere delle droghe lì dentro!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`

# act2h_opt1

b: Questo è *davv*--

(#act2h)

# act2h_opt2

b: E poi loro potr--

(#act2h)

# act2h_opt3

b: Lo *sapevo* ch--

(#act2h)

# act2h

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"back", mouth:"back"});
bb({body:"panicked", mouth:"panicked", eyes:"panicked"});
```

h: Delizioso, *e* più economico della terapia!

b: UMANO TI PREGO FERMATI

h: Hehehe!

h: Altrimenti *tu* cosa farai, ^coglione^?

b: Sono desolato, umano.

b: Dovrò usare il mio ATTACCO SPECIALE

```
bb({body:"special_a"});
music('battle', {volume:0.5});
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act2h_attack) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act2h_attack) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act2h_attack) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`

# act2h_attack

```
bb({body:"special_b_1"});
hong({body:"forward", mouth:"forward"});
sfx("charging");
```

h: Cos'è questa ^merda^?

h: Continuerai ad abbaiare stupide *parole* per far--

```
bb({body:"special_c"});
sfx("hadouken");
```

(...901)

(#act2i)

# act2i

```
publish("hide_tabs");
publish("show_special_attack");
Game.FORCE_CANT_SKIP = true;
music(null);
stopAllSounds();
```

(...5000)

```
publish("show_tabs");
hong({ body:"final", mouth:"final" });
bb({ body:"normal", mouth:"normal", eyes:"sad" });
attack("100p", _.SPECIAL_ATTACK);
Game.FORCE_CANT_SKIP = false;
setTimeout(function(){
	publish("remove_special_attack");
},30);
```

(...2500)

h: COSA ^CAZZO^ ERA QUELLO

b: Mi dispiace. Dovevo mostrarti le conseguenze.

{{if _.SPECIAL_ATTACK=="harm"}}
h: POTEVO *VEDERE* IL MIO STESSO CADAVERE. POTEVO *SENTIRE* DAVVERO LA MIA MORTE.
{{/if}}

{{if _.SPECIAL_ATTACK=="alone"}}
h: POTEVO *VEDERE* LO SGUARDO DISGUSTATO DELLA GENTE. POTEVO *SENTIRE* TUTTO CIÒ CHE DICEVANO.
{{/if}}

{{if _.SPECIAL_ATTACK=="bad"}}
h: POTEVO *SENTIRE* LO SCRICCHIOLARE DELLE COSTOLE. POTEVO *ASSAPORARE* IL SANGUE NELL'ARIA.
{{/if}}

b: Mi dispiace, umano.

n: *COLPO DI GRAZIA*

[LOTTA: Dai un pugno all'ospite.](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[SCAPPA: Vattene da qui.](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: Quell'essere spregevole si stava approfittando di te.

b: Stava cercando di corromperti, di farti piombare nei suoi stessi casini.

`bb({ body:"yell_angry_1" });`

b: Prendi a pugni quell'imbecille! Si merita una scarica di botte!

`bb({ body:"final_1" });`

b: A PUGNI A PUGNI A PUGNI A PUGNI A PUGNI A PUGNI A PUGNI A PUGN--

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: Lo *sapevo* che tutti questi festaioli erano incasinati di brutto. Cercano di attenuare il loro dolore con delle cose orribili.

`bb({ body:"yell_1" });`

b: E stavano cercando di farti fare la stessa fine! Ti stanno corrompendo! Dobbiamo andare via!

`bb({ body:"final_1" });`

b: VAI VIA VAI VIA VAI VIA VAI VIA VAI VIA VAI VIA VAI VIA VAI VIA VAI VIA VAI VIA VAI VIA--

`_.a2_ending = "flight";`

(#act2k)

# act2k

```
Game.clearText();
publish("act2-in-4");
publish("hp_hide");
music('party1', {volume:0.6, fade:1.5});
```

(...2001)

```
publish("act2",["party_hong",26]);
sfx("slide");
```

(...1001)

```
publish("act2",["party_hunter",14]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Tutto bene, tesoro?

`publish("act2",["party_hunter",13]);`

{{if _.a2_ending=="fight"}}
(#act2k_fight)
{{/if}}

{{if _.a2_ending=="flight"}}
(#act2k_flight)
{{/if}}

# act2k_fight

```
Game.clearText();
publish("act2",["party_hunter",21]);
publish("act2",["party_hong",33]);
music(null);
sfx("hit");
```

(...1000)

```
sfx("record_scratch");
publish("act2",["party_hunter",22]);
publish("act2",["party_hong",34]);
publish("act2",["dee",6]);
publish("act2",["dum",6]);
```

r: S-sei...

```
publish("act2",["party_hunter",23]);
publish("act2",["party_hong",35]);
publish("act2",["dee",5]);
publish("act2",["dum",5]);
music('party1', {volume:0.6, fade:6});
```

r: *intrigante*.

r: Mi piace. Vieni alla mia festa il prossimo weekend, bellezza.

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: ok ciao, bye bye, adios, au revoir

r: L'animale potrà anche aver vinto oggi, ma tu torna e preparerò per te qualcosa di ancora più forte!

h2: sayōnara, auf wiedersehen, zài jiàn, shalom

r: Io e te, tesoro, faremo vedere a quella bestia chi comanda!

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h2: ok scusa devo scappare.

`publish("act2",["party_hunter",16]);`

r: Maledizione. L'animale ha vinto oggi, eh?

`publish("act2",["party_hunter",15]);`

h2: no no, io, ehm, devo fare una maratona. E di corsa.

`publish("act2",["party_hunter",19]);`

r: Vieni alla mia festa il prossimo weekend, bellezza. Preparerò per te qualcosa di ancora più forte.

h2: ok grazie adesso devo correre correre correre

r: Io e te, tesoro, faremo vedere a quella bestia chi comanda!

(#act2k_end)

# act2k_end

```
Game.clearText();
publish("act2-out-5");
publish("act2-outro", ["end1"]);
music("hum", {fade:2, volume:0.6});
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2500)

```
publish("act2", ["act2_end",2]);
sfx("whoosh");
```

(...1000)

b: Umano! Stai bene?!

```
publish("act2", ["act2_end","next"]);
```

b: Fiuu, per un *pelo.* Avremmo potuto davvero--

```
Game.clearText();
publish("act2", ["act2_end","next"]);
music(null);
sfx("squeak");
```

(...1500)

```
publish("act2", ["act2_end","next"]);
sfx("hit");
```

(...1000)

h: Il prossimo weekend ci torno a quella festa.

h: E la prossima volta che lotteremo, non mi limiterò a *sconfiggerti*...

h: Io ti *ammazzerò*, ^cazzo^.

```
Game.clearText();
publish("act2", ["act2_end","next"]);
sfx("concrete_step1");
```

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step2", {volume:0.8});
```

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step3", {volume:0.5});
```

(...901)

`sfx("concrete_step4", {volume:0.25});`

(...3000)

`_.INTERMISSION_STAGE = 2;`

(#intermission)