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

a: Dio odio le news. Tutto senzionalismo e titoloni acchiappa click.

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

s: Chi spargerebbe mai una notizia del genere e far star male tutti i propri amici?

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

s: Ma hai *letto* quella notizia che si sta spargendo?

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

a: Si, completamente falsa. Mi domando come fa la gente a crederci e a condividerla...

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: n... bella festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Sul serio. Dai, ci sei? Ameno fare qualche ricerca per verificarla?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, vero?

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

s: I gatti non digeriscono quella ^merda^ di latte! Chi ritwitterebbe un tale *abuso* sugli animali?

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

s: Eh si, non ha mai risposto!

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

a: Anche se avete avuto entrambi un match su Tinder?

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

s: Finiscila di fare il santarellino! Apri la mente...e poi apri le cosce!

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

s: Boh! Non era così figo poi, ma sarebbe stata una bella preda!

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

[Stavi *fissando* la rossa?](#act2a_perv)

[Dai, parliamo del significato della vita.](#act2a_meaning)

# act2a_social

`bb({eyes:"sad"})`

b: Stiamo affliggendo tutti con la nostra seriosità!

`bb({eyes:"shock", body:"two_up"})`

b: Stiamo ammazzando l'atmosfera! Siamo degli assassini di atmosfere di primo grado!

`bb({eyes:"normal", body:"normal"})`

b: Umano, dobbiamo andarcene, *ora*. Prima che--

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: È molto più attraente di noi, che significa che se solo la *guardiamo* poi---

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

b: Alla fine, possiamo davvero dire *cosa* importa davvero?

`bb({body:"normal", eyes:"sad"})`

b: Contribuire all'umanità? Tutte le grandi opere deperiscono allo stesso modo di Osimandia. L'amore? Sarà sfaldato dalla morte.

`bb({eyes:"sad_r"})`

b: E quanta morte c'è attorno a noi! *Noi* moriremo. *Tutti i nostri cari* moriranno.

`bb({eyes:"shock", body:"two_up"})`

b: Cavolo, secondo la Seconda Legge della Termodinamica persino il nostro *universo* morirà!

`bb({eyes:"suspect", body:"normal"})`

b: Oh, "la morte ci fa apprezzare la vita"? È come dire che la schiavitù è buona perché ci fa apprezzare la libertà!

`bb({body:"one_up"})`

b: Oh, "sei tu che devi creare il significato della tua vita"? Questo è proprio quello che i complottari e i cospirazionisti fanno!

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

b: Dobbiamo andare in quarantena per sempre in una piccola stanza con Netflix e consegne di cibo a domicilio!

```
_.a2_second_danger = 'netflix';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "a quarantine";
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

b: Alfred Nobel voleva la pace nel mondo e che i popoli si capissero l'un l'altro. Quindi decise di facilitare le persone a viaggiare

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

b: In realtà, sai cosa è peggio dell'essere rifiutato dagli altri? Essere popolare per *tutti*.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: Ovvero, diventare uno di *questi* animali da festa sempre alla ricerca del piacere.

`bb({body:"normal", mouth:"small"})`

b: Una vita superficiale con amici superficiali che hanno ti conoscono solo in modo superficiale!

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

b: La gente sta morendo di fame *in questo momento* e noi semplicemente, facciamo festa!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Un saggio una volta disse: "l'unica cosa necessaria affinché il male trionfi è che la gente comune non faccia nulla."

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

b: Pensi che sei al sicuro solo perché hai tolto le batterie al rilevatore di monossido di carbonio?

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

b: Oh finalmente, sembra che tu possa sentirmi di nuovo!

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

b: In realtà, Netflix e consegne a domicilio non è abbastanza! Infetteremo anche i ragazzi delle consegne!

`bb({body:"one_up", mouth:"small"})`

b: Dobbiamo trasferirci in qualche eremo e farci consegnare il cibo coi droni!

`bb({body:"two_up", mouth:"normal"})`

b: E poi dovremmo sterilizzare i droni per eliminare i germi della SINDROME DEL TRISTONE

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

b: Il GRAN VISCIDO PERVERTITO  sarà condannato a 72 ore di gogna

b: (a meno che le gogne non lo eccitino)

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

b: Poi ti MORDERANNO e ti trasformeranno in uno MACHO SENZACERVELLO e/o una CAGNA SVAMPITA

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "zombies";`

(#act2d)

# act2c_louder_hitler

`bb({body:"scream_a_1"})`

b: I NAZI SONO RITORNATI A MARCIARE SULLE STRADE

`bb({body:"one_up", mouth:"smile", eyes:"happy"})`

b: Dicendo *meno male che quelle 'brave persone' scansafatiche si stanno 'rilassando' e 'prendendo cura di sé'!*

`bb({body:"point", mouth:"smile", eyes:"happy_r"})`

b: *Ora i nostri piani possono proseguire, appena in tempo!*

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "Hitler";`

(#act2d)

# act2c_louder_ignore

`bb({body:"normal", mouth:"normal", eyes:"normal_r"})`

b: A pensarci, sappiamo se *questo palazzo* ha un rilevatore di monossido di carbonio

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: E se ci stessero avvelenando *IN QUESTO MOMENTO*?

`bb({body:"scream_a_1"})`

b: NON RIUSCIREMMO NEANCHE A VEDERE LA MORTE AVVICINARSI. SEMPLICEMENTE CESSEREMO DI ESISTERE PER SEMP-

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "carbon monoxide";`

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: E se fossimo essenzialmente *incapaci* di essere amati, o di amare?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se qualcosa si fosse rotto irreversibilmente tanto tempo fa dentro di noi? O magari non è mai esistito?

`bb({body:"scream_a_1"})`

b: AAH NON STIAMO BENE! STIAMO A PEZZI, A PEZZI, A PEZZI! 

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: E se fossimo essenzialmente *marci*?

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

h: C^AAAAZZO^!

h: C^AZZ^O C^AZZO^-C^AZZ^O *C^AAAAZZZO^*

`bb({body:"two_up", mouth:"smile", eyes:"happy"});`

b: Evviva Umano! Sono contento che puoi sentirmi di nuovo!

`bb({body:"normal", mouth:"small", eyes:"sad"})`

b: Perché mi stavi ignorando?

`hong({body:"facepalm"})`

h: Dio santo, imbecille.

`hong({body:"facepalm_2"})`

h: Conosci la storia dei nativi americani?

h: "Ci sono due lupi dentro di te, uno è la speranza, l'altro è la disperazione. Quale lupo vince? Quello a cui dai da mangiare."

```
hong({body:"facepalm_3"});
bb({eyes:"normal"});
```

h: Stavo cercando di *farti morire di fame* grande sadica testa di ^cazzo^.

`hong({body:"smile", mouth:"smile"})`

h: Chi se ne frega. Mi concentro sul pensiero positivo.

h: *Io sono amato. Io sono buono. Io sono intelligente. Io sono bello. Io sono speciale.*

`bb({eyes:"suspect"});`

[Accidenti, che narcisismo!](#act2d_narcissist)

[Sai che il pensiero positivo è stato *confutato?*](#act2d_disproven)

[Wow. Per piacere non attribuire assurde storie folcloristiche alle popolazioni indigene](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Anzi, addirittura *è nocivo* per le persone con bassa autostima!

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: È stato stabilito da uno studio scientifico serio, nell'esperimento lo sperimentatore non era al corrente a quale gruppo appartenevano gli esaminati.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Risultato: se soffri di bassa autostima, ripeterti questo tipo di affermazioni ti fa' sentire *peggio* di quando non dici alcun tipo di affermazioni!

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Wood 2009, Psychological Science. Controllalo pure so Google Scholar, umano

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

b: *Devi* umilmente constatare le tue limitazioni se vorrai crescere come persona!

`bb({body:"two_up", eyes:"suspect"})`

b: Non puoi semplicemente spruzzare del deodorante in una stanza ammuffita! Coprire i tuoi difetti, a lungo andare, renderà le cose peggiori.

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: Per fortuna, io, come tuo lupo da guardia, posso avvertirti dei tuoi difetti. E ora--

`bb({body:"scream_b_1"})`

b: TUTTO. TUTTO É SBAGLIATO.

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: I nativi americami sono delle *persone*, non dei *selvaggi buoni* che puoi buttare in una conversazione per rendere il tuo consiglio da Bacio Perugina più *esotico*.

`bb({eyes:"suspect_r"})`

b: Stai riducendo persone e culture complesse a degli slogan da cartolina! Questo è vero e proprio razzismo bonario.

`bb({body:"scream_b_1"})`

b: FINISCILA DI ESSERE RAZZISTA, STUPIDO SECCHIONE.

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

h: Sai cosa? *TU* sei irrazionale.

h: Tutti sanno che le emozioni sono irrazionali. Specialmente la paura.

`hong({body:"facepalm_2"})`

h: Sei un inutile residuo del processo evolutivo. Come la mia appendice, o il mio dente del giodizio!

`hong({body:"yell", mouth:"yell"})`

h: ^Cazzo^, persino questa metafora del lupo da guardia è una stupidaggine! Sei soltanto un pugno di sostanze neuro-chimiche all'interno del mio cervello.

`hong({body:"cross", mouth:"cross"})`

h: Quindi perché dovrei dare ascolto a un irrazionale, non esistente pezzo di ^merda^ senza valore come te?

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Umano, mi stai facendo davvero del male.](#act2e_hurtful)

[Io sono un'emozione e le emozioni hanno senso.](#act2e_valid)

[Umano, siamo *entrambi* "un pugno di sostanze chimiche."](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: Io sono *parte* di te, sai? Quando dici questo, sta in realtà facendo male a te stesso. 

`bb({body:"scream_a_1"})`

b: Perché ti fai del male, umano? SMETTI DI FARTI DEL MALE

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

b: Quindi se l'essere "solo sostanze chimiche" significa essere irrazionale...beh allora questo significa che *irrazionale* lo sei anche tu!

`bb({body:"two_up", eyes:"shock"});`

b: E se siamo entrambi *irrazionali*, allora non riusciremo *mai* a capire come fare ad essere soddisfatti e felici!

`bb({body:"scream_a_1"})`

b: AAH NON STIAMO BENE! STIAMO A PEZZI, A PEZZI, A PEZZI! 

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

b: Aspetta... "loro" dicono che i sentimenti sono validi, allora dovresti sempre accettare le tue emozioni. 

`bb({eyes:"suspect_r"});`

b: Ma "loro" dicono anche che le emozioni sono irrazionali, che non ci si può fidare delle emozioni.

`bb({eyes:"angry"});`

b: O mio dio, "loro" ci hanno ingannato tutto il tempo!

`bb({body:"scream_a_1"})`

b: "LORO" CI CIBANO DI CONTRADDIZIONI PER RENDERCI DIPENDENTI DALL'INDUSTRIA DELL'AUTO-AIUTO

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

h: Odio tutto questo. Sto male e *odio* tutto questo.

h: Non posso placarti. Non posso ignorarti. Non posso combatterti.

`bb({eyes:"suspect"});`

h: Non importa quanti sforzi faccia, non riesco a sbarazzarmi di--

`bb({body:"cry_1"});`

b: Beh, forse NON *DOVRESTI* SBARAZZARTI DI ME.

`bb({body:"cry_2"});`

b: Come pensi che *IO* mi senta, umano?

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: Ce la sto mettendo tutta per essere il tuo lupo da guardia, ma tu continui a vedermi come il Gran Lupo Cattivo!

b: Quindi io mi sofrzo *ancora di più* per avvertirti del pericolo! *Più* pericoli! *Altri* pericoli!

`bb({eyes:"cry_2"})`

b: Ma non importa quanto io mi impegni, tu credi *ancora* che io sia tuo nemico.

`bb({body:"cry_5"});`

b: Dove sto sbagliando?!

`bb({body:"cry_2"});`

b: Lo *so* che faccio schifo come lupo da guardia. Ma ci sto *provando*, umano!

`bb({body:"cry_3"});`

b: ...ci sto provando.

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: Non devi seguire i miei avvertimenti, o essere d'accordo con me, non devi neanche *apprezzarmi*.

`bb({eyes:"cry_r_2"});`

b: Tutto quello che voglio...è che tu sia paziente con me.

`bb({eyes:"cry_r_3"});`

b: Vuoi solo che tu ti sieda con me per un po', invece di guardare dall'altro lato e--

```
bb({eyes:"cry_r_4"});
hong({body:"listen"});
```

r: Ehi..

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

r: Sembra che tu stia nel bel mezzo di una lotta con te stesso, ragazzo.

```
publish("act2",["party_hunter",3]);
publish("act2",["party_hong",13]);
```

h2: Era così ovvio?

```
publish("act2",["party_hunter",4]);
publish("act2",["party_hong",14]);
```

r: Eh, stavi parlando da solo di {{_.a2_hoodie_callback}} o qualcosa del genere.

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

h2: ho dio, 

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Ehi, non sei solo. Essere ansiosi è una cosa molto diffusa.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r: Pensa che proprio ieri ho sentito di uno che ha avuto un esaurimento nervoso e ha scaraventato il telefono al suolo!
{{/if}}

{{if _.act1_ending=="flight"}}
r: Pensa che proprio ieri un tipo si è rannicchiato e si messo a piangere in pubblico!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Ascolta, so che vuol dire avere quell'animale in testa.

```
publish("act2",["party_hunter",8]);
```

r: *Tutti* lo sappiamo. Ecco perché dò una festa ogni weekend. Per dimenticarci delle nostre paure e dimenticare quell'animale.

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: ma la mia ansia...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: Non preoccuparti. Io ero come te. Poi ho trovato un piccolo trucchetto per zittire quella voce negativa...

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

r: La mia miscela personale. È un po' più forte di...beh tutto quello che puoi comprare legalmente in effetti.

```
publish("act2",["party_hunter",12]);
publish("act2",["party_hong",24]);
```

r: Alla salute ^beell-lla^!

```
hong({body:"hold"});
bb({body:"normal", mouth:"small", eyes:"wat"});
Game.clearText();
Game.WORDS_HEIGHT_BOTTOM = -1;
publish("act2-out-3");
publish("hp_show");
```

(...3500)

[O. Mio. Dio.](#act2g_1) `Game.OVERRIDE_CHOICE_LINE=true`

[Questo non è un buon modo di reagire.](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

[Non accettare drink dagli sconosciuti.](#act2g_3) `Game.OVERRIDE_CHOICE_LINE=true`

# act2g_1

b: O--

(#act2g)

# act2g_2

b: T--

(#act2g)

# act2g_3

b: D--

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

h: Mmm, what an exquisite palette!

h: A full-bodied flavor of "shut your mind up," with a subtle aftertaste of "never feel anything ever again"!

b: This is bad, human. This is really, really bad.

[This is *actually* how addiction starts.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[I *knew* the host was deeply messed up!](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[Also, they could have drugged that!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`


# act2h_opt1

b: This is *actu*--

(#act2h)

# act2h_opt2

b: Also, they co--

(#act2h)

# act2h_opt3

b: I *knew* th--

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

h: Delicious, *and* cheaper than therapy!

b: HUMAN PLEASE STOP

h: Hehehe!

h: And what are *you* gonna do about it, ^asshole^?

b: I'm so sorry, human.

b: I'm going to have to use my SPECIAL ATTACK

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

h: What's this ^crap^?

h: You're gonna yap more stupid *words* at me to--

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

h: WHAT THE ^HELL^ WAS THAT

b: I'm sorry. I needed to show you the consequences.

{{if _.SPECIAL_ATTACK=="harm"}}
h: I COULD *SEE* MY OWN CORPSE. I COULD *FEEL* THE SENSATION OF BEING ACTUALLY DEAD.
{{/if}}

{{if _.SPECIAL_ATTACK=="alone"}}
h: I COULD *SEE* EVERYONE'S LOOK OF DISGUST. I COULD *HEAR* ALL THE THINGS THEY SAID.
{{/if}}

{{if _.SPECIAL_ATTACK=="bad"}}
h: I COULD *HEAR* THE CRUNCHING OF RIBS. I COULD *TASTE* THE BLOOD IN THE AIR.
{{/if}}

b: I'm sorry, human.

n: *FINISH THEM*

[{FIGHT: Punch the host.}](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[{FLIGHT: Let's get out of here.}](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: That psychopath was taking advantage of you.

b: They were trying to corrupt you, make you as messed up as they are!

`bb({ body:"yell_angry_1" });`

b: Punch that jerk! Knock their friggin' lights out!

`bb({ body:"final_1" });`

b: PUNCH THEM PUNCH THEM PUNCH THEM PUNCH THEM PUNCH THEM PUNCH THEM PUNCH THEM PUNCH THE--

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: I *knew* all these partygoers were deeply messed up. They all dull their pain with horrible things!

`bb({ body:"yell_1" });`

b: And they're tricking you into doing the same thing! They're corrupting you! We need to get out!

`bb({ body:"final_1" });`

b: GET OUT GET OUT GET OUT GET OUT GET OUT GET OUT GET OUT GET OUT GET OUT GET OU--

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

r: You alright, kid?

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

r: Y-you...

```
publish("act2",["party_hunter",23]);
publish("act2",["party_hong",35]);
publish("act2",["dee",5]);
publish("act2",["dum",5]);
music('party1', {volume:0.6, fade:6});
```

r: are *kinky*.

r: I like that. Come to my party next weekend, cutie.

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: ok bye, ciao, adios, au revoir

r: The animal might have won today, but come back, and I'll mix something even stronger for you!

h2: sayōnara, auf wiedersehen, zài jiàn, shalom

r: You and me, kid, we'll show that beast who's boss!

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h2: ok sorry i have to run

`publish("act2",["party_hunter",16]);`

r: ^Damn^ it. The animal won today, huh?

`publish("act2",["party_hunter",15]);`

h2: no no, just, uh, gotta run a marathon. gotta go fast.

`publish("act2",["party_hunter",19]);`

r: Come to my party next weekend, cutie. I'll mix something even stronger for you.

h2: ok thanks gonna run run run run run

r: You and me, kid, we'll show that beast who's boss!

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

b: Human! Are you okay?!

```
publish("act2", ["act2_end","next"]);
```

b: Gosh, that was *close.* We really could've--

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

h: I'm coming back to the party next weekend.

h: The next time we fight, I'm not just going to *defeat* you...

h: I'm going to ^fuck^ing *kill* you.

```
Game.clearText();
publish("act2", ["act2_end","next"]);
sfx("concrete_step1");
````

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