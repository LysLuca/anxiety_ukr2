# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Будьмо!

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

h2: *Ah* that hits the spot.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: Знаєш, дитя...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: Точніше, уражені частини - моя права і ліва амигдали.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Ти нагадуєш мені про мене самого, коли я був молодшим. Тоді я теж мучився від звіра у моїй голові.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: Я такий радий, що маю змогу передати це далі і допомогти вбити ту тварюку, як я це зробив зі своєю.

```
publish("act3",["roofhunter",2]);
```

r: Гей, швидке питання: правда чи ді--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: ДІЯ!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Ахах! Добре.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Окей. Бачиш отой блакитний басейн отам?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Ага? Той, що сім поверхів під нами?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Стрибни туди.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Чекай, що??

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: Звір знову скиглить, так?

```
publish("act3",["roofhunter",23]);
```

r: *О нііііі, це небезпечно, не роби цьогоооо.*

```
publish("act3",["roofhunter",22]);
```

r: Але саме тому нам і потрібні такі смертельно-гострі відчуття! Веселися від душі! Carpe diem! Глуши колу зі ^сраки^ повії, живемо лише раз!

```
publish("act3",["roofhunter",10]);
```

r: Покажи тому звіру, що ми клали, не один, а два ^хуї^ на його ^пизд^іння! Стрибай.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Ем, але іноді, ем... страх має сенс...

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

r: Перепрошую, ти що, повелися на пропаганду пана Майндфулднеса, що почуватись погано - *добре*?

```
publish("act3",["roofhunter",17]);
```

r: Ті ^уйобки^, що правлять цим світом, викликають у всіх *нас* тривожність і депресію,

```
publish("act3",["roofhunter",18]);
```

r: А тоді роблять TED Talks, щоб нав'язати нам "прийняття" нашої ^йобнутості^ і "любові" до того садистичного демона всередині нас!

```
publish("act3",["roofhunter",6]);
```

r: Дитя, я знаю, що *ти* знаєш, що та тварюка *завдає болю* таким, як ми. Вона*мучить* таких, як ми.

```
publish("act3",["roofhunter",19]);
```

r: Вона не наш друг. Це скажений звір, якого треба або *усипити*,

```
publish("act3",["roofhunter",20]);
```

r: Або ж *загнати кулю йому в лоба*.

```
publish("act3",["roofhunter",27]);
```

r: Інакше він переможе.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: Ні. Ти помиляєшся.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: Я не дозволю йому перемогти.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: Так ^блять^! Я вірю в тебе, крихітко! Убий його! <3

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

b: ні ні ні ні ні ні

n: ЦЯ ГЛАВА МАЄ ДВІ МОЖЛИВІ КІНЦІВКИ. ОДНА З НИХ *ДУЖЕ, ДУЖЕ ПОГАНА*.

b: НІ НІ НІ НІ НІ НІ НІ НІ НІ НІ НІ НІ НІ

n: ОБИРАЙ МУДРО. ЗАХИСТИ СВОЮ ЛЮДИНУ

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAA

`bb({ mouth:"normal" });`

n: ХАЙ ЩАСТИТЬ

```
Game.clearText();
bb({ eyes:"start" });
```

[Людино, ти можеш дійсно ВМЕРТИ тут!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[Це тупо і саморуйнуюче!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Ці прибиті насправді тобі не друзі!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Л--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Ц--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Ц--

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

h: Знаєш, я можливо б повірили тобі... якби ти не пробував те саме мільярд разів раніше.

h: Ти вовк, який кричав "Вовки!".

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

h: І це ти теж пробував.

b: людино, будь ласка...

`hong({ eyes:"look_right" });`

h: О, ну *вибач*, що Великій Фарма-мафії не подобаються мої власні ліки.

h: Слухай сюди, ^уйобку^, ми *всі* маємо свої методи, як змусити тебе закрити свій ^пиздак^.

`hong({ body:"look_up", eyes:"look_up" });`

h: Дехто кидається до роботу.

`hong({ body:"look_down", eyes:"look_down" });`

h: Дехто - до секс, наркотики і постійне гортання стрічки у Фейсбук.

`hong({ body:"normal", eyes:"look_right" });`

h: Деякі люди кидаються на допомогу іншим.. 

`hong({ eyes:"angry" });`

h: Я ж збираюсь кинутись у той басейн.

[Ти п'яні і тут СІМ ПОВЕРХІВ ДОНИЗУ](#act3_bad_1_harm)

[Ну капець, і отаке мені дякую?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Окей, визнаю, я провтикався.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Навіть якщо ти приземлишся, опір води поламає тобі ребра і в тебе буде струс мозку *щонайменше!*

h: Ех.

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

h: Я бачив як якась росня таке робила на Ютубі.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: Я- Перепрошую, це таке *дякую?*

`bb({ eyes:"angry" });`

b: Ось саме тому я й *існую*! Бо людям не можна довіряти турботу про самих себе!

b: Я намагався захистити твою тупу дупу все своє життя і тепер ти просто збирає--

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

h: хех.

`hong({ body:"laugh_2" })``

h: ахахахахахах

`hong({ body:"laugh_3" })``

h: АХАХАХАХАХАХАХАХ

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: Оу, ВАУ, це ^блять^ найбільше просвітлення за століття!

`hong({ body:"yell_2" });`

h: Так, ти, смердюча купа кривавого ^гівна^! Ти ^блять^ провтикався!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Ще якісь зауваження, Капітане Очевидність?

[Але помста мені - це не вихід!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Але цього разу я *дійсно* правий!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Я завдав тобі болю.](#act3_good_2a)


# act3_good_1_fail_revenge

b: Тобі варто налагодити здорові стосунки з емоціями, аніж топити їх в--

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

b: Тому, прошу, постав пляшку і давай--

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

b: будь ласка... не треба...

h: Твій рівень енергії виглядає жахливо малим, вовче.

h: На твоєму місці я б дуже обережно підбирали наступні слова.

`bb({ eyes:"normal" });`

[Окей. Я втомився тебе захищати.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Я увесь час був правий.](#act3_bad_2_right)

[Мені шкода.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: Ну, тоді давай стрибай. Побачимо, чи я відреагую.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Окей тоді. До дна.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: ЧЕКАЙ НІ ЦЕ БУЛА ЗВОРОТНА ПСИХОЛОГІЯ ТИ МАЛИ ЗРОБИТИ *ПРОТИЛЕЖНЕ* ВІД ТОГО, ЩО Я СКА--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: Ти *дійсно* наражаєш себе на небезпеку. Твої так звані друзі *дійсно* використовують тебе. І *ти* їх теж використовуєш.

`bb({ eyes:"sad" });`

b: Тож, будь ласка, людино... чому ти мені не віриш?!

h: Бо ти ніколи не вірив у *мене*.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Інаші сторожові вовки мають людей, які витрачають час, щоб терпляче їх тренувати, щоб *навчитися* працювати разом,

b: Аніж ненавидіти сторожових вовків за те, що ті намагаються їх захистити! То чому ти не можеш про--

`bb({ eyes:"normal" });`

h: Неправильна ^блять^ відповідь.

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

h: *"Єдине, чого варто боятися, - сам страх."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Don't worry, be happy!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Всі оті мудрагелі нашого часу погоджуються в одному: негативні емоції - *погані!*

`hong({ eyes:"less_angry" });`

h: Так! От чому вони називаються *негативні!*

b: людино... будь ласка...

`hong({ eyes:"normal" });`

h: Колись я сказали: "Я просто хочу звільнитися від усього цього болю."

h: І воно збулося. Я більше не відчуваю ні болю, ні страху, ні тривоги...

h: Я взагалі нічого не відчуваю.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Я так зосередився на тому, щоб не дозволити нікому зашкодити тобі, що не усвідомлював, що це *я* завдаю тобі болю.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: НІ. Б^ЛЯТЬ^.

`hong({ body:"yell_1" });`

h: ^СУКА^. Тобі треба було стільки часу, щоб нарешті це зрозуміти?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Мо могли уникнути стількох проблем, ти великий пухнастий довбо^йоб^. Чого ж ти не усвідомив того раніше?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...тобі *шкода.*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: Шкода за *що*?

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

[Мені шкода, що я був поганим захисником.](#act3_good_3_protector)

[Мені шкода, що я не поважав тебе.](#act3_good_3_respect)

[Мені шкода.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Мені шкода, що у мене така жахлва людина!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Мені шкода, що я не поважав тебе.](#act3_good_3_respect)

[Мені шкода, що я завдав тобі болю.](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: Мій обов'язок - захищати тебе від *справжньої* небезпеки, а я продовжував гавкати на машини і поштарів.

`bb({eyes:"sorry_up"});`

b: Гавкати на тіні. Так багато гавкати.

`bb({eyes:"sorry"});`

b: Логічно, що ти хотіли надянути намордник на мене.

`bb({eyes:"sorry_down"});`

b: Мені шкода.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: Я мав бути *твоїм* вірним сторожовим псом, але поводився так, ніби це ти маєш підкорятися *мені*.

`bb({eyes:"sorry_up"});`

b: Я різниця між захисником і наглядачем у в'язниці, і я перетнув межу.

`bb({eyes:"sorry_down"});`

b: Мені шкода.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Я так зосередився на тому, щоб не дозволити нікому зашкодити тобі, що не усвідомлював, що це *я* завдаю тобі болю.

`bb({eyes:"sorry_up"});`

b: Я був поганим псом.

`bb({eyes:"sorry_down"});`

b: Мені шкода.

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

h: Так, ну, це була тупа ідея.

h: Я так зробили тільки щоб тебе розізлити, і мені вдалося.

h: Зійдемося тут на нічиїй, окей?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Окей.

h: Окей.

n: *НІЧИЯ*

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

r: Ой, *камон*. Після всього, що той звір з тобою зробив, ти просто *здаєшся?*

r: Що з тобою, дитя? Ти що, *злякалися?*

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Так.

h2: Я злякалися.

`publish('hong-next')`

h2: І це нормально!

`publish('hong-next')`

h2: Нормально бути наляканими.

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

r: Вони що, щойно зачинили двері?

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

b: ні ні ні

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

b: НІ!

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
