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

s: Ma hai *letto* la "notizia" di quella cosa orribile che è successa?

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

a: Dio, odio le news. Tutto senzionalismo e titoloni acchiappa click.

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

s: Hai ragione, però lo fanno per ottenere incentivi. Il *vero* problema è chi clicca su quei titoli.

```
publish("act2",["dee",3]);
```

s: Chi retwitterebbe mai una notizia così orribile? Tutti ci rimarrebbero male.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, infatti.

(#act2-preamble-end)

# act2-preamble-news2

```
publish("act2",["dee",3]);
```

s: Hai *visto* quanti stanno condividendo quella "notizia"?

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

a: Si, è una bufala. Come fanno a crederci e a condividerla?

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: B... bella festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Sul serio. Cioè, quanto ci vuole ad aprire Google e verificare?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, infatti.

(#act2-preamble-end)

# act2-preamble-cat

```
publish("act2",["dee",3]);
```

s: Dicevo, l'Industria dei Meme sfrutta i gatti.

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: C-ciao...

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

s: Beh, ieri ho visto qualcuno retwittare la GIF di un gatto che beve il latte.

```
publish("act2",["dee",3]);
```

s: I gatti non digeriscono quella ^merda^! Chi retwitterebbe un tale *abuso* sugli animali?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, infatti.

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

h2: C-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Anche se avete avuto il match su Tinder?

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

s: Sì, non capisco! Avrà pensato che fossi un *serial killer* o qualcosa del genere. Che paranoici.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, infatti.

(#act2-preamble-end)

# act2-preamble-hookuphole

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Esatto! Pensano che non sia un buon modo per colmare le loro mancanze.

s: Uff, quanto sei moralista! Apri la mente e poi le gambe!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, infatti.

(#act2-preamble-end)

# act2-preamble-pokemon

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Sì, non capisco! Non era così sexy, ma non era neanche male!

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

n: SECONDO ROUND: _LOTTA!_

[Oh no, tutti ci odiano!](#act2a_social)

[Stavi *sbavando* su quella chioma?](#act2a_perv)

[Dai, parliamo del significato della vita.](#act2a_meaning)

# act2a_social

`bb({eyes:"sad"})`

b: Con quel muso lungo stiamo facendo deprimere tutti quanti!

`bb({eyes:"shock", body:"two_up"})`

b: Stiamo uccidendo l'atmosfera! Emaniamo vibrazioni omicide!

`bb({eyes:"normal", body:"normal"})`

b: Umano, dobbiamo andarcene *adesso*, prima che--

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: È molto più attraente di noi, se anche solo la *guardiamo* poi---

`bb({eyes:"shock", body:"two_up"})`

b: SIAMO DEI PERVERTITI

`bb({body:"normal"})`

b: Siamo dei vermi, viscidi, luridi schifosissimi perv--

```
_.a2_first_danger = 'perv';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2a_meaning

`bb({body:"one_up", eyes:"normal_r"})`

b: Alla fine, possiamo davvero dire *cosa* importa davvero?

`bb({body:"normal", eyes:"sad"})`

b: Contribuire all'umanità? Tutte le grandi opere deperiscono, anche se sei Ramses II. L'amore? Verrà sempre spezzato dalla morte.

`bb({eyes:"sad_r"})`

b: Siamo circondati dalla morte! *Noi* moriremo, *tutti* i nostri cari moriranno.

`bb({eyes:"shock", body:"two_up"})`

b: Cavolo, secondo la Seconda Legge della Termodinamica persino il nostro *universo* morirà!

`bb({eyes:"suspect", body:"normal"})`

b: "La morte ti fa apprezzare la vita"? È come dire che la schiavitù ci permette di apprezzare la libertà!

`bb({body:"one_up"})`

b: "Devi capire qual è il tuo scopo in questa vita"? È esattamente quello che fanno complottari e cospirazionisti!

`bb({eyes:"shock", body:"two_up"})`

b: La vita non ha senso, la morte non ha senso, nemmeno il *senso* ha un senso! Cosa dovrebbe fare una person--

```
_.a2_first_danger = 'meaning';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2b

`bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"suspect"})`

b: Ehi... mi senti?

`bb({eyes:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"shock", mouth:"small_talk", body:"chest", MOUTH_LOCK:true})`

b: *GASP*

`bb({mouth:"small_talk"})`

b: DEVO AVVERTIRTI CHE...

[Sei *ancora* in pericolo!](#act2b_louder)

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

b: Creerai un'epidemia fatale di SINDROME DA MUSO LUNGO

`bb({eyes:"suspect", body:"normal", mouth:"normal"})`

b: Dobbiamo andarcene e rinchiuderci per sempre in una stanza solo con Netflix e cibo a domicilio!
```
_.a2_second_danger = "netflix";
_.a2_attack_2 = "solitudine";
_.a2_hoodie_callback = "quarantena";
```

(#act2c)

# act2b_louder_perv

`bb({eyes:"suspect", body:"two_up", mouth:"normal"})`

b: NON FARE IL PERVERTITO, È CONTRO LA LEGGE!

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

b: Legge sulla Perversione, Sezione 74.5: (1) Chiunque si fissi su (a) quelle spalle muscolose (b) quel culetto rotondo (2) sarà tacciato di essere

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: "UN GRAN PERVERTITO SCHIFOSO"

```
_.a2_second_danger = 'legge';
_.a2_attack_2 = "cattivo";
_.a2_hoodie_callback = "la legge";
```

(#act2c)

# act2b_louder_meaning

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: In realtà, anche se trovassi uno scopo nobile nella vita, rischieresti *comunque* di mandare tutto a quel paese!

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Alfred Nobel voleva la pace e la comprensione tra popoli, quindi decise di rendere più semplice viaggiare.

`bb({eyes:"normal_r"})`

b: Gli serviva qualcosa di economico per creare delle gallerie, perciò ha inventato la dinamite...

`bb({body:"one_up", eyes:"normal"})`

b: ... che venne usata nella prima Guerra Mondiale per UCCIDERE MILIONI DI PERSONE

`bb({body:"two_up", eyes:"shock"})`

b: È L'EFFETTO FARFALLA, UMANO! QUANTE PERSONE STAI UCCIDENDO PROPRIO ORA, SENZA SAPERLO?!

```
_.a2_escond_danger = 'butterfly';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "World War I";
```

(#act2c)

# act2b_different_social

`_.a2_first_choice = "different"`

`bb({eyes:"normal_r", body:"point", mouth:"normal"})`

b: In realtà, sai cosa è peggio di non piacere a nessuno? Piacere a *tutti*.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: Diventare uno di *questi* animali da festa sempre alla ricerca del piacere.

`bb({body:"normal", mouth:"small"})`

b: Una vita superficiale con amici superficiali che non ti conoscono veramente!

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

b: La gente muore di fame *in ogni momento* mentre noi pensiamo a divertirci!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Un saggio una volta disse: "l'unica cosa necessaria affinché il male trionfi è che la gente comune non faccia nulla".

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: NON STIAMO FACENDO NULLA

`bb({mouth:"small"})`

b: IN QUESTO MODO STIAMO AIUTANDO _HITLER_.

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

b: Oh, finalmente riesci a sentirmi!

`bb({eyes:"closed", body:"point"})`

b: DEVO AVVERTIRTI CHE

{{if _.a2_first_choice=="louder"}}
[C'è *ancora* più pericolo!](#act2c_louder)
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

b: In realtà, Netflix e consegne a domicilio non sono sufficienti! Contageremmo anche i ragazzi delle consegne!

`bb({body:"one_up", mouth:"small"})`

b: Dobbiamo trasferirci in qualche eremo e farci consegnare il cibo con i droni!

`bb({body:"two_up", mouth:"normal"})`

b: E poi dovremmo sterilizzare il drone per eliminare i germi della SINDROME DEL MUSO LUNGO

`_.a2_attack_3 = "alone";`

`_.a2_hoodie_callback = "una quarantena";`

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

b: Quello SCHIFOSO PERVERTITO dev'essere condannato a 72 ore di gogna pubblica

b: (a meno che questo non gli piaccia)

`bb({body:"scream_a_1"})`

b: per essere così SCHIFOSO

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "legge";`

(#act2d)

# act2c_louder_butterfly

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: EFFETTO FARFALLA! Stai usando un bicchiere in plastica non bio-degradabile?

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: BAM, PERCOLATI TOSSICI DALLA DISCARICA UCCIDONO UN BAMBINO

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: Stai sudando? Il cuore ti va a mille?

`bb({body:"scream_a_1"})`

b: BAM, DISTRUGGI IL SISTEMA SANITARIO E MILIONI DI PERSONE MUOIONO

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "effetto farfalla";`

(#act2d)

# act2c_louder_zombies

`bb({body:"normal", mouth:"small", eyes:"angry"})`

b: Questi zombie-mangia-piacere verranno da te borbottando:

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: METTI UN LIIIKE. METTI UN LIIIIIKE.

`bb({body:"scream_a_1"})`

b: Poi ti MORDERANNO e ti trasformeranno in un MACHO SENZA CERVELLO e/o in una CAGNA SVAMPITA!

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "zombie";`

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

b: A pensarci bene: *questo edificio* dispone di un rilevatore di monossido di carbonio?!

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: E se ci stessero avvelenando _PROPRIO ADESSO_?

`bb({body:"scream_a_1"})`

b: NON RIUSCIREMMO NEANCHE A VEDERE LA MORTE AVVICINARSI. SEMPLICEMENTE CESSEREMO DI ESISTERE PER SEMP-

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "monossido di carbonio";`

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: E se nel profondo non fossimo *non adatti* ad essere amati, o ad amare?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se qualcosa si fosse rotto irrimediabilmente tanto tempo fa dentro di noi? O magari non è mai esistito?

`bb({body:"scream_a_1"})`

b: AAH SIAMO DIFETTOSI! ROTTI, ROTTI, ROTTI, ROTTI-

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: E se fossimo *marci dentro*?

`bb({body:"one_up", eyes:"sad"})`

b: Gli altri hanno una predisposizione a fare del bene, noi lo facciamo solo se spinti dalla vergogna o dal senso di colpa.

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se fosse nella nostra natura ferire gli altri? E se non potessimo essere *nient'altro* che un peso per coloro che ci sono vicini?

`bb({body:"scream_a_1"})`

b: AAH SIAMO DIFETTOSI! ROTTI, ROTTI, ROTTI, ROTTI-

`_.a2_attack_3 = "bad";`

(#act2d)

# act2c_punch

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Non sono irrazionale. La gente droga *davvero* i drink. Succede veramente.

`bb({eyes:"suspect"})`

b: Umano, ti fa male la testa? Ti senti le gambe molli? Forse stiamo morendo.

`bb({body:"scream_a_1"})`

b: AAAH STIAMO MORENDO! MORENDO MORENDO MORENDO MOREN--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "punch";`

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

b: Evviva, Umano! Sono contento che tu possa sentirmi di nuovo!

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

[Wow. Non attribuiamo storie assurde alle popolazioni indigene](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Anzi, addirittura *è nocivo* per chi ha bassa autostima!

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: La ricerca era ben progettata, lo sperimentatore non era al corrente di chi apparteneva a quale gruppo.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Risultato: se soffri di bassa autostima, ripeterti questo tipo di affermazioni ti fa' sentire *peggio* di quando non dici alcun tipo di affermazioni!

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Wood 2009, Psychological Science. Controllalo pure su Google Scholar, Umano.

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

b: *Devi* iniziare a guardare con umiltà i tuoi difetti per crescere come persona!

`bb({body:"two_up", eyes:"suspect"})`

b: Non basta spruzzare del deodorante in una stanza ammuffita! Coprire i tuoi difetti, a lungo andare, ti rende peggiore.

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: Per fortuna, io, come tuo lupo guardiano, posso avvertirti dei tuoi difetti. E ora--

`bb({body:"scream_b_1"})`

b: TUTTO. É TUTTO SBAGLIATO.

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: I nativi Americani sono delle *persone*, non dei *saggi popoli* a cui attribuire frasi per rendere più _esotici_ i tuoi biscotti della fortuna.

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

h: Sai cosa? Sei *irrazionale*.

h: Tutti sanno che le emozioni sono irrazionali. Specialmente la paura.

`hong({body:"facepalm_2"})`

h: Sei un inutile residuo del processo evolutivo. Come la mia appendice, o il mio dente del giudizio!

`hong({body:"yell", mouth:"yell"})`

h: ^Cazzo^, questa metafora del lupo guardiano è una stupidaggine! Sei soltanto un pugno di sostanze neuro-chimiche del mio cervello.

`hong({body:"cross", mouth:"cross"})`

h: Quindi perché dovrei dare ascolto a un irrazionale, inesistente pezzo di ^merda^ senza valore come te?

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Umano, questo fa davvero male.](#act2e_hurtful)

[Io sono un'emozione. Le emozioni sono legittime.](#act2e_valid)

[Umano, siamo fatti *entrambi* di "sostanze chimiche".](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: Io sono *parte* di te, sai? Quando dici questo ferisci te stesso, in realtà.

`bb({body:"scream_a_1"})`

b: Perché ti fai del male, Umano? SMETTI DI FARTI DEL MALE

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

b: Le tue memorie sono pesi sinaptici, la tua ragione è un insieme di segnali elettrici soggetti a guasti.

`bb({eyes:"normal", body:"normal"});`

b: Quindi se essere solo "sostanze chimiche" rende *me* irrazionale... significa che *tu* sei irrazionale!

`bb({body:"two_up", eyes:"shock"});`

b: E se siamo *entrambi* irrazionali, allora non riusciremo *mai* a capire come essere felici e soddisfatti!

`bb({body:"scream_a_1"})`

b: AAH SIAMO DIFETTOSI! ROTTI, ROTTI, ROTTI, ROTTI-

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

b: Aspetta... stai dicendo che i sentimenti sono legittimi, che dovresti sempre accettare le tue emozioni.

`bb({eyes:"suspect_r"});`

b: Però dici anche che le emozioni sono irrazionali, quindi inaffidabili.

`bb({eyes:"angry"});`

b: Oh mio dio, ci stiamo ingannando da soli!

`bb({body:"scream_a_1"})`

b: CI CIBIAMO DI CONTRADDIZIONI IN MODO DA DIPENDERE DALL'INDUSTRIA DELL'AUTO-AIUTO

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

h: Odio tutto questo. Sto male e questo mi fa *schifo*.

h: Non posso placarti. Non posso ignorarti. Non posso combatterti.

`bb({eyes:"suspect"});`

h: Non importa quanti sforzi faccia, non riesco a sbarazzarmi di--

`bb({body:"cry_1"});`

b: Beh, forse NON DEVI *PER FORZA* SBARAZZARTI DI ME.

`bb({body:"cry_2"});`

b: Come pensi che mi senta *IO*, Umano?

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: Ce la sto mettendo tutta per essere il tuo lupo guardiano, eppure continui a considerarmi un Lupo Cattivo!

b: Quindi io mi sforzo *ancora di più* per avvertirti del pericolo! *Più* pericoli! *Altri* pericoli!

`bb({eyes:"cry_2"})`

b: Non importa quanto io mi impegni, tu credi *ancora* che io sia tuo nemico.

`bb({body:"cry_5"});`

b: Dove sto sbagliando?!

`bb({body:"cry_2"});`

b: Lo *so* che faccio schifo nel mio intento. Ma ci sto *provando*, umano!

`bb({body:"cry_3"});`

b: ...ci sto provando.

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: Non devi seguire i miei avvertimenti, o essere d'accordo con me, non devi neanche *apprezzarmi*.

`bb({eyes:"cry_r_2"});`

b: Vorrei solo... che tu fossi paziente con me.

`bb({eyes:"cry_r_3"});`

b: Vorrei solo che ti sedessi con me per un po', invece di evitarmi, e--

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

r: Sembra che tu sia nel bel mezzo di una lotta con te stesso.

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

h2: Oh, Dio, sono proprio una frana.

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Ehi, non sei solo. Essere ansiosi è una cosa molto comune.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r: Pensa, proprio ieri ho sentito di uno che ha avuto un crollo nervoso e ha scaraventato il telefono a terra!
{{/if}}

{{if _.act1_ending=="flight"}}
r: Pensa che proprio ieri un tipo si è rannicchiato e si messo a piangere davanti a tutti!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Ascolta, so che vuol dire avere quella bestia che ti ronza intorno.

```
publish("act2",["party_hunter",8]);
```

r: Lo sappiamo *tutti*. Ecco perché organizzo feste ogni sabato. Per dimenticarci delle nostre paure e dimenticare quella bestia.

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: ma la mia ansia...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: Non preoccuparti. Io ero come te. Poi ho scoperto un piccolo trucchetto per zittire per sempre quella vocina...

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

r: La mia miscela personale. È un po' più forte di, beh... qualsiasi cosa che potresti comprare legalmente, in effetti.

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

[Non è un buon modo di reagire.](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

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

h: Mmm, che bouquet sopraffino!

h: Un forte sentore di "fatti gli affari tuoi" con un leggero retrogusto di "non voglio sentire niente"!

b: Così non va, umano. Non va bene per niente.

[È *così* che iniziano le dipendenze.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[Lo sapevo che quello stramboide era inaffidabile!](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[E poi, potrebbero esserci delle droghe lì dentro!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`

# act2h_opt1

b: Questo è *effett*--

(#act2h)

# act2h_opt2

b: E poi, tu p--

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

h: Delizioso *e* più economico della terapia!

b: UMANO TI PREGO FERMATI!

h: Eheheheh!

h: Altrimenti *cosa* farai, ^coglione^?

b: Scusami, umano.

b: Mi costringi ad usare il mio ATTACCO SPECIALE

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

h: Continuerai ad abbaiare qualche inutile *parola* per far--

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

h: COSA ^CAZZO^ ERA QUELLO?!

b: Mi dispiace. Dovevo mostrarti le conseguenze.

{{if _.SPECIAL_ATTACK=="harm"}}
h: POTEVO *VEDERE* IL MIO STESSO CADAVERE. *PERCEPIRE* LA SENSAZIONE DI ESSERE VERAMENTE MORTO.
{{/if}}

{{if _.SPECIAL_ATTACK=="alone"}}
h: POTEVO *VEDERE* L'ORRORE E IL DISGUSTO DI TUTTI. *SENTIRE* TUTTO CIÒ CHE DICEVANO.
{{/if}}

{{if _.SPECIAL_ATTACK=="bad"}}
h: POTEVO *SENTIRE* LO SCRICCHIOLARE DELLE OSSA. *ANNUSARE* IL SANGUE NELL'ARIA.
{{/if}}

b: Mi dispiace, umano.

n: FINISCILO

[LOTTA: Prendi a pugni quella stramboide.](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[SCAPPA: Vai via da qui.](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: Quella psicopatica si stava approfittando di te.

b: Stava cercando di corromperti per farti diventare come lei.

`bb({ body:"yell_angry_1" });`

b: Prendila a pugni! Mandala al tappeto!

`bb({ body:"final_1" });`

b: COLPISCI COLPISCI COLPISCI COLPISCI COLPISCI COLPISCI COLPISCI COLPISCI COLP--

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: Lo *sapevo*, tutti questi festaioli sono veramente disturbati. Cercano di soffocare il dolore con delle cose orribili!

`bb({ body:"yell_1" });`

b: Stavano cercando di farti fare la stessa fine! Ti stavano corrompendo! Dobbiamo andare via!

`bb({ body:"final_1" });`

b: VIA VIA VIA VIA VIA VIA VIA VIA VIA VIA VIA VIA VIA VIA VIA VIA VIA VI--

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

r: Tutto bene?

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

r: un *peperino*.

r: Mi piace. Vieni alla mia festa sabato prossimo, tesoro.

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: ok ciao, bye bye, adios, au revoir

r: La bestia ha vinto la battaglia per oggi, ma se torni e ti farò bere qualcosa di un po' più forte.

h2: sayōnara, auf wiedersehen, zài jiàn, shalom

r: Io e te faremo vedere a quella bestia chi comanda!

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h2: ok scusa devo andare.

`publish("act2",["party_hunter",16]);`

r: Maledizione. La bestia ha avuto la meglio, eh?

`publish("act2",["party_hunter",15]);`

h2: No, no. Devo fare una maratona, devo andarmene. E di corsa, anche.

`publish("act2",["party_hunter",19]);`

r: Vieni alla mia festa sabato prossimo, ti offro qualcosa di ancora più farte.

h2: ok grazie adesso devo correre correre correre

r: Io e te faremo vedere a quella bestia chi comanda!

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

b: Umano! Tutto bene?!

```
publish("act2", ["act2_end","next"]);
```

b: Fiuu, ci siamo andati *vicino*. Abbiamo rischiato davvero--

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

h: Il prossimo weekend ci torniamo.

h: La prossima volta che ci scontreremo non mi limiterò a farti *perdere*...

h: Ti *ucciderò*, brutto b^astardo^.

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
