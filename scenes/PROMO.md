# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[ГРАТИ!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Тож, перш ніж почати, як *тобі* буде зручно читати?

`publish("show_options_bottom")`

# intro-start-2

n3: Тепер, почнімо нашу історію...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: ЦЕ ЛЮДИНА

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

n: А ЦЕ ЇЇ ТРИВОЖНІСТЬ

n: _*ТИ*_ Є ТРИВОЖНІСТЮ

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Ніт. Ні, нє-а, я не слухаю. Гляну, що там в телефоні.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: ТВОЯ РОБОТА - ЗАХИСТИТИ ЛЮДИНУ ВІД *НЕБЕЗПЕКИ*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Ах! Ти провтикуєш своє життя у Твіттері! Знову!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Дійсно, чи не краще мені було б частіше сидіти і слухати власні думки.

`hong({eyes:"neutral"});`

n: ШВИДКО, ПОПЕРЕДЬ ЇХ ПРО "НЕБЕЗПЕКУ"*

```
bb({eyes:"look"});
```

[О ні, глянь на ці жахливі новини!](#act1d_news)

[О ні, а що як цей твіт насправді *про нас?*](#act1d_subtweet)

[Гей, гіфка з котиком, що п'є молоко!](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Хех, миленько. Я--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: КОТАМ НЕ МОЖНА МОЛОКА, І МИ ЖАХЛИВІ, ЩО НАСОЛОДЖУЄМОСЬ ЗНУЩАННЯМ НАД ТВАРИНКОЮ

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



