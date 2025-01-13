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

n3: (гра автоматично збережена)

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

h: *зітхнули*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: То яка в ^біса^ мораль цієї історії?

`hong({body:"one_up", eyes:"annoyed"})`

h: Чого ми взагалі *навчилися*? Я *були* дурні, мої "друзі" *дійсно* використовували мене, і ми майже, бляха, *вмерли*.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Ага, і це ми ще не згадуємо про рахунок за лікування.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Ага, і це ми ще не згадуємо про шкоду для печінки.](#act4a_liver)
{{/if}}

[Ага, то *був* найгірший сценарій.](#act4a_worst)

[Ага, я був правий.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Дійсно. Я не думаю, що моя страховка покриває "бути довбо^йобом^.

`hong({eyes:"annoyed", mouth:"normal"});`

b: Але все ж... ми вижили!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Ми точно мінуснули кілька років нашої тривалості життя...

`bb({eyes:"surprise"});`

b: Але принаймні у нас все ще *є* тривалість життя! Ми вижили!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: І все ж...

h: Хм?

`bb({eyes:"surprise"});`

b: Ми вижили!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Але... ти теж були праві.

`hong({eyes:"surprise"});`

h: Хм?

`bb({eyes:"normal"});`

b: Я *був* вовком, який кричав "Вовки!". Тож, коли *справжня* небезпека підкралась, ти - справедливо - не повірили мені.

`bb({eyes:"surprise_r"});`

b: І все ж, ми вижили!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Попри все, ми все ще тут!.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: Ти виглядаєш доволі спокійним, враховуючи, що ми щойно ледь не вмерли.
{{/if}}

{{if !_.INJURED}}
h: Ти виглядаєш доволі спокійним, враховуючи, що ми щойно *ледь*-ледь не померли.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Ну, це робить все решта менш страшним у порівнянні. І ще це змусило мене задуматися.

`bb({eyes:"normal", mouth:"normal"});`

b: Якщо моя боротьба з тобою беззмістовна, бо це не захищає тебе...

h: Але моя боротьба *теж* не має сенсу, бо це тільки змушує тебе волати голосніше...

`bb({eyes:"normal_r"})`

b: Тоді, можливо...

`bb({eyes:"normal"})`

h: Можливо, ми не мусимо воювати.

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

b: Я не Злий Вовк. Але і не сторожовий вовк теж.

`bb({eyes:"sad_d"})`

b: Я побитий собака з притулку.

`bb({eyes:"sad"})`

b: Ми пройшли через тяжкі події. Можливо, травму або нехтуванн. Ось, чому я іноді надто реагую і роблю:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: ТЯВ ТЯВ ТЯВ ТЯВ ТЯВ ТЯВ

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Але я не *хочу* бути боягузливим псом! Я хочу захистити тебе! Я хочу бути хорошим собакою!

`bb({eyes:"sad", mouth:"normal"});`

b: Людино... допоможеш мені приборкати цього вовка?

`hong({eyes:"sad"})`

h: Я... я спробую.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Окей. Здорові взаємини з емоціями. Вони потребують розмови. Тож, давай поговоримо.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: Наступні п'ять хвилин звучатимуть дуже паскудно, але давай спробуємо, може щось і вийде.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Дорогий внутрішній вовку... як *ти* почуваєшся?

n2: ВСІ ВИКОРИСТАНІ СТРАХИ:

n2: *ПОСТРАЖДАТИ* {{_.attack_harm_total}}, *ПОКИНУТІСТЬ* {{_.attack_alone_total}}, *ПОГАНА ЛЮДИНА* {{_.attack_bad_total}}

n2: ПРО ЯКИЙ СТРАХ ТИ ХОЧЕШ ПОГОВОРИТИ ПЕРШИМ? (ПРО ІНШІ МОЖНА ПОТІМ)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Я боюсь, що нам нашкодять.](#act4_harm)

[Я боюся, що ми будемо самотні.](#act4_alone)

[Я боюся, що ми погані.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Я хочу захистити твою потребу у психологічній безпеці,

`bb({eyes:"sad_d"})`

b: Але *увесь світ* здається таким небезпечним. Сповненим трагедій і зла.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: Я хз, досить, щоб *я* вказував, що говорити далі. Що *ти* скажеш, людино?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Знову, повертаючись до тебе, людино. Що ти думаєш про це??
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Ще думки, людино?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Ти правий. Тож, давай захистимо нас.](#act4_harm_skills)

[Давай наразимося на *ще більшу* небезпеку.](#act4_harm_exposure)

[Дякую.](#act4_thanks) `_.thanks_for = "physical safety";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Але... як? У мене є кігті та ікла, але я тільки метафора.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Ми можемо навчитися самообороні? Приєднатися до спільноти, яка захищає одне одного? Покращити власне здоров'я і особисті кордони?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Можливо, але...

[Звідки нам взагалі почати?](#act4_harm_skills_start)

[Що як це все ще не спрацює?](#act4_harm_skills_work)

[Що як ми перестараємося з "безпекою"?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: Але нам треба стільки всього зробити, стільки всього виправити в нас. Звідки нам узагалі *почати*?

`hong({ body:"shrug", eyes:"surprise" })`

h: Ми починаємо прямо зараз.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Га?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Ми практикуємо хорошу комунікацію прямо заращ. Що допоможе нам розпізнати небезпеку краще, з меншою кількістю помилок,

`hong({ eyes:"surprise" });`

h: І *ось це* допоможе захистити нас від шкоди!

`hong({ eyes:"normal", mouth:"normal" });`

h: Тому, це *і є* тренування з самооборони.

`bb({ eyes:"normal_r" })`

b: Оу. Я очікував більше такого:

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

h: Дійсно, ми не можемо захистити себе на всі 100%...

`hong({ body:"one_up" });`

h: Але стати кращими на 1% це вже щось, так?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Ти бачиш, що стакан не на 99% порожній, а на 1% повний?

`bb({ eyes:"normal" });`

h: Що все-ще чогось вартує, якщо ти загубився посеред пустелі.

`bb({ eyes:"closed" });`

b: Ну. Тоді, до дна.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: я маю на увазі, ти ігнорували мої попередження, бо *Я* перестарався з безпекою! 

`bb({ body:"normal", eyes:"normal" })`

h: Ні, ти праві. Ми точно хочемо помірності у безпеці. Помірності у всьому.

`bb({ eyes:"suspect" })`

b: Перепрошую, помірності *У ВСЬОМУ*?

`hong({ eyes:"annoyed" })`

h: *Помірної кількості речей* у помірності.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Дякую, що робиш свої слова рекурсивно самоузгодженими.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *ЩО*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Ну, типу, скажімо, що собака боїться грому.

`hong({ body:"hands_1" });`

h: Дехто з експертів радить вмикати звук грому на програвачі на низькій гучності, а тоді частувати собаку за те, що той був спокійним.

`hong({ body:"hands_2" });`

h: Протягом кількох днів кінолог поступово підвищує гучність, доки собака не переборює свій страх грому.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Це називається "експозиційна терапія"!

`hong({ body:"point", eyes:"normal" });`

h: Оскільки ти пес, це мало би спрацювати і для тебе, так? Всі ссавці мають таку саму реакцію "бий-або-біжи".

`hong({ body:"normal" });`

[Що як ми *занадто* розслабимося?](#act4_harm_exposure_overboard)

[Що як ми стикнемося зі *справжньою* небезпекою?](#act4_harm_exposure_hurt)

[Я вовк, а не пес.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: І я проявлятиму до тебе доброту і терплячість, доки не приручу тебе настільки, що ти станеш милим маленьким щеням.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: О-оу.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: Ми *щойно* перевірили, що стається, якщо ти повнстю заткнеш свій страх - ти потрапляєш у *дійсно* небезпечні ситуації.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Крім того, чи, *надто* спокійні, ми не будемо схожі на психопата?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Скоро ми частуватимемо себе, дивлячись порно з вбивствами!

`hong({ eyes:"annoyed" })`

h: Я... думаю, є певна межа між цим і громом.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Але *де* точніше, людино? *Де?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: Я не знаю. Але *ти* можеш допомогти мені!

`hong({ eyes:"normal", body:"normal" })`

h: Працюючи і дискутуючи, ми проведемо цю межу.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Окей, але у мене лапки, тому ти малюватимеш.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: До прикладу: ми зістрибнули з клятого *даху!*
{{/if}}

{{if !_.INJURED}}
b: До прикладу: ми ледь не стрибнули з клятого *даху!* 
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Блін, ти праві. Ми *можемо* зайти задалеко.

`hong({ eyes:"normal" });`

h: Але ось чому, якщо ми займемося експозиційною терапією, ми починатимемо з малого і робитимемо маленькі кроки.

h: І перш ніж зіткнутися з *реальною* небезпекою, ми зупинимося.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Ага, я провів лінію між гучним звуком грому і стоянням в шторм з височезним гостроконечним капелюхом.

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

b: Чекай, жодних аргументів за чи проти того, що я відчуваю? Просто... "дякую"?

`hong({ eyes:"surprise", body:"shrug" })`

h: Ага! Дякую, що ти висловлюєш занепокоєння через моє {{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Все окей?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Ти ніколи не *дякували* мені раніше.

`hong({ mouth:"smile" });`

h: Оу, ти великий пухнастий-вухастий панічний вовчику.

(#act4_something_else)

# act4_thanks_2

h: Навіть якщо ти надто відреагуєш, я цінуватиму твоє піклування про моє {{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: Чекай... ти ж не повторюєш "дякую", щоб уникнути розмови про ці страхи, чи не так?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Ну, це складні речі, і у мене не завжди є відповіді.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: У житті в тебе немає трьох готових відповідей на вибір у діалозі.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Але поки що, я можу принаймні сказати "дякую".

b: Ну, дякую і тобі теж, що терпляче мене вислухали.

`bb({ eyes:"closed" });`

b: Ти, короткошерстий шкіряний ссавець.

(#act4_something_else)

# act4_thanks_3

h: Навіть якщо твоє тявкання лякає мене, ти просто намагаєшся захистити моє {{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: Окей, якщо ти продовжиш отак лестити мені, у людей в інтернеті почнуть з'являтися дивні ідеї про нас.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Камон, я прост вразлива дитина-підліток, а ти - великий страшний вовк. Що найгірше може тра--

`hong({ eyes:"normal", body:"point" });`

h: А знаєш, не відповідай краще.

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Я хочу переконатися, що ти заповниш ту глибоку людську потребу в приналежності...

`bb({ eyes:"sad_u" });`

b: Але я переживаю, що всі, хто нас знали, - *справжніх нас* - втекли налякані.

`bb({ eyes:"sad" });`

b: Я хз, досить, щоб *я* вказував, що говорити далі. Що *ти* скажеш, людино?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Знову, повертаючись до тебе, людино. Що ти думаєш про це??
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Ще думки, людино?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Окей: давай попрацюємо над нашою соціалізацією.](#act4_alone_skills)

[Думаю, інші люди нас люблять. Давай дізнаємось?](#act4_alone_experiment)

[Дякую.](#act4_thanks) `_.thanks_for = "social belonging";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Ми могли б попрактикувати навичку ставити запитання, слухати і бути емпатичними, бути відкритими і вразливими тощо?

`hong({ eyes:"normal_l" });`

h: Або почати кращі соціальні звички, як-от планувати час з друзями або ходити регулярно на заходи?

`hong({ body:"one_up" });`

h: Ми могли б також навчитися спокійніше реагувати на відмову.

`hong({ eyes:"normal" });`

h: Або навчитися відрізняти, коли люди *не* відмовляють нам, вони просто втомлені, або просто мають  такий Resting ^Bitch^ Face.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Ух, багато варіантів вибору. Але щодо "покращити соціальні навички"...

[Хіба це не *маніпулятивно?*](#act4_alone_skills_manipulative)

[Хіба це не зробть нас *схильними до маніпуляцій?*](#act4_alone_skills_manipulated)

[Що як нам усе ще не вдасться?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Хіба серійні вбивці, що чудово читають емоцї свої жертв, не майстри "емпатії"?

`bb({ eyes:"annoyed" });`

b: Хіба Чарльз Менсон не здобув друзів і вплив серед людей?

`hong({ eyes:"annoyed", body:"chin" });`

h: Ні, ти правий.

h: "Соціальні навички" нічого не варті, якщо ми щиро не піклуємось *про* людей.

`hong({ body:"normal" });`

h: Коротше, просто не будь ^уйобком^.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Звучить як текст з мотиваційного постера.

`hong({ body:"shrug", mouth:"narrow" });`

h: “Не Будь ^Уйобком^™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Ми станемо килимком під дверима, говорячи "Дякую" і "Будь ласка", доки люди витиратимуть об нас ноги!

`bb({ mouth:"scream", eyes:"scream" })`

b: Ми стільки дуп лизатимемо, що виглядатиме, наче у нас коричнева помада!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Ні, ти правий. "Соціальні навички" - це не просто про догоджання іншим, воно також несе за собою встановлення *кордонів*.

`hong( body:"one_up" });`

h: Ми не можемо запросити інших додому, якщо там немає стін, які б його тримали.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: А ще... картинка в голові з коричневою помадою... *фу??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: У нас може не вдатися. Насправді у нас *точно* не вдасться.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: І це нормально! Всі вчаться на своїх невдачах спершу!

`hong({ body:"normal", eyes:"normal" });`

h: Тож, давай проторювати собі шлях, так?

`bb({ eyes:"normal_r" });`

b: Ну так, думаю... найгірший сценарій - просто втекти з міста і створити собі нову ідентичність

`bb({ eyes:"normal" });`

h: Так, думаю, це коштуватиме нам всього двох біткоїнів тепер.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Ми можемо поекспериментувати!

`hong({ body:"chin" });`

h: Ми можемо запросити друга прогулятися, зустрітися зі старим товаришем, або навіть побалакати з баристою.

`hong({ body:"normal" });`

h: Думаю, ми можемо виявити, що ми більш приємні, ніж думали.

`bb({ eyes:"annoyed" });`

[Що як це малі неважливі "перемоги"?](#act4_alone_experiment_cheap)

[Що як це тягар для інших?](#act4_alone_experiment_burden)

[Але такі поверхневі розмови - то не *справжні* ми!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Якщо ми начепимо фейкову посмішку, то ніколи не зблизимося ні з ким,

`bb({ eyes:"super_sad" });`

b: *Але* якщо ми відкриємося, то інші можуть побачити, які ми травмовані всередині!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Переверний.

b: Що.

`hong({body:"hands_1"})`

h: Коли собаки хочуть проявити любов і довіру, вони робляться вразливими, показуючи пузо.

`hong({body:"one_up"})`

h: Може, ми *ще* не надто в безпеці, щоб бути вразливими, але з достатньою кількістю тренувань,

`hong({body:"normal", eyes:"surprise"})`

h: Одного дня ми зможемо показати людям себе справжніх - травмованих, людяних.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Я перевернусь, якщо ти мене почастуєш чимось.

`bb({ eyes:"normal", mouth:"normal" });`

h: Ні.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Сказати "здоров" баристі це не зовсім золота медаль на Олімпійських Іграх Соціальних Метеликів.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Це не для *нас!*

`hong({ body:"one_up", eyes:"annoyed" });`

h: На соціальній арені, ми навіть не в пір'ячково-легкій вазі, ми типу... у кварковій вазі.

`hong({ body:"normal", eyes:"normal" });`

h: Якщо ми мусимо почати з малих неважливих перемог, т отак тому й бути. Треба ступити на першу сходинку, перш ніж стати на стопершу.

b: Так! Можливо, сказавши "здоров" ми навіть змодемо просунутися до...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Як у тебе справи?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Потроху!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Може, бариста просто хоче зробити нам нашу кляту каву, а не бути *експериментом*, щоб перевірити, чи наші соціальні навички досі не працюють.

`bb({ eyes:"annoyed" })`

h: Що ж, якщо виявиться, що ми таки *є* тягарем...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: То це теж добре знати!

`hong({ eyes:"normal" });`

h: Ми можемо тоді дізнатися, як проактивно спитати в когось, як їм буде комфортніше, щоб знати і поважати кордони інших.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Знаєш, отой весь ^пиздьож^ про "внутрішні навички" в психологічних брошурах.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Я хочу захистити твої психологічні потреби, що веде до того, аби бути кращою людиною,

`bb({ eyes:"sad_d" })`

b: Але здається, що глибоко всередині, ми такі фундаментально... зламані.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: І не кажи мені, що ми *не* травмовані. Ми стрибнули з *даху*.
{{/if}}

{{if !_.INJURED}}
b: І не кажи мені, що ми *не* травмовані. Ми ледь не стрибнули з *даху*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

b: Я хз, досить, щоб *я* вказував, що говорити далі. Що *ти* скажеш, людино?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Знову, повертаючись до тебе, людино. Що ти думаєш про це??
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Ще думки, людино?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Тож, ми поламані. Давай виправимо це.](#act4_bad_fix)

[Тож, ми поламані. Давай приймемо це.](#act4_bad_accept)

[Дякую.](#act4_thanks) `_.thanks_for = "moral well-being";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Нам варто повільно створювати корисні звички, узгоджувати своє життя з нашими цінностями,

`hong({body:"one_up"});`

h: І якщо потрібно, звернутися по професійну допомогу - психотерапевта чи психолога.

`hong({body:"normal"});`

h: Є безліч способів це виправити.

[Що як нам не вдасться виправити все?](#act4_bad_fix_cant)

[Що як ми виправимо *надто* багато?](#act4_bad_fix_too_much)

[Ми не можемо дозволити собі професійну допомогу.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Ні, думаю, ти правий..

h: МИ не можемо виправити все.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ааааа я так і знав, що ми завжди будемо поламані!

`hong({eyes:"surprise"});`

h: Але ми принаймі можемо бути *менш* поламаними.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Рани загоюються з часом, але вони залишають шрами. І це нормально.

`bb({eyes:"annoyed_r"});`

b: Ну, я сподіваюсь. Між іншим,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Шрами це *сексуально.*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Будь ласка, не роби так.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Важко це визнавати, але... деяка частина мене *хоче* мати цей розлад.

`bb({ eyes:"angry" })`

b: Типу, без цього хіба ми не будемо *нудними?*

`bb({ eyes:"sad_r", body:"one_up" })`

b: Без розладу, хіба наша творчість не буде прісною і нудною?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Без розладу, хіба ми не втратимо зв'язок з друзями, які його мають?

`bb({ eyes:"sad", body:"chest" })`

b: Якщо ми коли-небудь будемо задоволені життям, хіба нас це не зупинить на шляху до більшого успіху?

`hong({ MOUTH_LOCK:true })`

h: ...

h: Якщо ми навіть боїмося... "втратити всі страхи"...

h: Не думаю, що нам колись вдасться втратити їх усіх.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: О так! Хух! Яке полегшення!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Лікарю, боюсь, я плачу вам 100$/год лише щоб ви мене запитали *«як це змушує вас почуватися?»*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "М-гм. І як це змушує вас почуватися?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Ні, це цілком резонне зауваженя.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: І мене дійсно дратує, що туробота про ментальне здоров'я не є доступною для кожного.

`hong({ eyes:"normal", mouth:"normal" });`

h: Все ж, є деякі дешеві чи безкоштовні варіанти:

`hong({ body:"chin" })`

h: Групи підтримки, онлайн терапія, студентські/неприбуткові центри...

`hong({ body:"hands_1" })`

h: Створювати звички як-от медитація, здоровий сон, регулярні розмови з друзями, вивчення нового...

`hong({ body:"hands_2" })`

h: Піти до бібліотеки по книжку з науково доведеними методами психотерапії...

`hong({ body:"one_up" })`

h: Є цілий список ресурсів у кінці цієї гри!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Ну, *ця* четверта стіна довго не протримається.

`hong({ body:"point" });`

h: Деякі речі важливіші за цільність діалогу і сюжету в грі. Наприклад, психічне здоров'я.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Типу, це ж те, що всі терапевти кажуть, так? Прийми свої емоції, навіть негативні?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Чекай.

["Прийми" як і *здайся*?](#act4_bad_accept_give_up)

["Прийми" як і *схвалюй*?](#act4_bad_accept_approve)

["Прийми" як і *сприймай буквально*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Думаєш, Мартін Лютер Кінг сказав би "Тупо, що ми не можемо сидіти спереду автобуса, але давай просто *приймемо* це?"

`bb({ eyes:"angry_r", body:"two_up" });`

b: Чому Індустрія Самодопомоги вважає розмахування білим прапором якимось *глибоким пізнанням?*

`bb({ eyes:"annoyed", body:"normal" });`

h: Я думаю, що терапевти під "прийняттям" поганого мають на увазі усвідомлення, що вони існують  і що їх важко змінити,

h: Але необов'язково здаватися на шляху до змін.

`bb({ eyes:"suspect" });`

b: Тоді психотерапевти мали би говорити "усвідом" замість "прийми".

`hong({ body:"chin", eyes:"annoyed" });`

h: Ну так, подумай, "прийняти" - доволі розпливчасте поняття.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Ну, я це *усвідомлюю*.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Типу, це *добре*, що ми поламані? Ні!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Всі ті кляті голівудські сценаристи, які романтизують психічні розлади, просто психи!

`bb({ eyes:"angry", body:"two_up" });`

b: Мати психічний розлад *тупо*! Він псує людям *життя*! Чому ми мусимо його "приймати"?!

`bb({ body:"normal" });`

h: Думаю, психотерапевти під "приймати" наші емоції мають на увазі терпляче до них ставитись.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Типу, так само, як що більше ти борсаєшся в сипучих пісках, то більше ти тонеш, а найкраще лежати нерухомо,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Моя боротьба з тобою, страху, привела мене до стрибка з даху.
{{/if}}

{{if !_.INJURED}}
h: Моя боротьба з тобою, страху, ледь не привела мене до стрибка з даху.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Натомість, найкращим рішенням буде не боротися, а просто бути терплячими одне з одним.

`bb({ eyes:"annoyed" });`

b: Тоді треба було *так* і казати, аніж оте проблемне "прийми".

`hong({ body:"chin", eyes:"annoyed" });`

h: Ага, якщо подумати, "прийняття" звучить тупо.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: Я не приймаю "прийняття".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Але ми вже *знаємо*, що не варто сприймати мене буквально!

`bb({ eyes:"sad_u", body:"two_up" });`

b: Вся *проблема* в тому, що я хочу допомогти тобі, але не можу підібрати слів!

`bb({ eyes:"sad", body:"normal" });`

h: Я думаю, терапевти під "прийняттям" наших емоцій мають на увазі "не борись, але й не ігноруй їх."

`hong({ eyes:"surprise", body:"one_up" });`

h: Слухати себе, *співпрацювати* з собою, але не сприймати все як 100% правду.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Тоді терапевти мали б сказати *це* замість такого розпливчастого терміну як "прийняття".

`hong({ body:"chin", eyes:"annoyed" });`

h: Ну, думаю, їм теж важко підбирати слова.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: В будь-якому разі, є ще щось, про що ти хочеш поговорити?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: Тож, є ще щось, що лежить каменем на душі?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Я переживаю, що нам нашкодять.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Я переживаю, що ми будемо самі.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Я переживаю, що ми - погані.](#act4_bad)
{{/if}}

[Ні, поки нормально.](#act4c_prelude)

# act4_something_else_2

h: Окей, думаю, ми поговорили про всі страхи тепер.

b: Так, їх є тільки три.

h: Ага, саме три.

b: Зручно.

(#act4c)

# act4c_prelude

h: Класно поговорили, напарнику.

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

b: Ти ж знаєш, що це не *гра*.

`bb({eyes:"angry_d", body:"one_up"})`

b: Збудувати здорові стосунки зі своїми емоціями це важче ніж тикати кнопочки на екрані.

`bb({eyes:"sad", body:"normal"})`

b: Ми дійсно *можемо* порозумітися?

b: Ми дійсно *можемо* працювати разом, як команда?

`hong({eyes:"sad", body:"one_up"})`

h: Ну,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: П-перепрошую...

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

a: Ч-ч-чи ви не проти, якщо я підсяду до вас на обіді?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *То це* і є твій краш? Чому вони сидять самі як якийсь псих-маніяк?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Спитатися в краша, чи ми можемо з ними сісти? Ти хоч уявляєш, як *нав'язливо* ми звучимо?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *То це* і є твій краш?  Ми перервали їх тишу і спокій! Ми такий тягар!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: Я- я маю на увазі- це, це цілком окей, якщо ні, я просто...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Чекай, ми часом не бачились на вечірці?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Так, звісно! Ходи.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Вибач, мені потрібно побути насамоті поки.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Так, ти сиділи на дивані. На першій вечірці...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Коли у мене була та панічна атака і я вдарили господаря.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Коли у мене була та панічна атака і я втекли в сльозах.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Чекай, людино, ми, можливо, робимо їм некомфортно.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Оу, я не хотіли тебе заскочити зненацька!

`publish("act4", ["hong_to_alshire",4]);`

h2: Просто пригадали знайоме дружнє лице, ото й усе.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: ААААА Я ТАК І ЗНАВ! ВОНИ - НЕБЕЗПЕЧНИЙ ПАНІЧНИЙ ПСИХ!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: ААААААААА ПЕРШЕ ВРАЖЕННЯ ПРО НАС ЦЕ "ВОНИ ЗАСТАЛИ НАШУ ТРАВМУ"! ЦЕ ЗНАЧИТЬ, ЩО ВОНИ НАС НЕНАВИДЯТЬ!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: ААААААААА МИ ЗМУСИЛИ КОГОСЬ ЗГАДАТИ ТРАВМАТИЧНУ ПОДІЮ. САМА НАША ПРИСУТНІСТЬ ЗАВДАЄ БОЛЮ ІНШИМ.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Чекай, людино. Їм, здається, некомфортно.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Оу, я не наполягаю, звісно!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Просто кажу, що можеш сісти, якщо хочеш.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: ВОНИ *НАДТО* ДРУЖЕЛЮБНІ! ЯК ТЕД БАНДІ, СЕРІЙНИЙ ВБИВЦЯ!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: ВОНИ ПРОСТО ПОВОДЯТЬСЯ ВВІЧЛИВО! НІХТО *НАСПРАВДІ* НЕ ХОЧЕ З НАМИ ЗВ'ЯЗУВАТИСЬ!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: АААААА МИ ЗАВЖДИ ЗМУШУЄМО ІНШИХ ПОЧУВАТИСЬ НЕЗРУЧНО! МИ ТЕМНА ПЛЯМА НА ЗЕМЛІ!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Чекай, людино. Ми змушуємо їх почуватися некомфортно.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Оу, я не хотіли здатися нечемними!

`publish("act4", ["hong_to_alshire", 6]);`

h2: Мені потрібно трохи часу, щоб розібратися зі своїми емоціями. Будь ласка, не сприймай цей як особисту відмову.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: ЯКІ ЖАХЛИВІ СТРАШНІ ДУМКИ У НИХ В ГОЛОВІ?! ЯКІ ТЕМНІ ПРАГНЕННЯ НАПОВНЮЮТЬ СЕРЦЕ ЦЬОГО ПСИХА?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: НАМ ОСОБИСТО ВІДМОВИЛИ! НАС НІКОЛИ НЕ ПОЛЮБЛЯТЬ!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: МИ ПЕРЕРВАЛИ ЇХ ЧАС НА ВЛАСНІ ЕМОЦІЇ! ТЕПЕР ВОНИ ЗАВЖДИ БУДУТЬ ТРАВМОВАНІ І ЦЕ ВСЕ - НАША ПРОВИНА!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: ТІКАЙ ТІКАЙ ТІКАЙ ТІКАЙ ТІКАЙ ТІКАЙ ТІКАЙ ТІКАЙ ТІКАЙ 

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

h: Гм. Це було дивно. Цікаво, що у них в голові діється.

`publish("act4", ["hong_closer", 2]);`

h: Ну, то що ти там казав?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Ем, я забув? Щось про команду і роботу?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Кажуть, що треба "примиритися" зі своїми емоціями, так наче вони якісь *воєнні злочинці*.

`publish("act4", ["bb_closer", 7]);`

b: Але я б хотів, щоб у нас було щось *більше*, ніж просто мир! Я хочу, щоб ми були *союзниками!*

`publish("act4", ["bb_closer", 3]);`

b: Я хочу бути хорошим сторожовим псом. Як голод і спрага є попередженнями про твої фізичні потреби,

`publish("act4", ["bb_closer", 8]);`

b: Я хочу попереджати про твої *психологічні* потреби - потребу в безпеці, приналежності, доброті.

`publish("act4", ["bb_closer", 1]);`

b: Але... моя робота мені не дуже вдається, тож треба, щоб ти мене потренували.

`publish("act4", ["bb_closer", 4]);`

b: Я не "завжди валідний" чи "завжди ірраціональний". Я просто... стараюся з усіх сил. Тож, будь ласка,

`publish("act4", ["bb_closer", 30]);`

b: Допоможи мені допомагати тобі!

`publish("act4", ["bb_closer", 6]);`

b: Хоч, щоб навчити старого собаку новим трюками, *потрібен* час. Можливо *роки*.

`publish("act4", ["bb_closer", 3]);`

b: Й іноді я повертатимусь назад, до своїх старих звичок.

`publish("act4", ["bb_closer", 2]);`

b: Я гавкатиму на тіні. Лякатиму тебе словами. Можу навіть показати якісь нав'язливі картинки... всякого.

`publish("act4", ["bb_closer", 9]);`

b: І мені шкода! Я побити й пес з притулку! Побиті пси іноді какають тобі на ліжко!

`publish("act4", ["bb_closer", 4]);`

b: Але якщо ти будеш терплячими зі мною... якщо ти залишишся і посидиш зі мною...

`publish("act4", ["bb_closer", 8]);`

b: Можливо, ти приручиш цього вовка.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Хороший песик.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Хороша людина.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

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
b: АААА ТИ ВСЕ ЩЕ ЇСИ НА САМОТІ П'ЯТНАДЦЯТЬ ЦИГАРОК АААА
{{/if}}

{{if _.parasite}}
b: АААА ТИ ВСЕ ЩЕ НЕ ПРОДУКТИВНІ ПОКИ ЇСИ МИ СОЦІАЛЬНИЙ ПАРАЗИТ АААА
{{/if}}

{{if _.whitebread}}
b: АААА ТИ ЇСИ ЩЕ БІЛЬШЕ БІЛОГО ХЛІБА АААА
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

b: ТЯВ ТЯВ ТЯВ ТЯВ ТЯВ ТЯВ

(#credits)
