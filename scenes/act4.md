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

n3: (Gioco salvato.)

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

h: Quindi quale diavolo è la morale della storia?

`hong({body:"one_up", eyes:"annoyed"})`

h: Che cosa abbiamo *imparato*? Io sono stato stupido, i miei "amici" mi hanno usato e siamo quasi *morti*.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Per non parlare delle spese mediche.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Per non parlare dei danni al fegato.](#act4a_liver)
{{/if}}

[Eh già, era proprio lo scenario peggiore.](#act4a_worst)

[Avevo ragione.](#act4a_right)

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

b: Di sicuro abbiamo perso qualche anno di vita...

`bb({eyes:"surprise"});`

b: Almeno una vita ce l'abbiamo *ancora*! Siamo sopravvissuti!

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

b: Però... anche tu avevi ragione.

`hong({eyes:"surprise"});`

h: Hm?

`bb({eyes:"normal"});`

b: *Ero io* che gridavo "al lupo". Perciò, quando il pericolo é diventato *reale*, tu ovviamente non mi hai creduto.

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

b: Beh, ora tutto il resto mi sembra meno spaventoso. Mi ha fatto riflettere.

`bb({eyes:"normal", mouth:"normal"});`

b: Litigare con te non va bene perché non mi permette di proteggerti.

h: Ma anche litigare con te non va bene, non serve ad altro se non farti urlare di più.

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

b: Non sono il Lupo Cattivo, ma non sono neanche un lupo guardiano.

`bb({eyes:"sad_d"})`

b: Sono un cane randagio e malconcio.

`bb({eyes:"sad"})`

b: Ne abbiamo passate tante. Forse un trauma o un abbandono. Per questo a volte esagero e faccio:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: WOF WOF WOF WOF WOF WOF

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Ma non *voglio* essere un codardo! Voglio proteggerti! Voglio essere un bravo cane!

`bb({eyes:"sad", mouth:"normal"});`

b: Umano... mi aiuterai ad addomesticarmi?

`hong({eyes:"sad"})`

h: Ci... ci proverò.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: OK. Un rapporto sano con le emozioni. I rapporti hanno bisogno di comunicazione. Quindi, comunichiamo.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: I prossimi cinque minuti saranno super sdolcinati, ma proviamoci finché non ci riusciamo.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Caro lupo interiore...*Tu* come stai?

n2: NUMERO DI PAURE USATE:

n2: *FARSI MALE* {{_.attack_harm_total}}, *NON AMATO* {{_.attack_alone_total}}, *CATTIVO* {{_.attack_bad_total}}

n2: DI QUALE PAURA VUOI PARLARE PRIMA? (POSSIAMO PARLARE DELLE ALTRE DOPO)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Ho paura di farmi male.](#act4_harm)

[Ho paura di rimanere da solo.](#act4_alone)

[Ho paura di essere una brutta persona.](#act4_bad)

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

[Hai ragione. Proteggiamoci.](#act4_harm_skills)

[Esponiamoci a *più* pericoli.](#act4_harm_exposure)

[Grazie.](#act4_thanks) `_.thanks_for = "physical safety";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Ma... come? Io ho zanne e artigli, ma sono solo una metafora.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Potremmo imparare un po' di auto-difesa? Unirci ad un gruppo che si protegge a vicenda? Migliorare la nostra salute e superare i nostri limiti?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Forse, ma...

[E da dove iniziamo?](#act4_harm_skills_start)

[E se non dovesse funzionare?](#act4_harm_skills_work)

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

h: Ci stiamo esercitando a comunicare. Ci aiuterá a percepire il pericolo con meno falsi positivi,

`hong({ eyes:"surprise" });`

h: E questo ci aiuterá a proteggerci dal dolore!

`hong({ eyes:"normal", mouth:"normal" });`

h: Perciò: questo *è* un corso di auto-difesa.

`bb({ eyes:"normal_r" })`

b: Oh. Mi aspettavo piú di questo:

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

h: Ma anche un miglioramento dell'1% vale la pena, no?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Vedere il bicchiere non come vuoto al 99%, ma come pieno all'1%?

`bb({ eyes:"normal" });`

h: Che avrebbe ancora valore se fossi bloccato in mezzo al deserto.

`bb({ eyes:"closed" });`

b: Beh. Alla goccia, allora.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: L'unica ragione per cui hai ignorato i miei avvertimenti é perché ho esagerato con la sicurezza! 

`bb({ body:"normal", eyes:"normal" })`

h: Hai ragione. Dovremmo pensare alla sicurezza, a tutto, con moderazione.

`bb({ eyes:"suspect" })`

b: Scusa, *TUTTO* con moderazione?

`hong({ eyes:"annoyed" })`

h: *Un numero moderato di cose* con moderazione.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Grazie per aver reso le tue dichiarazioni coerenti e consistenti.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *COSA*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Voglio dire: immagina un cane ha paura dei tuoni.

`hong({ body:"hands_1" });`

h: Un trucco usato dagli addestrattori é fargli ascoltare un tuono a basso volume, premiandolo quando rimane calmo.

`hong({ body:"hands_2" });`

h: Nei giorni successivi, l'addestratore inizia ad alzare il volume, fino a quando il cane non ha più paura.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Si chiama terapia espositiva!

`hong({ body:"point", eyes:"normal" });`

h: Dato che sei un cane dovrebbe funzionare, no? Tutti i mammiferi hanno lo stesso meccanismo di risposta agli stimoli.

`hong({ body:"normal" });`

[E se ci desensibilizziamo *troppo*?](#act4_harm_exposure_overboard)

[E se ci esponiamo a del pericolo *vero*?](#act4_harm_exposure_hurt)

[Sono un lupo, non un cane.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: Ti mostrerò gentilezza e pazienza fino a farti diventare un cucciolotto.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Oh.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: Abbiamo appena visto che quando ignori le tue paure ti metti in *serio* pericolo.

`bb({ eyes:"angry_r", body:"one_up" })`

b: E poi: *tutta* questa desensibilizzazione non ci fará diventare psicopatici?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Presto inizieremo persino a darci dei premi mentre guardiamo dei porno violenti!

`hong({ eyes:"annoyed" })`

h: Penso ci sia una gran differenza tra quello e il tuono.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: *Quale*, esattamente?!

`hong({ eyes:"surprise", body:"one_up" })`

h: Non so, ma *tu* mi puoi aiutare!

`hong({ eyes:"normal", body:"normal" })`

h: Lavorandoci e parlandone insieme, riusciremo a capire la differenza.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Ok. Io però non ho i pollici opponibili, perciò il disegno devi farlo tu.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: Ad esempio: ci siamo buttati giu da un cavolo di *tetto!*
{{/if}}

{{if !_.INJURED}}
b: Ad esempio: per poco non ci siamo buttati giù da un cavolo di *tetto!*
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Hai ragione. Si rischia di esagerare.

`hong({ eyes:"normal" });`

h: Per questo dovremmo fare terapia espositiva. Iniziamo con calma, un passo alla volta.

h: E prima di imbatterci in un pericolo *reale*, ci fermiamo.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Capirò la differenza tra sentire un tuono e stare in mezzo alla tempesta con un cappello a punta.

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

b: Aspetta, nulla da ribattere su quello che ti ho detto? Solo... "Grazie"?

`hong({ eyes:"surprise", body:"shrug" })`

h: Si! Grazie per esserti preoccupato per {{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Tutto ok?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Non mi avevi mai *ringraziato*.

`hong({ mouth:"smile" });`

h: Oh, piccolo tenerone fifone.

(#act4_something_else)

# act4_thanks_2

h: Anche se esageri, apprezzo che ti preoccupi per {{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: Aspetta... non stai ripetendo "grazie" solo per evitare di parlare delle tue paure, vero?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Beh, la faccenda è complicata e non ho sempre tutte le risposte.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: La vita vera non è fatta di dialoghi a scelta multipla.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Per adesso, almeno, posso ringraziarti.

b: Beh, grazie a te che mi stai a sentire.

`bb({ eyes:"closed" });`

b: Piccolo mammifero dalla pelle glabra.

(#act4_something_else)

# act4_thanks_3

h: Anche se mi fai paura quando blateri, cerchi solo di proteggermi da {{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: OK, se continui ad adularmi cosí, l'internet si fará delle strane idee su noi due.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Ma dai, sono solo un giovane vulnerabile e tu un grande lupo spaventoso, cosa potrebbero pensar--

`hong({ eyes:"normal", body:"point" });`

h: OK, meglio evitare.

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Vorrei che soddisfacessi il tuo enorme bisogno di appartenenza...

`bb({ eyes:"sad_u" });`

b: Ma ho paura che se le persone ci conoscessero *veramente* si allontanerebbero da noi. 

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Non so, ne ho abbastanza di parlare *io*. *Tu* cosa hai da dire, umano?
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

h: Potremmo allenarci a fare domande e ad ascoltare, ad essere più empatici, aperti e vulnerabili?

`hong({ eyes:"normal_l" });`

h: Oppure potremmo sviluppare delle abitudini sociali, come programmare uscite con amici o andare a degli incontri?

`hong({ body:"one_up" });`

h: Potremmo anche imparare a scendere a patti con il rifiuto.
`hong({ eyes:"normal" });`

h: O imparare che le persone *non ci stanno* rifiutando, che magari sono solo stanche o hanno una naturale espressione crucciata.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Sono un sacco di opzioni. Parlando di imparare a socializzare...

[Non è *manipolatorio?*](#act4_alone_skills_manipulative)

[Non ci renderà più *facili da manipolare?*](#act4_alone_skills_manipulated)

[E se fallissimo di nuovo?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: I serial killer che sanno leggere le emozioni delle loro vittime; non è "empatia" anche quella?

`bb({ eyes:"annoyed" });`

b: Anche Charles Manson era bravo a farsi tanti amici e a manipolare le persone?

`hong({ eyes:"annoyed", body:"chin" });`

h: Hai ragione.

h: "Socializzare" non serve a niente se cnon ci importa *nulla* delle persone

`hong({ body:"normal" });`

h: In sostanza basta non essere una testa di ^cazzo^.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Un perfetto poster motivazionale.

`hong({ body:"shrug", mouth:"narrow" });`

h: “Non essere una testa di ^cazzo^.™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Diventeremo uno zerbino, diremo "grazie tante" mentre la gente si pulirà le scarpe su di noi! 

`bb({ mouth:"scream", eyes:"scream" })`

b: Baceremo così tanti culi che sembrerà di indossare un rossetto marrone!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: No, hai ragione: "socializzare" non significa solo compiacere gli altri, ma anche saper mettere dei *paletti*.

`hong( body:"one_up" });`

h: Non possiamo invitare gente a casa se questa non ha nemmeno i muri.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: E poi, la metafora del rossetto... *che schifo!*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Potremmo sbagliare. Anzi, *sbaglieremo*.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: E va bene! Solo sbagliando si impara!

`hong({ body:"normal", eyes:"normal" });`

h: Perciò continuiamo a sbagliare insieme, ok?

`bb({ eyes:"normal_r" });`

b: Certo, male che vada potremmo trasferirci in un'altra città e cambiare identità.

`bb({ eyes:"normal" });`

h: Già, dovrebbe costare solo un paio di bitcoin.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Potremmo fare qualche esperimento!

`hong({ body:"chin" });`

h: Potremmo chiamare qualcuno, rimetterci in contatto con qualche vecchio amico, oppure andare al bar a fare due chiacchiere.

`hong({ body:"normal" });`

h: Potremmo scoprire che siamo più piacevoli di quanto crediamo.

`bb({ eyes:"annoyed" });`

[Potrebbero essere delle piccole "rivincite"?](#act4_alone_experiment_cheap)

[E se fossimo un peso per gli altri?](#act4_alone_experiment_burden)

[A noi non interessano le chiacchiere da bar!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Se ci limitiamo a sorridere non stabiliremo mai una relazione con qualcuno,

`bb({ eyes:"super_sad" });`

b: *ma* se ci esponiamo tutti potranno vedere quanto siamo incasinati!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Girati.

b: Cosa?

`hong({body:"hands_1"})`

h: Quando i cani ti vogliono bene e si fidano di te si mettono a pancia in su.

`hong({body:"one_up"})`

h: Forse non siamo *ancora* abbastanza forti per essere vulnerabili, ma con un po' di allenamento

`hong({body:"normal", eyes:"surprise"})`

h: un giorno potremo mostrarci per come siamo davvero: incasimati, ma del tutto umani.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Mi giro solo se mi dai un premietto.

`bb({ eyes:"normal", mouth:"normal" });`

h: No.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Dire "ciao" alla barista non é esattamente come vincere la medaglia d'oro alle Olimpiadi della Socialità.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Per noi lo è!

`hong({ body:"one_up", eyes:"annoyed" });`

h: Nell'arena della socialità non siamo neanche un peso piuma, siamo un peso quark.

`hong({ body:"normal", eyes:"normal" });`

h: Se dobbiamo partire con piccole vittorie, così sia. Bisogna salire il primo gradino per arrivare al millesimo.

b: Sì! Dopo aver detto "Ciao", potremmo andare avanti e dire...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Come stai?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Tutto bene!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Forse la barista vuole solo lavorare in pace, invece di fare da *cavia* per i nostri esperimenti di socializzazione.

`bb({ eyes:"annoyed" })`

h: Beh, se si scoprisse che siamo *davvero* un peso...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Buono a sapersi!

`hong({ eyes:"normal" });`

h: Potremmo anche imparare a prendere iniziativa e chiedere alle persone cosa va bene per loro e rispettare i loro spazi.
```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Sai, tutta quella ^merda^ sulle capacità interpersonali che abbiamo letto sulle brochure dello psicologo.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Voglio difendere le tue necessità morali, la tua volontà di voler diventare una persona migliore,

`bb({ eyes:"sad_d" })`

b: ma sembra come se, alla base nel profondo, ci fosse qualcosa di... rotto.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: E non venirmi a dire che *non* siamo incasinati. Ci siamo buttati da un *tetto*.
{{/if}}

{{if !_.INJURED}}
b: E non venirmi a dire che *non* siamo incasinati. Ci siamo quasi buttati da un *tetto*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: Non lo so, ma ora basta, sono stanco di scegliere cosa dire. *Tu* cosa dici?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Toccca di nuovo a te. Cosa ne dici?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Altri pensieri?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Ok, siamo rotti. Aggiustiamoci.](#act4_bad_fix)

[Ok, siamo rotti. Accettiamolo.](#act4_bad_accept)

[Grazie.](#act4_thanks) `_.thanks_for = "la mia integritá";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Potremmo creare una alla volta delle nuove abitudini. Riallineare la nostra vita con i nostri ideali.

`hong({body:"one_up"});`

h: E se servirà potremmo chiedere aiuto a un terapeuta o a uno psicologo.

`hong({body:"normal"});`

h: I modi per aggiustarci ci sono.

[E se non ci riuscissimo?](#act4_bad_fix_cant)

[E se ci aggiustassimo *troppo*?](#act4_bad_fix_too_much)

[Non possiamo permetterci l'aiuto di un professionista.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Penso che tu abbia ragione.

h: Non possiamo aggiustarci completamente.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ahhh lo sapevo, saremo sempre rotti!

`hong({eyes:"surprise"});`

h: Ma possiamo essere un po' *meno* rotti.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Le cicatrici col tempo guariscono ma non vanno mai via del tutto. E va bene così.

`bb({eyes:"annoyed_r"});`

b: Immagino di sì. Tra l'altro,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: le cicatrici sono *sexy*.

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Ti prego, evita.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Mi sembra strano ammetterlo, ma una parte di me *desidera* avere questo disordine.

`bb({ eyes:"angry" })`

b: Voglio dire, non saremmo *noiosi*, senza?

`bb({ eyes:"sad_r", body:"one_up" })`

b: Senza questo problema, la nostra arte non sarebbe piatta e mediocre?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Non saremmo in grado di capire chi ha le nostre stesse ferite.

`bb({ eyes:"sad", body:"chest" })`

b: Se ci accontentassimo, forse non cercheremmo di sforzarci per fare di meglio.

`hong({ MOUTH_LOCK:true })`

h: ...

h: Se abbiamo paura di... "non avere più paure"...

h: Non penso che rimarremo senza.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Evvai! Meno male!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Dottore, ho l'ansia di pagare $100 all'ora solo per sentirle dire *e questo come ti fa sentire?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "E questo come ti fa sentire?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: È una preoccupazione totalmente comprensibile. 

`hong({ eyes:"annoyed", mouth:"sad" });`

h: Ed è davvero brutto che l'assistenza psicologica non sia accessibile a tutti.

`hong({ eyes:"normal", mouth:"normal" });`

h: Beh, ci sono delle alternative poco costose o addirittura gratuite:

`hong({ body:"chin" })`

h: Gruppi di supporto, terapie online, centri per la salute fatti da studenti o da no profit...

`hong({ body:"hands_1" })`

h: Coltivare abitudini come la meditazione, il buon sonno, chiacchierare regolarmente con amici, imparare cose nuove...

`hong({ body:"hands_2" })`

h: Andare in biblioteca e prendere in prestito libri di psicoterapia che funzionano.

`hong({ body:"one_up" })`

h: C'è una lista di risorse enorme alla fine di questo gioco!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Non è durata molto *questa* quarta parete.

`hong({ body:"point" });`

h: Ci sono cose più importanti delle convenzioni narrative, come ad esempio la salute mentale.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: O almeno, questo è quello che dicono gli psicologi, no? Accetta tutte le tue emozioni, anche quelle negative?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Aspetta.

["Accettare" vuol dire *rassegnarsi*?](#act4_bad_accept_give_up)

["Accettare" vuol dire *approvare*?](#act4_bad_accept_approve)

["Accettare" nel senso *letterale* del termine?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Pensi che Martin Luter King avrebbe detto: "accidenti, non possiamo sederci nel bus davanti, dovremmo *farcene una ragione*?"

`bb({ eyes:"angry_r", body:"two_up" });`

b: Perché il Complesso Industriale dell'Auto-Aiuto pensa che sventolare bandiera bianca sia segno di *profonda saggezza?*

`bb({ eyes:"annoyed", body:"normal" });`

h: Penso che gli psicologi intendano dire che "accettare" le emozioni negative equivalga a riconoscere che esistono e che non sono facili da modificare,

h: ma non necessariamente arrendersi senza provare a cambiarle.

`bb({ eyes:"suspect" });`

b: Allora i terapisti dovrebbero dire *riconoscere*, non *accettare*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Ora che ci penso "accettare" confonde un po' le idee.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Bene, lo *riconosco*.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Come se andasse bene ssere a pezzi? No!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Tutti quegli sceneggiatori di Hollywood che romanticizzano la malattia mentale sono degli incoscienti!

`bb({ eyes:"angry", body:"two_up" });`

b: Avere una malettia mentale *fa schifo!* Deruba le persone delle loro *vite!* Perché dovremmo "accettarlo"?!

`bb({ body:"normal" });`

h: Penso che gli psicologi intendano che "accettare" le nostre emozioni significa avere pazienza.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Come agitarsi nelle sabbie mobili ti fa affondare più in fretta e la soluzione è aspettare pazientemente stendendosi sul dorso,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Combattere contro di te mi ha portato a saltare da un tetto.
{{/if}}

{{if !_.INJURED}}
h: Combattere contro di te mi ha quasi portato a saltare da un tetto.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Invece la soluzione è quello che stiamo facendo ora – non combattere, ma essere pazienti l'uno con l'altro.

`bb({ eyes:"annoyed" });`

b: Allora è *questo* che dovremmo dire, invece di usare parole fraintendibili come "accettare".

`hong({ body:"chin", eyes:"annoyed" });`

h: Eh si, pensandoci "accettare" fa un po' schifo.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: Non accetto "accettare".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: *Sai* che non devi prendermi alla lettera!

`bb({ eyes:"sad_u", body:"two_up" });`

b: Il *problema* è che voglio aiutarti, ma con le parole faccio schifo perciò non ci riesco.

`bb({ eyes:"sad", body:"normal" });`

h: Penso che gli psicologi dicano di "accettare" le tue emozioni nel senso di: "non combatterle o ignorarle."

`hong({ eyes:"surprise", body:"one_up" });`

h: Ascoltare te stesso, lavorare su *te stesso* e non prendere per verità assoluta quello che ti dici.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Allora è *questo* che dovremmo dire, invece di usare una parola vaga e fraintendibile come "accettare".

`hong({ body:"chin", eyes:"annoyed" });`

h: Penso che anche loro forse non siano molto bravi con le parole.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Comunque, c'è qualcos'altro di cui vorresti parlare?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: C'è qualche altro peso che ti vuoi togliere?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Ho paura di farmi male.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Ho paura di rimanere da solo.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Ho paura di essere una brutta persona.](#act4_bad)
{{/if}}

[Sto bene per ora.](#act4c_prelude)

# act4_something_else_2

h: Ok, mi pare che abbiamo parlato di tutte le nostre paure.

b: Si, ci sono solo tre paure.

h: Si, esattamente tre.

b: Ottimo.

(#act4c)

# act4c_prelude

h: Bella chiacchierata, compagno.

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

b: Questo non è un semplice *gioco*.

`bb({eyes:"angry_d", body:"one_up"})`

b: Creare una relazione sana con le tue emozioni non è semplice come premere dei pulsanti su uno schermo.

`bb({eyes:"sad", body:"normal"})`

b: *Possiamo* davvero andare d'accordo?

b: *Possiamo* lavorare assieme, come una squadra?

`hong({eyes:"sad", body:"one_up"})`

h: Beh,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: S-scusami...

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

a: T-ti spiace se mi siedo con te per mangiare?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *Questa* è la ragazza che ti piace? Perché è seduta da sola come un serial killer?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Non è un po' troppo da disperati chiedere se puoi sederti qui?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *Questa* è la ragazza che ti piace? Abbiamo interrotto il suo attimo di tranquillità! Che palla che siamo.
{{/if}}

`publish("act4", ["alshire", 2]);`

a: V-voglio dire, se n-non ti disturbo...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Aspetta, non ci siamo già visti alla festa?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Certo! Siediti pure.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Scusa, ho bisogno di stare un attimo da solo.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Sì, eri sui divanetti! Alla prima festa alla quale sono andato...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Quella dove ho avuto un attacco di panico e ho dato un pugno al proprietario.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Quella dove ho avuto un attacco di panico e sono scappato via.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Aspetta, forse la stiamo mettendo in imbarazzo.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Scusa, non volevo metterti in imbarazzo...

`publish("act4", ["hong_to_alshire",4]);`

h2: Stavo solo ricordando una faccia amica, tutto qui.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHH LO SAPEVO! E' UN PAZZO PSICOPATICO!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHH LO SAPEVO ABBIAMO ROVINATO LA PRIMA IMPRESSIONE SVELANDO IL NOSTRO TRAUMA! ORA CI ODIANO!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAHHH GLI ABBIAMO RICORDATO UN MOMENTO TRAUMATICO DELLA SUA VITA! LA NOSTRA PRESENZA È NOCIVA.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Aspetta, forse la stiamo mettendo in imbarazzo.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Nessuna pressione, ovviamente!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Puoi sederti qui se vuoi.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: SONO *TROPPO* AMICHEVOLI! NON SARANNO MICA DEI SERIAL KILLER?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: STANNO SOLO FINGENDO DI ESSERE CARINI! NESSUNO VUOLE SEDERSI CON NOI!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH METTIAMO SEMPRE GLI ALTRI IN IMBARAZZO! SIAMO UNA PIAGA DEL PIANETA!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Aspetta, forse la stiamo mettendo in imbarazzo.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, non volevo essere scortese!

`publish("act4", ["hong_to_alshire", 6]);`

h2: Mi serve solo un momento per elaborare le mie emozioni. Non prenderla sul personale.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: QUALI ORRIBILI PENSIERI STARANNO MAI FACENDO?! CHISSÀ CHE DESIDERI RIVOLTANTI CI SONO NEL CUORE DI QUESTO PSICOPATICO!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: SIAMO STATI RIFIUTATI! NESSUNO CI AMERA' MAI!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: ABBIAMO INTERROTTO I LORO PENSIERI! ADESSO SARANNO TRAUMATIZZATI A VITA!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: CORRI CORRI CORRI CORRI CORRI CORRI CORRI CORRI CORRI 

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

h: Oh. Che strano. Mi domando cosa le sia preso.

`publish("act4", ["hong_closer", 2]);`

h: Comunque, cosa stavi dicendo?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Non mi ricordo... Qualcosa riguardo al lavoro di squadra?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Dicono che dovresti "riappacificarti" con le tue emozioni. Come se le emozioni fossero un nemico di guerra.

`publish("act4", ["bb_closer", 7]);`

b: Ma io voglio *più* che una semplice pace! Vorrei che fossimo *alleati*!

`publish("act4", ["bb_closer", 3]);`

b: Io vorrei essere un buon cane da guardia, così come la fame e la sete lo sono per i tuoi bisogni fisici,

`publish("act4", ["bb_closer", 8]);`

b: Io voglio essere un allarme per i tuoi bisogni *psicologici* – il tuo bisogno di sentirti sicuro, di appartenenza, di sentirti una brava persona.

`publish("act4", ["bb_closer", 1]);`

b: Ma... non sono bravo nel mio lavoro, devi allenarmi.

`publish("act4", ["bb_closer", 4]);`

b: Non ho sempre ragione, ma nemmeno sempre torto. Sto soltanto... facendo del mio meglio. Quindi, per piacere,

`publish("act4", ["bb_closer", 30]);`

b: Aiutami ad aiurtarti!

`publish("act4", ["bb_closer", 6]);`

b: Anche se ci vorrà molto tempo a farmi imparare nuove cose. Forse *anni*.

`publish("act4", ["bb_closer", 3]);`

b: E alle volte ci ricascherò, ritornerò alle mie vecchie abitudini.

`publish("act4", ["bb_closer", 2]);`

b: Abbaierò alle ombre. Ti spaventerò con le parole. Potrei perfino farti immaginare...cose.

`publish("act4", ["bb_closer", 9]);`

b: Scusami ma sono solo un cane abbandonato e impaurito! I cani abbandonati fanno la cacca nel letto a volte!

`publish("act4", ["bb_closer", 4]);`

b: Ma se sarai paziente con me...

`publish("act4", ["bb_closer", 8]);`

b: Riuscirai a domarmi.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Bravo cane.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Bravo umano.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

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
b: AAAAA STAI ANCORA MANGANDO DA SOLO AAAH QUINDICI SIGARETTE AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA NON SEI PRODUTTIVO QUANDO MANGI AAAAA PARASSITA AAAA
{{/if}}

{{if _.whitebread}}
b: AAAAA STAI ANCORA MANGIANDO PANE BIANCO AAAAA
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

b: WOF WOF WOF WOF WOF WOF WOF

(#credits)
