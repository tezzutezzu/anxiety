# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (game auto-saved)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *sigh*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Quindi quale ^diavolo^ è la morale della storia?

`hong({body:"one_up", eyes:"annoyed"})`
  
h: Che cosa abbiamo *imparato*? Io sono stato stupido, i miei "amici" mi hanno usato, e siamo quasi *morti*.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Si, per non parlare delle spese mediche.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Si, per non parlare dei danni al fegato.](#act4a_liver)
{{/if}}

[Si, quello *era* il peggiore dei casi.](#act4a_worst)

[Si, avevo ragione.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Già. Non penso l'assicurazione copra "essere un ^imbecille^".

`hong({eyes:"annoyed", mouth:"normal"});`

b: Eppure... siamo sopravvissuti!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Di sicuro ci abbiamo rimesso qualche anno di vita...

`bb({eyes:"surprise"});`

b: Almeno ce *l'abbiamo* ancora una vita! Siamo sopravvissuti!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: Eppure...

h: Hm?

`bb({eyes:"surprise"});`

b: Siamo sopravvissuti!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Ma... avevi ragione pure tu.

`hong({eyes:"surprise"});`

h: Hm?

`bb({eyes:"normal"});`

b: Ero *io* il lupo che gridava "al lupo". E quando il pericolo era *reale*, tu – giustamente – non mi hai creduto.

`bb({eyes:"surprise_r"});`

b: Eppure, siamo sopravvissuti!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Nonostante tutto, siamo ancora qui.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: Sembri abbastanza calmo considerando che abbiamo visto la morte in faccia.
{{/if}}

{{if !_.INJURED}}
h: Sembri abbastanza calmo considerando che abbiamo *quasi* visto la morte in faccia.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Beh, rende tutto il resto meno preoccupante a confronto. Mi ha anche fatto riflettere.

`bb({eyes:"normal", mouth:"normal"});`

b: Se litigare con te non ti sta bene perché non ti fa sentire protetto

h: E *inoltre* non ti sta bene perché ti fa solo urlare di piu'...

`bb({eyes:"normal_r"})`

b: Allora forse...

`bb({eyes:"normal"})`

h: Forse non dobbiamo litigare.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: Non sono il Lupo Cattivo, ma non sono neanche un lupo da guardia.

`bb({eyes:"sad_d"})`

b: Sono un cane randagio malconcio.

`bb({eyes:"sad"})`

b: Abbiamo passato dei brutti momenti. Forse trauma o abbandono. Per questo a volte esagero e faccio:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: YAP YAP YAP YAP YAP

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Ma non *voglio* essere un cane codardo! Voglio proteggerti! Voglio essere un bravo cane!

`bb({eyes:"sad", mouth:"normal"});`

b: Umano... mi aiutarai ad addomesticare questo lupo?

`hong({eyes:"sad"})`

h: Ci... ci proverò.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Okay. Un rapporto sano con le emozioni. I rapporti hanno bisogno di comunicazione. Quindi, comunichiamo.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: I prossimi cinque minuti saranno super sdolcinati, ma proviamoci finché non ci riusciamo.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Caro lupo interiore...*Tu* come stai?

n2: NUMERO DI PAURE USATE:

n2: *FERITO* {{_.attack_harm_total}}, *NON AMATO* {{_.attack_alone_total}}, *CATTIVO* {{_.attack_bad_total}}

n2: DI QUALE PAURA VUOI PARLARE PRIMA? (POSSIAMO PARLARE DELLE ALTRE DOPO)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Ho paura di essere ferito.](#act4_harm)

[Ho paura di rimanere da solo.](#act4_alone)

[Ho paura di essere una cattiva persona.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Voglio proteggere il tuo bisogno di incolumità fisica,

`bb({eyes:"sad_d"})`

b: Ma il *mondo intero* sembra così pericoloso. Pieno di tragedie e cattiveria.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: Non so, ne ho abbastanza di decidere *io* cosa dire. *Tu* cosa hai da dire, umano?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Tocca di nuovo a te, umano. Che ne pensi?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Altri pensieri, umano?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Hai ragione. Ci dobbiamo proteggere.](#act4_harm_skills)

[Esponiamoci a *più* pericoli.](#act4_harm_exposure)

[Grazie.](#act4_thanks) `_.thanks_for = "physical safety";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Ma... come? Io ho zanne e artigli, ma sono solo una metafora.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Potremmo imparare auto-difesa? Unirci ad un gruppo che si protegge a vicenda? Migliorare la nostra salute e limiti?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Forse, ma...

[E da dove iniziamo?](#act4_harm_skills_start)

[E se neanche questo funziona?](#act4_harm_skills_work)

[E se esageriamo con la "sicurezza"?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: C'è cosi tanto da fare, tante cose che dobbiamo correggere. Da dove iniziamo?

`hong({ body:"shrug", eyes:"surprise" })`

h: Iniziamo adesso.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Eh?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Ci stiamo esercitando a comunicare in questo momento. Ciò ci aiuterá a percepire il pericolo con meno falsi positivi,

`hong({ eyes:"surprise" });`

h: E questo ci aiuterá a proteggerci dal dolore!

`hong({ eyes:"normal", mouth:"normal" });`

h: Perciò: questo *è* un corso di auto-difesa.

`bb({ eyes:"normal_r" })`

b: Huh. Mi aspettavo piú di questo:

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: Vero, non c'é modo di proteggerci al 100%...

`hong({ body:"one_up" });`

h: Ma anche un miglioramento dell'1% vale la pena, giusto?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Vedi il bicchiere non come vuoto al 99%, ma come pieno all'1%?

`bb({ eyes:"normal" });`

h: Che é ancora un bene prezioso, se sei bloccato in mezzo al deserto.

`bb({ eyes:"closed" });`

b: Beh. Alla goccia, allora.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Voglio dire, la ragione per cui hai ignorato i miei avvertimenti é perché ho esagerato con la sicurezza! 

`bb({ body:"normal", eyes:"normal" })`

h: Nah, hai ragione. Vorremmo pensare alla sicurezza con moderazione. Tutto con moderazione.

`bb({ eyes:"suspect" })`

b: Scusa, *TUTTO* con moderazione?

`hong({ eyes:"annoyed" })`

h: *Un numero moderato di cose* con moderazione.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Grazie per aver reso le tue dichiarazioni ricorsivamente autoconsistenti.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *COSA*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Voglio dire, diciamo che un cane ha paura dei tuoni.

`hong({ body:"hands_1" });`

h: Un trucco usato dagli addestrattori é fargli ascoltare un tuono a basso volume mentre gli danno dei premi per tenerli calmi.

`hong({ body:"hands_2" });`

h: Nei giorni successivi, l'addestratore inizia ad alzare il volume, fino a quando il cane non ha più paura.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Si chiama terapia espositiva!

`hong({ body:"point", eyes:"normal" });`

h: Dato che sei un cane dovrebbe funzionare, giusto? Tutti i mammiferi hanno lo stesso istinto di sopravvivenza.

`hong({ body:"normal" });`

[E se ci desensibilizziamo *troppo*?](#act4_harm_exposure_overboard)

[E se ci esponiamo a del *vero* pericolo?](#act4_harm_exposure_hurt)

[Sono un lupo, non un cane.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: E ti mostrerò gentilezza e pazienza fino ad addomesticarti fino a farti diventare un cucciolotto.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Aww.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: Abbiamo appena visto cosa succede quando ignori le tue paure, metti te stesso in *serio* pericolo.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Comunque, *troppa* desensibilizzazione non ci fará diventare psicopatici?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Si e presto inizieremo persino a darci dei premi mentre guardiamo dei porno snuff!

`hong({ eyes:"annoyed" })`

h: ...penso ci sia una gran differenza tra quello e il tuono.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Esattamente *quale*, umano? *Quale?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: Non so, ma *tu* mi puoi aiutare!

`hong({ eyes:"normal", body:"normal" })`

h: Lavorando e parlando insieme, faremo dei piani per trovare una soluzione.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Okay. Ma io non sono così bravo a pianificare, quello dovrai farlo tu

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: Per esempio: ci siamo buttati giu da un cavolo di *tetto!*
{{/if}}

{{if !_.INJURED}}
b: Per esempio: ci siamo quasi buttati giu da un cavolo di *tetto!*
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Nah, hai ragione. Uno *può* esagerare.

`hong({ eyes:"normal" });`

h: Per questo dovremmo fare terapia espositiva, inizieremo lentamente, un passo alla volta.

h: Ci fermeremmo prima di imbatterci in un pericolo *reale*.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Si metto il limite tra sentire un tuono, e stare in mezzo ad una tempesta con un cappello a punta.

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: Aspe', niente discussione su come mi sento? Solo... "Grazie"?

`hong({ eyes:"surprise", body:"shrug" })`

h: Si! Grazie per esserti preoccupato per {{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Tutto okay?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Non mi hai mai *ringraziato* prima.

`hong({ mouth:"smile" });`

h: Aw lupone fifone.

(#act4_something_else)

# act4_thanks_2

h: Anche se esageri, apprezzo che ti preoccupi per il mio {{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: Aspe'... non stai solamente ripetendo "grazie" per evitare di parlare delle tue paure, giusto?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Beh, la cose sono complicate, e io non ho sempre tutte le risposte.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Non é che la vita ti dá una lista di 3 risposte scelte da scegliere.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Ma per adesso almeno, posso almeno ringraziarti.

b: Beh, grazie anche a te per stare ad ascoltarmi.

`bb({ eyes:"closed" });`

b: Piccolo mammifero dalla pelle glabra.

(#act4_something_else)

# act4_thanks_3

h: Anche se il tuo blaterare mi spaventa, stai solo cercando di proteggermi {{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: Okay, se continui ad adularmi cosí, l'internet si fará delle strane idee su noi due.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Dai, sono solo un ragazzino universitario e tu sei un grande lupo spaventoso, qual è il peggio che ci può--

`hong({ eyes:"normal", body:"point" });`

h: OK, meglio non rispondere.

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Voglio assicurarmi che tu finalmente raggiunga quel profondo, umano, bisogno di appartenenza...

`bb({ eyes:"sad_u" });`

b: Ma mi preoccupo che se le persone scoprano chi siamo *per davvero* si spaventerebbero e scapperebbero via 

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Non so, ne ho abbastanza di decidere *io* cosa dire. *Tu* cosa hai da dire, umano?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Tocca di nuovo a te, umano. Che ne pensi?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Altri pensieri, umano?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Sono d'accordo: lavoriamo sulla nostra vita sociale.](#act4_alone_skills)

[Penso che piaceremmo alle persone. Ti va di scoprirlo?](#act4_alone_experiment)

[Grazie.](#act4_thanks) `_.thanks_for = "social belonging";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Potremmo allenarci a fare domande, ascoltare essere più empatici, aperti e vulnerabili...?

`hong({ eyes:"normal_l" });`

h: Oppure sviluppare delle abitudini sociali, come programmare uscite con amici o andare regolarmente a dei meetup?

`hong({ body:"one_up" });`

h: Potremmo anche imparare anche a essere più abituati all'essere rifiutati.

`hong({ eyes:"normal" });`

h: O imparare che le persone *non ci stanno* rifiutando, sono solo stanche o hanno la classica "Resting Bitch Face"

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Sono un sacco di opzioni...ma riguardo all'imparare delle abilità sociali...

[Non è *manipolatorio?*](#act4_alone_skills_manipulative)

[Non ci renderà più *facili da manipolare?*](#act4_alone_skills_manipulated)

[E se continuassimo a fallire?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: I serial killer che son bravi a leggere le emozioni dell loro vittime, non sono anche loro "empatici"?

`bb({ eyes:"annoyed" });`

b: Anche Charles Manson era bravo a farsi tanti amici e influenzare la gente

`hong({ eyes:"annoyed", body:"chin" });`

h: No, hai ragione.

h: Le "abilità sociali" sono insignificanti se comunque non ci importa *nulla* delle persone

`hong({ body:"normal" });`

h: In sostanza basta non essere una testa di ^cazzo^.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Un perfetto poster motivazionale

`hong({ body:"shrug", mouth:"narrow" });`

h: “Non essere una testa di ^cazzo^.™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Diventeremo uno zerbino, diremo Grazie Tante mentre la gente si pulirà le scarpe su di noi! 

`bb({ mouth:"scream", eyes:"scream" })`

b: Baceremo così tanti culi che sembrerà di indossare un rossetto marrone!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Nah, hai ragione: avere delle "abilità sociali" non significa solo far piacere agli altri, ma vuole anche dire saper definire dei *limiti*.

`hong( body:"one_up" });`

h: Non possiamo invitare persone nella nostra casa se la nostra casa non ha un tetto o dei muri per sorreggerlo.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: Inoltre riguardo quella metafora del rossetto... *che schifo??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Potremmo faillire. Anzi, *falliremo*.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: E va bene! Fallire è come le persone imparano!

`hong({ body:"normal", eyes:"normal" });`

h: Quindi continuiamo a fallire assieme, ok?

`bb({ eyes:"normal_r" });`

b: Certo, nello scenario peggiore potremmo trasferirci in un'altra città e farci una nuova identità.

`bb({ eyes:"normal" });`

h: Eh si, penso che costi solo un paio di bitcoin

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Potremmo fare qualche esperimento!

`hong({ body:"chin" });`

h: Potremmo chiamare qualcuno, rimetterci in contatto con qualche vecchio amico, o anche farci una chiacchierata con la barista.

`hong({ body:"normal" });`

h: Potremmo scoprire che siamo più piacevoli di quanto crediamo.

`bb({ eyes:"annoyed" });`

[E se queste fossero solo delle piccole "rivincite"?](#act4_alone_experiment_cheap)

[E se questo fosse un peso per gli altri?](#act4_alone_experiment_burden)

[Ma fare delle semplici chiacchiere non é il vero "te"!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Se ci limitiamo a sorridere non stabiliremo mai una relazione con qualcuno

`bb({ eyes:"super_sad" });`

b: *Ma* se ci apriamo agli altri tutti potranno vedere quanto siamo incasinati dentro!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Girati.

b: Cosa?

`hong({body:"hands_1"})`

h: Quando i cani vogliono mostrare amore e fiducia, si mostrano vulnerabili esponendo la propria pancia.

`hong({body:"one_up"})`

h: Forse non siamo *ancora* troppo stabili per essere troppo vulnerabili, ma con abbastanza allenamento,

`hong({body:"normal", eyes:"surprise"})`

h: Un giorno possiamo mostrare alle persone chi siamo davvero

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Mi giro solo se mi dai un regalino.

`bb({ eyes:"normal", mouth:"normal" });`

h: No.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Dire "ciao" alla barista non é esattamente vincere la medaglia d'oro alle Olimpiadi della Socialità.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: É per noi!

`hong({ body:"one_up", eyes:"annoyed" });`

h: Nell'arena della socialità non siamo neanche un peso piuma, siamo un peso quark.

`hong({ body:"normal", eyes:"normal" });`

h: Se dobbiamo partire con piccole vittorie, facciamolo. Dobbiamo partire dal primo scalino per arrivare al millesimo.

b: Sì! Dopo aver detto "Ciao", potremmo andare avanti e dire...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Come stai?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Non molto!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Forse la barista vuole solo fare dei caffé e non essere un *esperimento* per verificare se le nostre abilità sociali fanno schifo.

`bb({ eyes:"annoyed" })`

h: Bene, e se si scopre che siamo *davvero* un peso...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Buono a sapersi!

`hong({ eyes:"normal" });`

h: Potremmo anche imparare a prendere iniziativa e chiedere alle persone cosa va bene per loro e a mantenere le distanze.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Sai, tutte quella ^merda^ sulle abilità sociali che abbiamo letto sulle brochure degli psicologi.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Voglio difendere le tue necessità morali, la tua volontà di voler diventare una persona migliore,

`bb({ eyes:"sad_d" })`

b: Ma sembra come se sotto sotto siamo fondalmente...rotti.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: E non dirmi che *non* siamo incasinati. Abbiamo saltato da un *tetto*.
{{/if}}

{{if !_.INJURED}}
b: E non dirmi che *non* siamo incasinati. Ci siamo quasi buttati da un *tetto*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: Non so, ma ora basta, non voglio continuarti a dire *io* cosa dire. *Tu* cosa dici umano?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Di nuovo, a te, umano. Cosa ne dici?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Altri pensieri, umano?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Ok, siamo rotti. Aggiustiamoci.](#act4_bad_fix)

[Ok, siamo rotti. Accettiamolo.](#act4_bad_accept)

[Grazie.](#act4_thanks) `_.thanks_for = "moral well-being";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Potremmo creare lentamente delle nuovi abitudini. Riallineare la nostra vita ai nostri ideali.

`hong({body:"one_up"});`

h: E se c'è bisogno potremmo chiedere un aiuto a un terapista 

`hong({body:"normal"});`

h: Ci sono modi per aggiustarci

[E se non riuscissimo ad aggiustarci?](#act4_bad_fix_cant)

[E se ci aggiustiamo *troppo*?](#act4_bad_fix_too_much)

[Non possiamo permetterci un aiuto di un professionista.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Eh, penso che hai ragione.

h: Non possiamo aggiustarci completamente.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ahhh lo sapevo, saremo sempre rotti!

`hong({eyes:"surprise"});`

h: Ma almeno saremo *meno* rotti.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Le cicatrici guariscono col tempo, ma non spariscono mai completamente. E va bene così.

`bb({eyes:"annoyed_r"});`

b: Immagino. Tra l'altro,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: le cicatrici sono *sexy.*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Per piacere non farlo

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Mi sembra quasi malato ammetterlo ma una parte di me quasi *vuole* avere questo disordine.

`bb({ eyes:"angry" })`

b: Voglio dire, senza, non saremmo *noiosi?*

`bb({ eyes:"sad_r", body:"one_up" })`

b: Senza questo problema, la nostra arte non sarebbe blanda e mediocre?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Senza, non saremmo in grado di trovare una connessione con le persone che hanno questo problema?

`bb({ eyes:"sad", body:"chest" })`

b: Se fossimo soddisfatti della nostra vita, forse non cercheremo più di sforzarci per fare di meglio

`hong({ MOUTH_LOCK:true })`

h: ...

h: Se abbiamo paura di... "esaurire le paure"...

h: Non penso che esauriremo mai le nostre paure.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Eh si! Fiuu! Che sollievo!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Dottore, ho l'ansia di pagare $100 all'ora solo per sentirle dire *e questo come ti fa sentire?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Mm-hmm. E questo come ti fa sentire?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Nah, è una preoccupazione totalmente comprensibile. 

`hong({ eyes:"annoyed", mouth:"sad" });`

h: E fa davvero schifo che l'assistenza sanitaria non é disponibile a tutti.

`hong({ eyes:"normal", mouth:"normal" });`

h: Beh ci sono ancora delle alternative poco costose o addirittura gratuite:

`hong({ body:"chin" })`

h: Gruppi di supporto, terapie online, centri di salute per studenti o no profit...

`hong({ body:"hands_1" })`

h: Coltivare abitudini come la meditazione, il dormire bene, il chiacchierare regolarmente con amici, imparare nuove cose...

`hong({ body:"hands_2" })`

h: Andare in biblioteca per prendere in prestito dei libri di psicoterapie basate su prove scientifiche. 

`hong({ body:"one_up" })`

h: C'è un'enorme lista di risorse alla fine di questo gioco!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Abbiamo finalmente rotto questa *quarta parete* eh?

`hong({ body:"point" });`

h: Ci sono cose più importanti delle convenzioni narrative, come ad esempio la salute mentale.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Voglio dire questo è quello che i terapisti dicono, giusto? Accetta tutte le tue emozioni, anche quelle negative?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Aspetta.

["Accettare" vuol dire *arrendersi*?](#act4_bad_accept_give_up)

["Accettare" vuol dire *approvare*?](#act4_bad_accept_approve)

["Accettare" vuol dire *prenderle alla lettera*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Pensi che Martin Luter King abbia detto, "Accidenti, non possiamo sederci nel bus davanti, dovremmo *farcene una ragione*?"

`bb({ eyes:"angry_r", body:"two_up" });`

b: Perché il Complesso Industriale dell'Auto-Aiuto pensa che sventolare bandiera bianca sia qualche *profonda saggezza?*

`bb({ eyes:"annoyed", body:"normal" });`

h: Penso che i terapisti intendano dire che "accettare" queste cattive emozioni equivalga a riconoscere che esistano e che siano difficili da cambiare.

h: Ma non necessariamente arrendersi a una volontà di cambiamento. 

`bb({ eyes:"suspect" });`

b: Allora i terapisti dovrebbero dire *riconoscere*, non *accettare*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Ora che ci penso "accettare" confonde un po' le idee.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Bene, lo *riconosco*.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Come se fosse una cosa *buona* essere a pezzi? No!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Tutti quei maledetti sceneggiatori di Hollywood che romanticizzano la malattia mentale, sono degli schifosi!

`bb({ eyes:"angry", body:"two_up" });`

b: Avere una malettia mentale *fa schifo!* Deruba le persone delle loro *vite!* Perché dovremmo "accettarlo"?!

`bb({ body:"normal" });`

h: Penso che i terapisti intendano che "accettare" le nostre emozioni significa avere pazienza con loro.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Come agitarsi nelle sabbie mobili ti fa affondare più in fretta e la soluzione è aspettare pazientemente stendendosi sul dorso

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Mentre combattevo con te, la mia paura mi ha fatto saltare dal tetto.
{{/if}}

{{if !_.INJURED}}
h: Mentre combattevo con te, la mia paura mi ha quasi fatto saltare dal tetto.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Invece la soluzione è quello che stiamo facendo ora – non combatter, ma essere pazienti con l'altro.

`bb({ eyes:"annoyed" });`

b: Allora dovremmo dire *questo* invece di parole problematiche come "accettare".

`hong({ body:"chin", eyes:"annoyed" });`

h: Eh si, pensandoci "accettare" fa un po' schifo.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: Non accetto "accettare".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Ma sappiamo *già* che non dovremmo prenderlo alla lettera.

`bb({ eyes:"sad_u", body:"two_up" });`

b: Il *problema* è che voglio aiutarti, ma non so scegliere le parole per farlo. 

`bb({ eyes:"sad", body:"normal" });`

h: I think therapists mean "accept" your emotions as in: "don't fight or ignore them."

`hong({ eyes:"surprise", body:"one_up" });`

h: To listen to you, work *with* you, but not take what you say as 100% literal truth.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Then therapists should say *that* instead of some vague confusing word like "accept".

`hong({ body:"chin", eyes:"annoyed" });`

h: I guess they suck at using words, too.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Anyway, anything else you wanna chat about?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: So, anything else on your heavy heart?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[I'm scared we'll be harmed.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[I'm scared we'll be alone.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[I'm scared we're bad people.](#act4_bad)
{{/if}}

[Nah, I'm good for now.](#act4c_prelude)

# act4_something_else_2

h: Okay, I think we've talked about all our fears now.

b: Yes, there are only three fears.

h: Yup, exactly three.

b: Convenient.

(#act4c)

# act4c_prelude

h: Good chat, team.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: This isn't some *game*, you know.

`bb({eyes:"angry_d", body:"one_up"})`

b: Building a healthy relationship with your emotions isn't as simple as clicking buttons on a screen.

`bb({eyes:"sad", body:"normal"})`

b: *Can* we really get along?

b: *Can* we work together, as a team?

`hong({eyes:"sad", body:"one_up"})`

h: Well,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: E-excuse me...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: W-wo-would you mind if I sat with you for lunch?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *This* is your crush? Why are they sitting alone like a psycho serial killer?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Asking your crush if you can sit with them? Do you know how *needy* we sound?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *This* is your crush? We interrupted their peace and quiet! We're such a burden!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: I- I mean- it's, it's okay if not, I just...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Wait, didn't I see you at the party?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Yeah, of course! Come here.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Sorry, I need alone time right now.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Yeah you were on the couch! At the first party I went to...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Where I had that panic attack and punched the host.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Where I had that panic attack and ran out crying.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Hang on human, we may be making them uncomfortable.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, I don't mean to put you on the spot!

`publish("act4", ["hong_to_alshire",4]);`

h2: Just remembering a friendly face, is all.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHHHH I KNEW IT! THEY'RE A DANGEROUS PANIC-DRIVEN PSYCHO!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHHH THE FIRST IMPRESSION WE MADE WAS "WITNESSED MY TRAUMA"! THAT MEANS THEY HATE US!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAHHH WE MADE SOMEONE REMEMBER A TRAUMATIC EVENT. OUR MERE PRESENCE HURTS OTHERS.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Hang on human, they seem uncomfortable.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, no pressure of course!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Just saying, you can sit here if you want to.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: THEY'RE BEING *TOO* FRIENDLY! LIKE TED BUNDY, THE SERIAL KILLER!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: THEY'RE JUST ACTING NICE! NO ONE *REALLY* WANTS TO BE CLOSE TO US!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH WE ALWAYS MAKE OTHERS FEEL AWKWARD! WE'RE A STAIN UPON THE EARTH!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Hang on human, we may be making them uncomfortable.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, I don't mean to be rude!

`publish("act4", ["hong_to_alshire", 6]);`

h2: I just need some time to process my emotions. Please don't take it as a personal rejection.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: WHAT SICK, TWISTED THOUGHTS ARE THEY PROCESSING?! WHAT DARK DESIRES FILL THIS PSYCHO'S HEART?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: WE'VE BEEN PERSONALLY REJECTED! WE'LL NEVER BE LOVED!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: WE INTERRUPTED THEIR EMOTIONAL PROCESSING! NOW THEY'LL BE TRAUMATIZED FOREVER AND IT'S ALL OUR FAULT!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: Huh. That was weird. I wonder what was going on in their head.

`publish("act4", ["hong_closer", 2]);`

h: Anyway, you were saying?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Uh, I forget? Something about teams and work?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: They say you should "make peace" with your emotions, as if your emotions are *war criminals*.

`publish("act4", ["bb_closer", 7]);`

b: But I want us to make *more* than mere peace! I want us to be *allies!*

`publish("act4", ["bb_closer", 3]);`

b: I want to be a good guard-dog. Just like how hunger & thirst are alarms for your physical needs,

`publish("act4", ["bb_closer", 8]);`

b: I want to be the alarm for your *psychological* needs – your needs for safety, belonging, goodness.

`publish("act4", ["bb_closer", 1]);`

b: But... I suck at my job, so I need you to train me.

`publish("act4", ["bb_closer", 4]);`

b: I'm not "always valid," nor "always irrational." I'm just... trying my best. So, please,

`publish("act4", ["bb_closer", 30]);`

b: Help me help you!

`publish("act4", ["bb_closer", 6]);`

b: Though, teaching an old dog new tricks *will* take a while. Maybe *years.*

`publish("act4", ["bb_closer", 3]);`

b: And sometimes I'll relapse, I'll slip into my old habits.

`publish("act4", ["bb_closer", 2]);`

b: I'll bark at shadows. I'll scare you with words. I might even show you some intrusive images of... things.

`publish("act4", ["bb_closer", 9]);`

b: I'm sorry! I'm a battered shelter dog! Battered dogs poop on your bed sometimes!

`publish("act4", ["bb_closer", 4]);`

b: But if you're patient with me... and just stay and sit with me...

`publish("act4", ["bb_closer", 8]);`

b: Maybe you can tame this wolf.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Good dog.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Good human.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: AAAAA YOU'RE STILL EATING ALONE FIFTEEN CIGARETTES AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA YOU'RE STILL NOT PRODUCTIVE WHILE EATING WE'RE SOCIETY-PARASITES AAAAA
{{/if}}
s
{{if _.whitebread}}
b: AAAAA YOU'RE EATING MORE WHITE BREAD AAAAA
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: YAP YAP YAP YAP YAP

(#credits)
