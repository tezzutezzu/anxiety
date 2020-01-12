# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Alla salute!

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *Ah* senti come va giù.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: Sai, tesoro...


```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: Per esser precisi, va giù proprio tra l'amigdala destra e quella sinistra.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Mi ricordi di quando ero giovane. Di quando la bestia tormentava anche me.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: Sono riconoscente di poter fare lo stesso con te, aiutarti ad uccidere la bestia come ho fatto io.

```
publish("act3",["roofhunter",2]);
```

r: Giochiamo a "veritá o penitenza", cosa preferisci?

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: PENITENZA!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Haha! Va bene.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Ok. La vedi quella piscina azzurro pastello là sotto?


```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Sì? Sei piani sotto?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Saltaci.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Aspetta, che?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: La bestia ha iniziato a lamentersi, non é vero?

```
publish("act3",["roofhunter",23]);
```

r: *O nooooo! É pericoloso! Non farlo!*

```
publish("act3",["roofhunter",22]);
```


r: Ed ecco perché abbiamo bisogno di sfiorare la morte! Spassatela! Carpe diem! Sniffa coca dal ^culo^ di un bel bocconcino, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: Mostra a quella bestia che non ce ne frega un  *^cazzo* dei suoi piagnistei! Salta!

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Uh, ma qualche volta, um... la paura ha senso...

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: Scusami, credi davvero a quella commercialata della "mindfulness" e su quanto fa *bene* sentirsi uno schifo?

```
publish("act3",["roofhunter",17]);
```

r: Il piacere è il contrario del dolore. Quindi, ^cazzo^, puoi usare il piacere per sconfiggere il dolore!

```
publish("act3",["roofhunter",18]);
```

r: Come fanno quegli pseudo-buddisti della Silicon Valley a non capire questa ^stronz^ata?

```
publish("act3",["roofhunter",6]);
```

r: Tesoro, so che *tu* sai che quell'animale *ferisce* quelli come noi. *Tortura* quelli come noi.

```
publish("act3",["roofhunter",19]);
```

r: Non è nostro amico. È una bestia rabbiosa che deve essere *sedata*.

```
publish("act3",["roofhunter",20]);
```

r: O beccarsi un *proiettile nel cranio*.

```
publish("act3",["roofhunter",27]);
```

r: Altrimenti la lascerai vincere.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: No. Ti sbagli.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: Non la lascerò vincere.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: ^Cazzo^ sì! Credo in te, baby! Uccidila!

(#act3a)



# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: no no no no no no

n: QUESTO CAPITOLO HA DUE POSSIBILI FINALI. UNO È *DAVVERO, DAVVERO BRUTTO.*

b: NO NO NO NO NO NO NO NO NO NO NO NO NO NO

n: SCEGLI SAGGIAMENTE. PROTEGGI IL TUO UMANO.

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAAH

`bb({ mouth:"normal" });`

n: BUONA FORTUNA

```
Game.clearText();
bb({ eyes:"start" });
```

[Umano, qui puoi veramente MORIRCI!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[Questo è stupido ed autodistruttivo!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Questi squilibrati non sono davvero tuoi amici!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: U--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Q--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Q--

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Sai, avrei potuto crederti... se questa non fosse la milionesima volta che ci provi.

h: Sei il lupo che ha gridato "al lupo, al lupo".

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`


# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Ci hai già provato anche così.

b: Umano, per favore...

`hong({ eyes:"look_right" });`

h: Oh mi *dispiace* che Big Pharma non approvi la mia cura fai-da-te.

h: Senti, testa di ^cazzo^, abbiamo *tutti* un modo per farti chiudere quella ^fottuta^ bocca.

`hong({ body:"look_up", eyes:"look_up" });`

h: Alcuni si buttano sul lavoro.

`hong({ body:"look_down", eyes:"look_down" });`

h: Altri si buttano nel sesso, nella droga o nel aggiornare di continuo la pagina di Facebook.

`hong({ body:"normal", eyes:"look_right" });`

h: Altri ancora si gettano tra le braccia di qualcuno.

`hong({ eyes:"angry" });`

h: Io mi lancerò in quella piscina.

[Hai bevuto troppo e sono SEI PIANI!](#act3_bad_1_harm)

[Maledizione, questo è il tuo ringraziamento?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Ok, lo ammetto. Ho fatto un casino.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Anche se tu cadessi in acqua, l'impatto con la superficie ti spaccherebbe le costole ed otterresti una commozione cerebrale, *come minimo!*

h: Eh.

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Una volta ho visto un ragazzo russo farlo su YouTube.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: C-chiedo scusa, il *ringraziamento?*

`bb({ eyes:"angry" });`

b: È proprio per questo che *esisto!* Gli umani non sono in grado di proteggersi da soli!

b: Ho provato a salvare le tue stupide chiappe per tutta la vita ed adesso vuoi b--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: heh.

`hong({ body:"laugh_2" })``

h: hahahaha

`hong({ body:"laugh_3" })``

h: HAHAHAHAHAHA

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: Oh WOW, questo è il più grande ^fottuto^ *eufemismo* del secolo!

`hong({ body:"yell_2" });`

h: Esatto, brutto ammasso di ^merda^ rossa! Hai fatto un ^cazzo^ di casino!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Altro da dichiarare, Capitan Ovvio?

[Però vendicarti di me non è la risposta!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Però *questa* volta ho ragione!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Ti ho fatto del male.](#act3_good_2a)


# act3_good_1_fail_revenge

b: Devi imparare e relazionarti in modo sano con le tue emozioni, invece di annegarle n--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)



# act3_good_1_fail_harm

b: Quindi, per favore, metti giù la bottiglia e poi--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)




# act3_bad_2

`bb({ eyes:"sad" });`

b: per favore... non farlo...

h: La tua energia è schifosamente bassa, lupo.

h: Fossi in te, sceglierei le prossime parole molto attentamente.

`bb({ eyes:"normal" });`

[Benissimo. La pianto di proteggerti.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Ho sempre avuto ragione.](#act3_bad_2_right)

[Mi dispiace.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: Allora vai, buttati. Non me ne frega.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: E va bene. Alla goccia.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: ASPETTA QUELLA ERA PSICOLOGIA INVERSA DOVEVI FARE IL *CONTRARIO* DI QUELLO CHE TI STAVO DICEND-

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: Ti *stai* ficcando nei guai. I tuoi cosiddetti amici ti *stanno* usando. E *tu* stai usando i tuoi cosiddetti amici.

`bb({ eyes:"sad" });`

b: Quindi dai, umano... perché non mi credi?!

h: perché non hai mai creduto in *me*.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Gli altri lupi da guardia hanno umani che si prendono il tempo di addestrarli con pazienza, per *imparare* a cooperare.

b: Piuttosto che odiare i lupi da guardia che hanno provato a proteggerli! Quindi non potresti sol--

`bb({ eyes:"normal" });`

h: Risposta ^fottutame^nte sbagliata.

(#act3_bad_3)



# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *"L’unica cosa che dobbiamo temere è proprio la paura."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Don't worry, be happy!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Le menti illuminate del nostro tempo concordano: le emozioni negative sono *brutte!*

`hong({ eyes:"less_angry" });`

h: Ma va?! È per questo che si chiamano *negative!*

b: Umano... per favore...

`hong({ eyes:"normal" });`

h: Tempo fa dissi: "vorrei solo liberarmi di tutto questo dolore."

h: Il mio desiderio è stato esaudito. Non sento più dolore, paura o ansia...

h: Non sento più nulla.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Assicurarmi che nulla ti facesse del male era diventata un'ossessione tale che non ho realizzato di essere *IO* a creare quel male.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: MA. NON. MI. DIRE.

`hong({ body:"yell_1" });`

h: CRISTO. Ce ne hai messo di tempo per arrivarci!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Avresti potuto risparmiarci così tanti casini, stupida palla di pelo. Perché non l'hai capito prima?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...ti *dispiace.*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: Ti dispiace per *cosa*?

(#act3_good_2q)


# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized)
{{/if}}


# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[Mi dispiace di non essere stato un buon difensore.](#act3_good_3_protector)

[Mi dispiace di non averti portato rispetto.](#act3_good_3_respect)

[Mi dispiace.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Mi dispiace di avere un umano terribile!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Mi dispiace di non averti portato rispetto.](#act3_good_3_respect)

[Mi dispiace di averti fatto del male.](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: È mio dovere metterti in guardia dei pericoli *reali*, ma ho continuato ad abbaiare alle macchine ed al postino.

`bb({eyes:"sorry_up"});`

b: Abbaiare alle ombre. Abbaiare così tanto.

`bb({eyes:"sorry"});`

b: Capisco perché volessi mettermi la museruola.

`bb({eyes:"sorry_down"});`

b: Mi dispiace.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: Dovevo essere il *tuo* fedele cane da guardia, ma ho finito per comportarmi come se fossi tu a dover obbedire a *me*.

`bb({eyes:"sorry_up"});`

b: C'è differenza tra l'essere un difensore ed un secondino, ed io ho passato il segno.

`bb({eyes:"sorry_down"});`

b: Mi dispiace.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Provare a proteggerti era un'ossessione tale che non ho mai frenato per riflettere sul fatto che ero *io* a ferirti.

`bb({eyes:"sorry_up"});`

b: Ero un cane cattivo.

`bb({eyes:"sorry_down"});`

b: Mi dispiace.

(#act3_good_4)


# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: Beh, sì, comunque era un'idea del cavolo.

h: L'ho fatto solo per incasinarti e, beh, obiettivo raggiunto.

h: Diciamo che stavolta siamo pari, ok?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Ok.

h: Ok.

n: *PAREGGIO*

`_.a3_ending = "walkaway";`

(#act3_end)









# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}






# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: Oh *ma per favore*. Dopo tutto ciò che quell'animale ti ha fatto, ti *arrendi* così?

r: Cosa c'è, tesoro? Hai *paura?*

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Sì.

h2: Ho paura.

`publish('hong-next')`

h2: E va bene così.

`publish('hong-next')`

h2: È giusto avere paura.

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: Ma hanno chiuso a chiave?

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)




# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```
(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: no...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: no no no

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: NO!

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
