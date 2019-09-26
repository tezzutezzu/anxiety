# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[GIOCA!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Ok, prima di cominciare, come ti piacerebbe leggere?

`publish("show_options_bottom")`

# intro-start-2

n3: Bene, cominciamo la nostra storia...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: QUESTO È UN UMANO

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: E QUESTA È L'ANSIA DELL'UMANO

n: _TU_ SEI L'ANSIA

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Lalala, no. Non ti sento. Dò un'occhiata al mio telefono.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: IL TUO COMPITO È PROTEGGERE IL TUO UMANO DAL *PERICOLO*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Oh no! Stai buttando la tua vita su Twitter! Di nuovo!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Già, chissà perché semplicemente non mi siedo e asolto i miei pensieri più spesso.

`hong({eyes:"neutral"});`

n: PRESO, AVVERTILO DI UN *PERICOLO!*

```
bb({eyes:"look"});
```

[Oh no di nuovo quella new orribil!](#act1d_news)

[Oh no, ma quel tweet sta parlando di noi?](#act1d_subtweet)

[Eh!i, una gif di un gattino che beve il latte](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Hehe è così carin-- 

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: I GATTI NON DIGERISCONO IL LATTE E SIAMO DELLE PERSONE ORRIBILI PER GODERE DEGLI ABUSI SUGLI ANIMALI

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



